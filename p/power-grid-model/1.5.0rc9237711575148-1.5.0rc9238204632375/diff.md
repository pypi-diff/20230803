# Comparing `tmp/power-grid-model-1.5.0rc9237711575148.tar.gz` & `tmp/power-grid-model-1.5.0rc9238204632375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9237711575148.tar", last modified: Wed Aug  2 07:21:29 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9238204632375.tar", last modified: Wed Aug  2 13:34:08 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9237711575148.tar` & `power-grid-model-1.5.0rc9238204632375.tar`

### file list

```diff
@@ -1,593 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.075359 power-grid-model-1.5.0rc9237711575148/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 07:21:29.075359 power-grid-model-1.5.0rc9237711575148/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 07:20:44.000000 power-grid-model-1.5.0rc9237711575148/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.003358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.003358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.003358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    61599 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24917 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.007358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    56026 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.011358 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    94102 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:21:29.075359 power-grid-model-1.5.0rc9237711575148/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.011358 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.011358 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.015358 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.011358 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 07:21:28.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-08-02 07:21:28.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:21:28.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-02 07:21:28.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 07:21:28.000000 power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.015358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.015358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.015358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.019358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.019358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.023358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.023358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.023358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.027358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.027358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.027358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.027358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.031358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.031358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.031358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.031358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.035359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.035359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.035359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.035359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.039358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.039358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.039358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.043358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.043358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.043358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.043358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.047359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.047359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.047359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.995358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.051359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.051359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.051359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.051359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.055359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.055359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.055359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.059359 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.059359 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   234523 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.059359 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    57182 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.063359 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   226262 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.063359 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   234409 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:28.999358 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.063359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.063359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.067359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.067359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.067359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.067359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.071359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.071359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.071359 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.071359 power-grid-model-1.5.0rc9237711575148/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:21:29.075359 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-08-02 07:20:40.000000 power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.224062 power-grid-model-1.5.0rc9238204632375/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 13:34:08.224062 power-grid-model-1.5.0rc9238204632375/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 13:33:21.000000 power-grid-model-1.5.0rc9238204632375/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.144060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.144060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.136060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.144060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.144060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.144060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.148060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.148060 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    61599 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24917 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56026 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    94102 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:34:08.224062 power-grid-model-1.5.0rc9238204632375/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.136060 power-grid-model-1.5.0rc9238204632375/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.152061 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.156061 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.156061 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.156061 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-02 13:34:08.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-08-02 13:34:08.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:34:08.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-02 13:34:08.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 13:34:08.000000 power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.156061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.160061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.160061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.160061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.168061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.168061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.168061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.172061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.172061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.172061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.176061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.176061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.176061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.176061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.180061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.180061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.180061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.180061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.184061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.184061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.184061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.184061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.188061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.188061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.188061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.188061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.192061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.192061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.192061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.196061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.196061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.196061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.196061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.200061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.200061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.200061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.204061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.204061 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.204061 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   255637 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.208061 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    62578 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.208061 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   250520 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.208061 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   255901 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.140060 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.212061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.212061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.212061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.216061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.216061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.216061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.220061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.220061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.220061 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.224062 power-grid-model-1.5.0rc9238204632375/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:34:08.224062 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-08-02 13:33:15.000000 power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9237711575148/LICENSE` & `power-grid-model-1.5.0rc9238204632375/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/PKG-INFO` & `power-grid-model-1.5.0rc9238204632375/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9237711575148
+Version: 1.5.0rc9238204632375
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9237711575148/README.md` & `power-grid-model-1.5.0rc9238204632375/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9238204632375/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/pyproject.toml` & `power-grid-model-1.5.0rc9238204632375/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/setup.py` & `power-grid-model-1.5.0rc9238204632375/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9237711575148
+Version: 1.5.0rc9238204632375
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9237711575148/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9238204632375/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9238204632375/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -12,36 +12,36 @@
     ],
     "line": [
         {
             "c0": 6.4e-07,
             "c1": 6.4e-07,
             "from_node": 1,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 7,
             "r0": 0.75,
             "r1": 0.049,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 2,
             "to_status": 1,
             "x0": 0.04,
             "x1": 0.153
         },
         {
             "c0": 3.2e-07,
             "c1": 3.2e-07,
             "from_node": 2,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 8,
             "r0": 0.375,
             "r1": 0.0245,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 3,
             "to_status": 1,
             "x0": 0.02,
             "x1": 0.0765
         }
     ],
     "node": [
@@ -61,60 +61,60 @@
             "id": 3,
             "u_rated": 10000.0
         }
     ],
     "shunt": [
         {
             "b0": 5.0,
-            "b1": 0,
-            "g0": 0,
-            "g1": 0,
+            "b1": 0.0,
+            "g0": 0.0,
+            "g1": 0.0,
             "id": 9,
             "node": 1,
             "status": 1
         }
     ],
     "source": [
         {
             "id": 4,
             "node": 0,
             "rx_ratio": 0.1,
             "sk": 20000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": 0.0,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         },
         {
             "id": 5,
             "node": 2,
             "rx_ratio": 0.1,
             "sk": 2000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": -0.5235987755982988,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         }
     ],
     "transformer": [
         {
             "clock": 1,
             "from_node": 0,
             "from_status": 1,
-            "i0": 0,
+            "i0": 0.0,
             "id": 6,
-            "p0": 0,
-            "pk": 0,
+            "p0": 0.0,
+            "pk": 0.0,
             "sn": 20000000.0,
             "tap_max": 1,
             "tap_min": -1,
             "tap_nom": 0,
             "tap_pos": 0,
             "tap_side": 0,
-            "tap_size": 100,
+            "tap_size": 100.0,
             "to_node": 1,
             "to_status": 1,
             "u1": 150000.0,
             "u2": 10000.0,
             "uk": 0.05,
             "winding_from": 1,
             "winding_to": 2
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {'0': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer': [OrderedDict([('id', 6), "*

 * *      "('energized', 1), ('i_from', [0.33791566956759234, 0.12770399637309612, "*

 * *      "0.3379238102470673]), ('i_from_angle', [1.2372270219475148, -0.5236056997455355, "*

 * *      "-2.284563617669219]), ('i_to', [5.74750397032484, 3.318110750024341, 3.3182972821545613]), "*

 * *      "('i_to_angle', [-2.094466942439717, 1.5706786199378147, 0.5236052533305937])])]}",*

 * * '1': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transfor […]*

```diff
@@ -1,22 +1,12 @@
 [
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.74747402954125,
-                    8.041086459980025e-16,
-                    6.009258394948638e-16
-                ],
-                "i_angle": [
-                    -2.094499242824724,
-                    -0.08457559607190217,
-                    0.0
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -185,30 +175,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33791566956759234,
+                    0.12770399637309612,
+                    0.3379238102470673
+                ],
+                "i_from_angle": [
+                    1.2372270219475148,
+                    -0.5236056997455355,
+                    -2.284563617669219
+                ],
+                "i_to": [
+                    5.74750397032484,
+                    3.318110750024341,
+                    3.3182972821545613
+                ],
+                "i_to_angle": [
+                    -2.094466942439717,
+                    1.5706786199378147,
+                    0.5236052533305937
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    61463.949515399676,
-                    4.011906280418248e-12,
-                    4.6412457148092364e-12
-                ],
-                "i_angle": [
-                    1.0504076684695445,
-                    2.528772451424552,
-                    2.356194490192345
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -377,30 +383,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2365.819661825651,
+                    0.1277039963730371,
+                    2365.820072653962
+                ],
+                "i_from_angle": [
+                    -2.091211974561429,
+                    -0.5236056997407288,
+                    1.050434657497871
+                ],
+                "i_to": [
+                    40977.20210122772,
+                    20488.59578095684,
+                    20488.606454589426
+                ],
+                "i_to_angle": [
+                    1.0504076682654613,
+                    -2.091265953049525,
+                    -2.09110401764132
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    22402.312747881486,
-                    1.8346134549116837e-12,
-                    2.051160198809135e-12
-                ],
-                "i_angle": [
-                    2.23297612691668,
-                    -2.0344439357957027,
-                    -2.498091544796509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -569,30 +591,46 @@
                 "i_angle": [
                     -0.8473731745890964,
                     -1.0504973838084937,
                     -1.0508959932953557
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    392.4581915819866,
+                    0.028527483315196944,
+                    392.4840416381267
+                ],
+                "i_from_angle": [
+                    -1.0503052480947048,
+                    -0.6135741734012512,
+                    2.0913181495331368
+                ],
+                "i_to": [
+                    6797.799143915923,
+                    3398.5637734928873,
+                    3399.2353776514447
+                ],
+                "i_to_angle": [
+                    2.0913027780203506,
+                    -1.0503359961830285,
+                    -1.050243764068141
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    205032.25844191352,
-                    2.80401926733944e-11,
-                    2.5047681269829595e-11
-                ],
-                "i_angle": [
-                    2.2049079962374933,
-                    -1.9295669970654687,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -761,30 +799,46 @@
                 "i_angle": [
                     -1.0512241307607684,
                     2.769081609693555,
                     2.7690738170091738
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    3592.077710973006,
+                    0.028527483314505966,
+                    3592.1032115667294
+                ],
+                "i_from_angle": [
+                    -1.078410677446369,
+                    -0.6135741733901677,
+                    2.0631855362318077
+                ],
+                "i_to": [
+                    62216.831842930784,
+                    31108.084659479322,
+                    31108.7471843386
+                ],
+                "i_to_angle": [
+                    2.0631837561939346,
+                    -1.0784142375853008,
+                    -1.0784035573201483
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.748158405083368,
-                    8.18684547740158e-16,
-                    8.258935698000961e-16
-                ],
-                "i_angle": [
-                    -2.0944632553048095,
-                    -0.2068378622272056,
-                    -0.24497866312686414
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -953,30 +1007,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379493154850622,
+                    0.12770399637317842,
+                    0.33795527136631337
+                ],
+                "i_from_angle": [
+                    1.2372252868487605,
+                    -0.5236056997451537,
+                    -2.2845282826909568
+                ],
+                "i_to": [
+                    5.7480781562560095,
+                    3.3183844217710248,
+                    3.318520895266836
+                ],
+                "i_to_angle": [
+                    -2.0944495201197593,
+                    1.570648433648122,
+                    0.5236615714162574
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    17760.976526474282,
-                    2.051160198809135e-12,
-                    2.469923953021461e-12
-                ],
-                "i_angle": [
-                    1.9601627077040327,
-                    -2.214297435588181,
-                    -2.297438667476622
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1145,30 +1215,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    683.5757682608864,
+                    0.12770399637281488,
+                    683.6768327564602
+                ],
+                "i_from_angle": [
+                    -1.1813690329610833,
+                    -0.5236056997437116,
+                    1.9603378143917738
+                ],
+                "i_to": [
+                    11840.75483941297,
+                    5919.064640268169,
+                    5921.690372851553
+                ],
+                "i_to_angle": [
+                    1.9602807217307257,
+                    -1.1814832604940173,
+                    -1.1811406791928294
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    136915.96230745324,
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11
-                ],
-                "i_angle": [
-                    1.148330201987778,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1337,30 +1423,46 @@
                 "i_angle": [
                     -1.9947264499020332,
                     -1.974244983047042,
                     -1.9747637940348024
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    571.6103589428899,
+                    0.02852748331542307,
+                    571.6163028687619
+                ],
+                "i_from_angle": [
+                    -1.9744992190226975,
+                    -0.6135741733991866,
+                    1.1671422462012484
+                ],
+                "i_to": [
+                    9900.633311177093,
+                    4950.239454995499,
+                    4950.393882719229
+                ],
+                "i_to_angle": [
+                    1.1671178405110643,
+                    -1.9745480316718862,
+                    -1.9744015967696296
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    136727.84188424365,
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11
-                ],
-                "i_angle": [
-                    1.171820801074162,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1529,30 +1631,46 @@
                 "i_angle": [
                     -1.9947264499020334,
                     -2.487043174079903,
                     -2.4874465649398103
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    570.8247385314772,
+                    0.028527483315286383,
+                    570.8313362052144
+                ],
+                "i_from_angle": [
+                    -1.9510075203121573,
+                    -0.6135741733990432,
+                    1.1906337539848402
+                ],
+                "i_to": [
+                    9887.031628146427,
+                    4943.430120924612,
+                    4943.601533516075
+                ],
+                "i_to_angle": [
+                    1.1906094437717287,
+                    -1.9510561421431893,
+                    -1.9509102800217686
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.748468897310853,
-                    4.344673780753835e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.094554694044177,
-                    -0.39735401778895213,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1721,30 +1839,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795801274392934,
+                    0.1277039963731637,
+                    0.3379717173258611
+                ],
+                "i_from_angle": [
+                    1.237158544639972,
+                    -0.5236056997450331,
+                    -2.2845807091515065
+                ],
+                "i_to": [
+                    5.748299897509254,
+                    3.318391663394129,
+                    3.3187056937756316
+                ],
+                "i_to_angle": [
+                    -2.094511309907328,
+                    1.5705853814019168,
+                    0.5236319245461281
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12543.843934648457,
-                    1.1603114287023091e-12,
-                    1.1603114287023091e-12
-                ],
-                "i_angle": [
-                    2.040795602241189,
-                    -2.356194490192345,
-                    -2.356194490192345
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1913,30 +2047,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    482.7527666890548,
+                    0.12770399637316113,
+                    482.859795045005
+                ],
+                "i_from_angle": [
+                    -1.1006884836561186,
+                    -0.5236056997441245,
+                    2.0410484621992997
+                ],
+                "i_to": [
+                    8362.450064987113,
+                    4179.834791330796,
+                    4182.615469528245
+                ],
+                "i_to_angle": [
+                    2.040976324063154,
+                    -1.1008328399133507,
+                    -1.1003999630799406
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35448.479883073465,
-                    4.10232039761827e-12,
-                    3.1309601587286993e-12
-                ],
-                "i_angle": [
-                    1.9999451994518511,
-                    -2.214297435588181,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2105,30 +2255,46 @@
                 "i_angle": [
                     -1.1430836906933466,
                     -1.1229205767117405,
                     -1.1240992170421655
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    147.97693112895487,
+                    0.028527483315241034,
+                    148.00184016008106
+                ],
+                "i_from_angle": [
+                    -1.1227712824547507,
+                    -0.6135741733992833,
+                    2.018915332629333
+                ],
+                "i_to": [
+                    2563.2513463433024,
+                    1281.3021080979902,
+                    1281.9492637044427
+                ],
+                "i_to_angle": [
+                    2.0188683558360014,
+                    -1.1228652755867088,
+                    -1.1225833910895235
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35279.978347555196,
-                    4.10232039761827e-12,
-                    4.78848169866233e-12
-                ],
-                "i_angle": [
-                    2.0037248298386054,
-                    -2.214297435588181,
-                    -2.32590073027357
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2297,30 +2463,46 @@
                 "i_angle": [
                     -1.162795058082173,
                     -1.6549429599546457,
                     -1.6565097193635687
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    147.27347351062767,
+                    0.02852748331535079,
+                    147.29843493448598
+                ],
+                "i_from_angle": [
+                    -1.1189905522583279,
+                    -0.613574173398919,
+                    2.0226958715269503
+                ],
+                "i_to": [
+                    2551.06755674343,
+                    1275.2095325844537,
+                    1275.8580493940253
+                ],
+                "i_to_angle": [
+                    2.0226489904021547,
+                    -1.1190843542446518,
+                    -1.1188030436436878
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.747526034574178,
-                    8.041086459980025e-16,
-                    8.012344526598184e-16
-                ],
-                "i_angle": [
-                    -2.0945082930762267,
-                    -0.08457559607190217,
-                    0.0
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2489,30 +2671,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33791725691064484,
+                    0.12770399637327606,
+                    0.33792615429513784
+                ],
+                "i_from_angle": [
+                    1.2372200838188165,
+                    -0.5236056997452951,
+                    -2.284568317003021
+                ],
+                "i_to": [
+                    5.7475386418368215,
+                    3.3181170939817246,
+                    3.3183209651975596
+                ],
+                "i_to_angle": [
+                    -2.094472976587306,
+                    1.570671481826725,
+                    0.5236033392503372
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    55809.55246338669,
-                    6.678093778054823e-12,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    1.1381080045539778,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2681,30 +2879,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2148.1599442770134,
+                    0.12770399637298238,
+                    2148.171539376016
+                ],
+                "i_from_angle": [
+                    -2.003509726602329,
+                    -0.5236056997399869,
+                    1.1381421293601008
+                ],
+                "i_to": [
+                    37207.32206292302,
+                    18603.51048006251,
+                    18603.81172957033
+                ],
+                "i_to_angle": [
+                    1.1381125282536713,
+                    -2.003568929613874,
+                    -2.0033913224963684
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21414.663285460443,
-                    1.4791126541994494e-12,
-                    1.9913163527955457e-12
-                ],
-                "i_angle": [
-                    2.214388654197379,
-                    -2.5535900500422257,
-                    -2.539305307454829
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2873,30 +3087,46 @@
                 "i_angle": [
                     -0.8659571842120841,
                     -1.0690757567303182,
                     -1.0695052376503775
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    375.1545796196698,
+                    0.02852748331547031,
+                    375.18020097053176
+                ],
+                "i_from_angle": [
+                    -1.0688919646176038,
+                    -0.6135741734015381,
+                    2.072734125962205
+                ],
+                "i_to": [
+                    6498.089812433243,
+                    3248.712079192715,
+                    3249.377741413738
+                ],
+                "i_to_angle": [
+                    2.072717408038076,
+                    -1.0689254061750835,
+                    -1.0688250952041753
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    142887.18546987922,
-                    2.366580246719119e-11,
-                    2.4041979785572788e-11
-                ],
-                "i_angle": [
-                    2.0889041942220152,
-                    -2.5535900500422257,
-                    -2.5305172221520817
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3065,30 +3295,46 @@
                 "i_angle": [
                     -1.167222703343486,
                     2.6530822968485546,
                     2.653081466641693
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2503.3136633204977,
+                    0.028527483314684854,
+                    2503.337512410011
+                ],
+                "i_from_angle": [
+                    -1.1944137234377359,
+                    -0.6135741733857517,
+                    1.9471851833127325
+                ],
+                "i_to": [
+                    43358.87106048655,
+                    21679.125722436325,
+                    21679.745339957582
+                ],
+                "i_to_angle": [
+                    1.9471820567472886,
+                    -1.1944199767175603,
+                    -1.194401217235531
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.7482104232866735,
-                    4.344673780753835e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.0944723059407107,
-                    -0.39735401778895213,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3257,30 +3503,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795090337872924,
+                    0.12770399637305999,
+                    0.33795761603056784
+                ],
+                "i_from_angle": [
+                    1.2372183481046142,
+                    -0.5236056997448749,
+                    -2.2845329824518905
+                ],
+                "i_to": [
+                    5.748112837912838,
+                    3.3183907696533317,
+                    3.318544584047291
+                ],
+                "i_to_angle": [
+                    -2.0944555547717583,
+                    1.5706412946214492,
+                    0.5236596571226464
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    17090.403201116897,
-                    2.051160198809135e-12,
-                    1.5654800793643497e-12
-                ],
-                "i_angle": [
-                    1.9553211642884165,
-                    -2.214297435588181,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3449,30 +3711,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    657.7623765890656,
+                    0.12770399637314112,
+                    657.8630622977595
+                ],
+                "i_from_angle": [
+                    -1.1862086638218121,
+                    -0.5236056997447096,
+                    1.955503406424493
+                ],
+                "i_to": [
+                    11393.650499100764,
+                    5695.517395239622,
+                    5698.13328664812
+                ],
+                "i_to_angle": [
+                    1.9554437026657558,
+                    -1.1863281170411664,
+                    -1.1859698670582517
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109429.52799393355,
-                    1.9759391624171684e-11,
-                    1.640928159047308e-11
-                ],
-                "i_angle": [
-                    1.302974132893974,
-                    -3.058451421701352,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3641,30 +3919,46 @@
                 "i_angle": [
                     -1.8400800604182057,
                     -1.819576712276655,
                     -1.820208641738679
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8507831403224,
+                    0.02852748331513395,
+                    456.8609540097659
+                ],
+                "i_from_angle": [
+                    -1.8198497781443317,
+                    -0.6135741733981159,
+                    1.3218012150281153
+                ],
+                "i_to": [
+                    7912.975757713378,
+                    3956.3557705365633,
+                    3956.6200174751652
+                ],
+                "i_to_angle": [
+                    1.3217720455614885,
+                    -1.819908120324474,
+                    -1.819733101576735
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109000.79805496582,
-                    1.3531440247604774e-11,
-                    1.3531440247604774e-11
-                ],
-                "i_angle": [
-                    1.321342086586508,
-                    -2.896613990462929,
-                    -2.896613990462929
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3833,30 +4127,46 @@
                 "i_angle": [
                     -1.845202770771154,
                     -2.337465947871521,
                     -2.337999824103851
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    455.06071558934633,
+                    0.028527483315483534,
+                    455.07137429919163
+                ],
+                "i_from_angle": [
+                    -1.8014807248097613,
+                    -0.6135741733988664,
+                    1.3401700774087604
+                ],
+                "i_to": [
+                    7881.975103097586,
+                    3940.8491058380027,
+                    3941.126027241994
+                ],
+                "i_to_angle": [
+                    1.3401410034348904,
+                    -1.8015388761623425,
+                    -1.8013644302763592
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.7485209162401265,
-                    8.449575060241685e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.094563745950491,
-                    -0.3231049223228771,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4025,30 +4335,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379596005369549,
+                    0.12770399637324598,
+                    0.337974062036374
+                ],
+                "i_from_angle": [
+                    1.2371516047793492,
+                    -0.523605699744634,
+                    -2.2845854100966676
+                ],
+                "i_to": [
+                    5.748334578718067,
+                    3.318398009128972,
+                    3.3187293841463785
+                ],
+                "i_to_angle": [
+                    -2.0945173457092254,
+                    1.5705782413910658,
+                    0.5236300090573025
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12209.990635538234,
-                    1.740467143053464e-12,
-                    1.4791126541994494e-12
-                ],
-                "i_angle": [
-                    2.0351758962812303,
-                    -2.356194490192345,
-                    -2.158798930342464
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4217,30 +4543,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    469.9009910110001,
+                    0.1277039963732222,
+                    470.0076264988873
+                ],
+                "i_from_angle": [
+                    -1.1063062766241116,
+                    -0.5236056997440959,
+                    2.035435891701585
+                ],
+                "i_to": [
+                    8139.847377249304,
+                    4068.5385553882616,
+                    4071.309026569986
+                ],
+                "i_to_angle": [
+                    2.0353611428150837,
+                    -1.1064558592313762,
+                    -1.1060073149841618
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    32886.210755032254,
-                    3.6692269098233675e-12,
-                    4.10232039761827e-12
-                ],
-                "i_angle": [
-                    1.9877468368006401,
-                    -2.677945044588987,
-                    -2.498091544796509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4409,30 +4751,46 @@
                 "i_angle": [
                     -1.155279594676233,
                     -1.1350945970664827,
                     -1.1363864355210234
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    137.27899008719672,
+                    0.028527483315236944,
+                    137.30372779337205
+                ],
+                "i_from_angle": [
+                    -1.1349641329410305,
+                    -0.6135741734040746,
+                    2.006732007547474
+                ],
+                "i_to": [
+                    2377.95608806413,
+                    1188.656706130901,
+                    1189.299410583394
+                ],
+                "i_to_angle": [
+                    2.0066802687597893,
+                    -1.1350676571420824,
+                    -1.1347571964280048
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    32742.559189895983,
-                    4.10232039761827e-12,
-                    3.6692269098233675e-12
-                ],
-                "i_angle": [
-                    1.9913080968758046,
-                    -2.214297435588181,
-                    -2.0344439357957027
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4601,30 +4959,46 @@
                 "i_angle": [
                     -1.1752093973334015,
                     -1.6673038083902076,
                     -1.6690009797019687
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    136.67927963903668,
+                    0.028527483315338827,
+                    136.70406780028856
+                ],
+                "i_from_angle": [
+                    -1.1314017730383141,
+                    -0.6135741734033183,
+                    2.0102941761243986
+                ],
+                "i_to": [
+                    2367.569235383094,
+                    1183.4626242444488,
+                    1184.106639558292
+                ],
+                "i_to_angle": [
+                    2.010242533020936,
+                    -1.1315051060843078,
+                    -1.1311952193473738
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.009258394948637e-16,
-                    5.74747402954125,
-                    8.041086459980025e-16
-                ],
-                "i_angle": [
-                    -2.0943951023931957,
-                    2.0942909619616663,
-                    -2.1789706984650983
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4793,30 +5167,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33792381024706725,
+                    0.33791566956759234,
+                    0.12770399637309612
+                ],
+                "i_from_angle": [
+                    1.9042265871171715,
+                    -0.8571680804456813,
+                    -2.6180008021387313
+                ],
+                "i_to": [
+                    3.3182972821545613,
+                    5.74750397032484,
+                    3.3181107500243407
+                ],
+                "i_to_angle": [
+                    -1.5707898490626022,
+                    2.0943232623466734,
+                    -0.5237164824553814
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.6412457148092364e-12,
-                    61463.949515399676,
-                    4.011906280418247e-12
-                ],
-                "i_angle": [
-                    0.261799387799149,
-                    -1.0439874339236515,
-                    0.43437734903135605
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4985,30 +5375,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2365.820072653962,
+                    2365.8196618256507,
+                    0.12770399637303706
+                ],
+                "i_from_angle": [
+                    -1.043960444895325,
+                    2.0975782302249617,
+                    -2.6180008021339245
+                ],
+                "i_to": [
+                    20488.606454589426,
+                    40977.20210122772,
+                    20488.595780956835
+                ],
+                "i_to_angle": [
+                    2.097686187145071,
+                    -1.0439874341277346,
+                    2.0975242517368655
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.0511601988091346e-12,
-                    22402.312747881482,
-                    1.8346134549116837e-12
-                ],
-                "i_angle": [
-                    1.6906986599898817,
-                    0.1385810245234842,
-                    2.154346268990688
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5177,30 +5583,46 @@
                 "i_angle": [
                     3.137894211491035,
                     -2.9417682769822924,
                     3.1382928209778966
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    392.4840416381267,
+                    392.4581915819866,
+                    0.02852748331519694
+                ],
+                "i_from_angle": [
+                    -0.0030769528600590504,
+                    3.1384849566916855,
+                    -2.707969275794447
+                ],
+                "i_to": [
+                    3399.235377651444,
+                    6797.799143915922,
+                    3398.563773492887
+                ],
+                "i_to_angle": [
+                    3.1385464407182493,
+                    -0.0030923243728455227,
+                    3.138454208603362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.5047681269829595e-11,
-                    205032.2584419135,
-                    2.80401926733944e-11
-                ],
-                "i_angle": [
-                    2.066338895462947,
-                    0.11051289384429731,
-                    2.2592232077209218
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5369,30 +5791,46 @@
                 "i_angle": [
                     0.6746787146159781,
                     3.137566074025622,
                     0.6746865073003591
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    3592.103211566729,
+                    3592.077710973006,
+                    0.028527483314505962
+                ],
+                "i_from_angle": [
+                    -0.031209566161388202,
+                    3.1103795273400214,
+                    -2.7079692757833635
+                ],
+                "i_to": [
+                    31108.747184338587,
+                    62216.831842930784,
+                    31108.08465947932
+                ],
+                "i_to_angle": [
+                    3.1103866474662425,
+                    -0.031211346199261577,
+                    3.1103759672010898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.258935698000959e-16,
-                    5.748158405083368,
-                    8.18684547740158e-16
-                ],
-                "i_angle": [
-                    -2.33937376552006,
-                    2.094326949481581,
-                    -2.3012329646204015
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5561,30 +5999,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795527136631337,
+                    0.33794931548506224,
+                    0.12770399637317842
+                ],
+                "i_from_angle": [
+                    1.9042619220954338,
+                    -0.8571698155444356,
+                    -2.61800080213835
+                ],
+                "i_to": [
+                    3.3185208952668352,
+                    5.748078156256009,
+                    3.3183844217710248
+                ],
+                "i_to_angle": [
+                    -1.5707335309769386,
+                    2.0943406846666313,
+                    -0.5237466687450739
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.4699239530214605e-12,
-                    17760.97652647428,
-                    2.0511601988091346e-12
-                ],
-                "i_angle": [
-                    1.8913515373097682,
-                    -0.13423239468916315,
-                    1.9744927691982097
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5753,30 +6207,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    683.67683275646,
+                    683.5757682608864,
+                    0.12770399637281485
+                ],
+                "i_from_angle": [
+                    -0.13405728800142205,
+                    3.007421171825307,
+                    -2.6180008021369074
+                ],
+                "i_to": [
+                    5921.690372851554,
+                    11840.754839412968,
+                    5919.064640268169
+                ],
+                "i_to_angle": [
+                    3.0076495255935614,
+                    -0.13411438066247025,
+                    3.0073069442923734
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3127425272378461e-11,
-                    136915.9623074532,
-                    1.3356187556109646e-11
-                ],
-                "i_angle": [
-                    1.0471975511965974,
-                    -0.9460649004054179,
-                    0.8618496012009026
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5945,30 +6415,46 @@
                 "i_angle": [
                     2.214026410751588,
                     2.194063754884357,
                     2.2145452217393484
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    571.6163028687619,
+                    571.6103589428898,
+                    0.02852748331542307
+                ],
+                "i_from_angle": [
+                    -0.9272528561919476,
+                    2.214290985763693,
+                    -2.7079692757923826
+                ],
+                "i_to": [
+                    4950.393882719229,
+                    9900.633311177093,
+                    4950.239454995498
+                ],
+                "i_to_angle": [
+                    2.214388608016761,
+                    -0.9272772618821318,
+                    2.214242173114504
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3127425272378461e-11,
-                    136727.84188424365,
-                    1.3356187556109646e-11
-                ],
-                "i_angle": [
-                    1.0471975511965974,
-                    -0.9225743013190341,
-                    0.8618496012009026
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6137,30 +6623,46 @@
                 "i_angle": [
                     1.7013436398465804,
                     2.194063754884357,
                     1.701747030706488
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    570.8313362052144,
+                    570.8247385314771,
+                    0.028527483315286383
+                ],
+                "i_from_angle": [
+                    -0.9037613484083556,
+                    2.2377826844742335,
+                    -2.707969275792239
+                ],
+                "i_to": [
+                    4943.601533516075,
+                    9887.031628146426,
+                    4943.430120924612
+                ],
+                "i_to_angle": [
+                    2.237879924764622,
+                    -0.9037856586214673,
+                    2.237734062643201
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.334314525508457e-16,
-                    5.748468897310852,
-                    4.344673780753835e-16
-                ],
-                "i_angle": [
-                    -2.4161456567898383,
-                    2.0942355107422137,
-                    -2.4917491201821482
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6329,30 +6831,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33797171732586107,
+                    0.3379580127439293,
+                    0.1277039963731637
+                ],
+                "i_from_angle": [
+                    1.904209495634884,
+                    -0.857236557753224,
+                    -2.618000802138229
+                ],
+                "i_to": [
+                    3.318705693775631,
+                    5.748299897509253,
+                    3.3183916633941286
+                ],
+                "i_to_angle": [
+                    -1.5707631778470679,
+                    2.0942788948790625,
+                    -0.5238097209912791
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.1603114287023091e-12,
-                    12543.843934648457,
-                    1.1603114287023091e-12
-                ],
-                "i_angle": [
-                    1.8325957145940457,
-                    -0.05359950015200677,
-                    1.8325957145940457
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6521,30 +7039,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    482.8597950450049,
+                    482.7527666890548,
+                    0.12770399637316113
+                ],
+                "i_from_angle": [
+                    -0.053346640193896414,
+                    3.088101721130272,
+                    -2.6180008021373204
+                ],
+                "i_to": [
+                    4182.615469528245,
+                    8362.450064987112,
+                    4179.834791330795
+                ],
+                "i_to_angle": [
+                    3.08839024170645,
+                    -0.05341877833004185,
+                    3.08795736487304
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    3.1309601587286993e-12,
-                    35448.479883073465,
-                    4.102320397618269e-12
-                ],
-                "i_angle": [
-                    2.066338895462947,
-                    -0.09444990294134478,
-                    1.9744927691982097
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6713,30 +7247,46 @@
                 "i_angle": [
                     3.0646909877442248,
                     3.045706514093044,
                     3.0658696280746502
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    148.00184016008106,
+                    147.97693112895487,
+                    0.028527483315241034
+                ],
+                "i_from_angle": [
+                    -0.07547976976386275,
+                    3.06601892233164,
+                    -2.7079692757924794
+                ],
+                "i_to": [
+                    1281.9492637044427,
+                    2563.2513463433015,
+                    1281.3021080979902
+                ],
+                "i_to_angle": [
+                    3.066206813696867,
+                    -0.0755267465571947,
+                    3.065924929199682
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.7884816986623306e-12,
-                    35279.978347555196,
-                    4.102320397618269e-12
-                ],
-                "i_angle": [
-                    1.8628894745128206,
-                    -0.09067027255459044,
-                    1.9744927691982097
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6905,30 +7455,46 @@
                 "i_angle": [
                     2.5322804854228216,
                     3.0259951467042177,
                     2.533847244831745
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    147.29843493448595,
+                    147.27347351062767,
+                    0.028527483315350786
+                ],
+                "i_from_angle": [
+                    -0.0716992308662456,
+                    3.069799652528063,
+                    -2.7079692757921148
+                ],
+                "i_to": [
+                    1275.8580493940253,
+                    2551.0675567434296,
+                    1275.2095325844537
+                ],
+                "i_to_angle": [
+                    3.0699871611427025,
+                    -0.0717461119910411,
+                    3.0697058505417387
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.012344526598182e-16,
-                    5.747526034574177,
-                    8.041086459980025e-16
-                ],
-                "i_angle": [
-                    -2.0943951023931957,
-                    2.0942819117101643,
-                    -2.1789706984650983
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7097,30 +7663,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379261542951378,
+                    0.3379172569106448,
+                    0.12770399637327606
+                ],
+                "i_from_angle": [
+                    1.9042218877833699,
+                    -0.8571750185743795,
+                    -2.618000802138491
+                ],
+                "i_to": [
+                    3.3183209651975596,
+                    5.747538641836821,
+                    3.318117093981725
+                ],
+                "i_to_angle": [
+                    -1.5707917631428587,
+                    2.094317228199085,
+                    -0.5237236205664709
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.5637126361892306e-12,
-                    55809.55246338668,
-                    6.678093778054823e-12
-                ],
-                "i_angle": [
-                    1.0471975511965974,
-                    -0.9562870978392181,
-                    0.8618496012009026
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7289,30 +7871,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2148.1715393760155,
+                    2148.1599442770134,
+                    0.12770399637298238
+                ],
+                "i_from_angle": [
+                    -0.9562529730330952,
+                    2.1852804781840613,
+                    -2.618000802133183
+                ],
+                "i_to": [
+                    18603.811729570327,
+                    37207.32206292301,
+                    18603.51048006251
+                ],
+                "i_to_angle": [
+                    2.185398882290022,
+                    -0.9562825741395247,
+                    2.1852212751725166
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.9913163527955453e-12,
-                    21414.66328546044,
-                    1.4791126541994492e-12
-                ],
-                "i_angle": [
-                    1.6494848973315615,
-                    0.11999355180418311,
-                    1.6352001547441648
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7481,30 +8079,46 @@
                 "i_angle": [
                     3.119284967136013,
                     -2.96035228660528,
                     3.1197144480560723
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    375.18020097053176,
+                    375.1545796196699,
+                    0.02852748331547031
+                ],
+                "i_from_angle": [
+                    -0.021660976430990703,
+                    3.1198982401687867,
+                    -2.707969275794734
+                ],
+                "i_to": [
+                    3249.3777414137376,
+                    6498.0898124332425,
+                    3248.712079192715
+                ],
+                "i_to_angle": [
+                    3.1199651095822154,
+                    -0.02167769435511999,
+                    3.119864798611307
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.4041979785572788e-11,
-                    142887.18546987922,
-                    2.3665802467191187e-11
-                ],
-                "i_angle": [
-                    1.6582729826343088,
-                    -0.005490908171180816,
-                    1.6352001547441648
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7673,30 +8287,46 @@
                 "i_angle": [
                     0.5586863642484972,
                     3.0215675014429046,
                     0.5586871944553587
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2503.3375124100107,
+                    2503.313663320497,
+                    0.02852748331468485
+                ],
+                "i_from_angle": [
+                    -0.14720991908046335,
+                    2.9943764813486546,
+                    -2.7079692757789475
+                ],
+                "i_to": [
+                    21679.745339957582,
+                    43358.871060486556,
+                    21679.125722436325
+                ],
+                "i_to_angle": [
+                    2.9943889875508596,
+                    -0.14721304564590737,
+                    2.9943702280688305
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.334314525508457e-16,
-                    5.7482104232866735,
-                    4.344673780753835e-16
-                ],
-                "i_angle": [
-                    -2.4161456567898383,
-                    2.09431789884568,
-                    -2.4917491201821482
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7865,30 +8495,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795761603056784,
+                    0.3379509033787293,
+                    0.12770399637305999
+                ],
+                "i_from_angle": [
+                    1.9042572223345,
+                    -0.8571767542885818,
+                    -2.618000802138071
+                ],
+                "i_to": [
+                    3.3185445840472907,
+                    5.748112837912838,
+                    3.3183907696533312
+                ],
+                "i_to_angle": [
+                    -1.5707354452705495,
+                    2.0943346500146323,
+                    -0.5237538077717467
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.5654800793643497e-12,
-                    17090.403201116897,
-                    2.0511601988091346e-12
-                ],
-                "i_angle": [
-                    2.066338895462947,
-                    -0.13907393810477936,
-                    1.9744927691982097
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8057,30 +8703,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    657.8630622977593,
+                    657.7623765890658,
+                    0.1277039963731411
+                ],
+                "i_from_angle": [
+                    -0.13889169596870307,
+                    3.002581540964578,
+                    -2.6180008021379053
+                ],
+                "i_to": [
+                    5698.13328664812,
+                    11393.650499100762,
+                    5695.517395239621
+                ],
+                "i_to_angle": [
+                    3.002820337728139,
+                    -0.13895139972744014,
+                    3.0024620877452244
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.640928159047308e-11,
-                    109429.52799393355,
-                    1.9759391624171687e-11
-                ],
-                "i_angle": [
-                    1.0471975511965974,
-                    -0.791420969499222,
-                    1.1303387830850384
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8249,30 +8911,46 @@
                 "i_angle": [
                     2.368581563047712,
                     2.348710144368185,
                     2.3692134925097355
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8609540097659,
+                    456.85078314032233,
+                    0.028527483315133953
+                ],
+                "i_from_angle": [
+                    -0.7725938873650807,
+                    2.368940426642059,
+                    -2.707969275791312
+                ],
+                "i_to": [
+                    3956.6200174751652,
+                    7912.975757713378,
+                    3956.3557705365633
+                ],
+                "i_to_angle": [
+                    2.3690571032096552,
+                    -0.7726230568317075,
+                    2.3688820844619167
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3531440247604774e-11,
-                    109000.79805496581,
-                    1.3531440247604774e-11
-                ],
-                "i_angle": [
-                    1.2921762143234614,
-                    -0.773053015806688,
-                    1.2921762143234614
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8441,30 +9119,46 @@
                 "i_angle": [
                     1.8507903806825396,
                     2.3435874340152365,
                     1.8513242569148693
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    455.07137429919163,
+                    455.06071558934633,
+                    0.028527483315483534
+                ],
+                "i_from_angle": [
+                    -0.7542250249844356,
+                    2.3873094799766292,
+                    -2.7079692757920624
+                ],
+                "i_to": [
+                    3941.126027241994,
+                    7881.975103097584,
+                    3940.8491058380027
+                ],
+                "i_to_angle": [
+                    2.3874257745100316,
+                    -0.7542540989583055,
+                    2.387251328624048
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.334314525508457e-16,
-                    5.7485209162401265,
-                    8.449575060241683e-16
-                ],
-                "i_angle": [
-                    -2.4161456567898383,
-                    2.0942264588358994,
-                    -2.417500024716073
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8633,30 +9327,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379740620363739,
+                    0.33795960053695484,
+                    0.12770399637324595
+                ],
+                "i_from_angle": [
+                    1.9042047946897231,
+                    -0.8572434976138468,
+                    -2.61800080213783
+                ],
+                "i_to": [
+                    3.318729384146379,
+                    5.748334578718068,
+                    3.3183980091289715
+                ],
+                "i_to_angle": [
+                    -1.5707650933358934,
+                    2.094272859077165,
+                    -0.5238168610021301
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.4791126541994492e-12,
-                    12209.990635538235,
-                    1.7404671430534636e-12
-                ],
-                "i_angle": [
-                    2.0299912744439266,
-                    -0.05921920611196566,
-                    1.8325957145940457
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8825,30 +9535,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    470.00762649888736,
+                    469.900991011,
+                    0.1277039963732222
+                ],
+                "i_from_angle": [
+                    -0.05895921069161068,
+                    3.082483928162279,
+                    -2.618000802137292
+                ],
+                "i_to": [
+                    4071.309026569986,
+                    8139.847377249303,
+                    4068.5385553882616
+                ],
+                "i_to_angle": [
+                    3.0827828898022287,
+                    -0.05903395957811235,
+                    3.0823343455550143
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.102320397618269e-12,
-                    32886.21075503225,
-                    3.6692269098233675e-12
-                ],
-                "i_angle": [
-                    1.6906986599898817,
-                    -0.10664826559255575,
-                    1.5108451601974033
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9017,30 +9743,46 @@
                 "i_angle": [
                     3.0524037692653674,
                     3.033510610110157,
                     3.0536956077199076
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    137.30372779337208,
+                    137.2789900871967,
+                    0.02852748331523694
+                ],
+                "i_from_angle": [
+                    -0.08766309484572168,
+                    3.05382607184536,
+                    -2.7079692757972706
+                ],
+                "i_to": [
+                    1189.299410583394,
+                    2377.95608806413,
+                    1188.656706130901
+                ],
+                "i_to_angle": [
+                    3.054033008358386,
+                    -0.08771483363340662,
+                    3.053722547644308
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    3.6692269098233675e-12,
-                    32742.559189895976,
-                    4.102320397618269e-12
-                ],
-                "i_angle": [
-                    2.154346268990688,
-                    -0.1030870055173914,
-                    1.9744927691982097
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9209,30 +9951,46 @@
                 "i_angle": [
                     2.519789225084422,
                     3.013580807452989,
                     2.521486396396183
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    136.70406780028856,
+                    136.67927963903665,
+                    0.028527483315338824
+                ],
+                "i_from_angle": [
+                    -0.08410092626879707,
+                    3.0573884317480764,
+                    -2.7079692757965144
+                ],
+                "i_to": [
+                    1184.106639558292,
+                    2367.569235383094,
+                    1183.4626242444488
+                ],
+                "i_to_angle": [
+                    3.057594985439017,
+                    -0.08415256937225953,
+                    3.0572850987020828
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.041086459980025e-16,
-                    6.009258394948638e-16,
-                    5.74747402954125
-                ],
-                "i_angle": [
-                    2.009819506321293,
-                    2.0943951023931953,
-                    -0.00010414043152882815
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9401,30 +10159,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.1277039963730961,
+                    0.33792381024706725,
+                    0.3379156695675923
+                ],
+                "i_from_angle": [
+                    1.5707894026476599,
+                    -0.1901685152760237,
+                    -2.9515631828388766
+                ],
+                "i_to": [
+                    3.3181107500243407,
+                    3.3182972821545613,
+                    5.747503970324839
+                ],
+                "i_to_angle": [
+                    -2.6181115848485765,
+                    2.618000355723789,
+                    -7.184004652187174e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.011906280418248e-12,
-                    4.641245714809236e-12,
-                    61463.94951539966
-                ],
-                "i_angle": [
-                    -1.6600177533618392,
-                    -1.8325957145940464,
-                    -3.138382536316847
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9593,30 +10367,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637303703,
+                    2365.820072653962,
+                    2365.819661825651
+                ],
+                "i_from_angle": [
+                    1.5707894026524665,
+                    -3.13835554728852,
+                    0.0031831278317665484
+                ],
+                "i_to": [
+                    20488.59578095684,
+                    20488.606454589422,
+                    40977.20210122772
+                ],
+                "i_to_angle": [
+                    0.0031291493436701547,
+                    0.0032910847518754774,
+                    -3.13838253652093
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8346134549116837e-12,
-                    2.0511601988091346e-12,
-                    22402.31274788148
-                ],
-                "i_angle": [
-                    0.059951166597492535,
-                    -0.4036964424033136,
-                    -1.955814077869711
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9785,30 +10575,46 @@
                 "i_angle": [
                     1.0438977185847016,
                     1.0434991090978396,
                     1.2470219278040988
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331519694,
+                    392.4840416381267,
+                    392.4581915819866
+                ],
+                "i_from_angle": [
+                    1.480820928991944,
+                    -2.0974720552532546,
+                    1.0440898542984904
+                ],
+                "i_to": [
+                    3398.5637734928873,
+                    3399.2353776514447,
+                    6797.799143915923
+                ],
+                "i_to_angle": [
+                    1.0440591062101667,
+                    1.0441513383250542,
+                    -2.097487426766041
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.80401926733944e-11,
-                    2.5047681269829595e-11,
-                    205032.25844191352
-                ],
-                "i_angle": [
-                    0.16482810532772646,
-                    -0.02805620693024822,
-                    -1.983882208548898
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9977,30 +10783,46 @@
                 "i_angle": [
                     -1.4197085950928363,
                     -1.4197163877772172,
                     1.043170971632427
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483314505962,
+                    3592.103211566729,
+                    3592.077710973006
+                ],
+                "i_from_angle": [
+                    1.4808209290030276,
+                    -2.1256046685545833,
+                    1.0159844249468262
+                ],
+                "i_to": [
+                    31108.08465947932,
+                    31108.747184338594,
+                    62216.831842930784
+                ],
+                "i_to_angle": [
+                    1.0159808648078947,
+                    1.015991545073047,
+                    -2.125606448592457
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.18684547740158e-16,
-                    8.258935698000961e-16,
-                    5.748158405083367
-                ],
-                "i_angle": [
-                    1.8875572401659897,
-                    1.849416439266331,
-                    -6.815291161444347e-05
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10169,30 +10991,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637317842,
+                    0.33795527136631337,
+                    0.3379493154850622
+                ],
+                "i_from_angle": [
+                    1.5707894026480416,
+                    -0.19013318029776152,
+                    -2.9515649179376306
+                ],
+                "i_to": [
+                    3.3183844217710248,
+                    3.3185208952668352,
+                    5.748078156256009
+                ],
+                "i_to_angle": [
+                    -2.6181417711382693,
+                    2.6180566738094524,
+                    -5.441772656421252e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.051160198809135e-12,
-                    2.4699239530214605e-12,
-                    17760.976526474282
-                ],
-                "i_angle": [
-                    -0.11990233319498574,
-                    -0.20304356508342694,
-                    -2.2286274970823583
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10361,30 +11199,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637281488,
+                    683.67683275646,
+                    683.5757682608864
+                ],
+                "i_from_angle": [
+                    1.5707894026494837,
+                    -2.2284523903946174,
+                    0.9130260694321118
+                ],
+                "i_to": [
+                    5919.064640268168,
+                    5921.690372851553,
+                    11840.754839412968
+                ],
+                "i_to_angle": [
+                    0.912911841899178,
+                    0.9132544232003658,
+                    -2.2285094830556655
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11,
-                    136915.9623074532
-                ],
-                "i_angle": [
-                    -1.2325455011922928,
-                    -1.047197551196598,
-                    -3.0404600027986133
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10553,30 +11407,46 @@
                 "i_angle": [
                     0.12015011934615327,
                     0.11963130835839286,
                     0.099668652491162
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483315423065,
+                    571.6163028687619,
+                    571.6103589428899
+                ],
+                "i_from_angle": [
+                    1.4808209289940086,
+                    -3.021647958585143,
+                    0.1198958833704977
+                ],
+                "i_to": [
+                    4950.239454995498,
+                    4950.393882719229,
+                    9900.633311177093
+                ],
+                "i_to_angle": [
+                    0.11984707072130907,
+                    0.11999350562356585,
+                    -3.021672364275327
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11,
-                    136727.84188424365
-                ],
-                "i_angle": [
-                    -1.2325455011922928,
-                    -1.047197551196598,
-                    -3.0169694037122294
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10745,30 +11615,46 @@
                 "i_angle": [
                     -0.39264807168670746,
                     -0.3930514625466148,
                     0.09966865249116189
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331528638,
+                    570.8313362052144,
+                    570.8247385314771
+                ],
+                "i_from_angle": [
+                    1.480820928994152,
+                    -2.998156450801551,
+                    0.143387582081038
+                ],
+                "i_to": [
+                    4943.430120924612,
+                    4943.601533516075,
+                    9887.031628146426
+                ],
+                "i_to_angle": [
+                    0.14333896025000586,
+                    0.14348482237142682,
+                    -2.9981807610146625
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.3446737807538343e-16,
-                    6.334314525508456e-16,
-                    5.748468897310853
-                ],
-                "i_angle": [
-                    1.6970410846042432,
-                    1.7726445479965531,
-                    -0.0001595916509816671
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10937,30 +11823,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.1277039963731637,
+                    0.3379717173258611,
+                    0.3379580127439292
+                ],
+                "i_from_angle": [
+                    1.5707894026481621,
+                    -0.19018560675831128,
+                    -2.951631660146419
+                ],
+                "i_to": [
+                    3.3183916633941286,
+                    3.3187056937756316,
+                    5.748299897509252
+                ],
+                "i_to_angle": [
+                    -2.6182048233844744,
+                    2.6180270269393233,
+                    -0.00011620751413300206
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.160311428702309e-12,
-                    1.160311428702309e-12,
-                    12543.843934648457
-                ],
-                "i_angle": [
-                    -0.2617993877991497,
-                    -0.2617993877991497,
-                    -2.147994602545202
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11129,30 +12031,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637316113,
+                    482.859795045005,
+                    482.7527666890548
+                ],
+                "i_from_angle": [
+                    1.5707894026490707,
+                    -2.1477417425870917,
+                    0.9937066187370767
+                ],
+                "i_to": [
+                    4179.834791330796,
+                    4182.615469528245,
+                    8362.45006498711
+                ],
+                "i_to_angle": [
+                    0.9935622624798447,
+                    0.9939951393132546,
+                    -2.147813880723237
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.10232039761827e-12,
-                    3.1309601587286993e-12,
-                    35448.479883073465
-                ],
-                "i_angle": [
-                    -0.11990233319498574,
-                    -0.02805620693024822,
-                    -2.18884500533454
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11321,30 +12239,46 @@
                 "i_angle": [
                     0.9714745256814549,
                     0.9702958853510296,
                     0.9513114116998486
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483315241034,
+                    148.00184016008106,
+                    147.9769311289549
+                ],
+                "i_from_angle": [
+                    1.4808209289939118,
+                    -2.169874872157058,
+                    0.9716238199384446
+                ],
+                "i_to": [
+                    1281.30210809799,
+                    1281.9492637044427,
+                    2563.2513463433015
+                ],
+                "i_to_angle": [
+                    0.9715298268064865,
+                    0.9718117113036716,
+                    -2.16992184895039
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.10232039761827e-12,
-                    4.7884816986623306e-12,
-                    35279.97834755519
-                ],
-                "i_angle": [
-                    -0.11990233319498574,
-                    -0.23150562788037454,
-                    -2.185065374947786
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11513,30 +12447,46 @@
                 "i_angle": [
                     0.4394521424385496,
                     0.43788538302962643,
                     0.9316000443110222
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331535079,
+                    147.29843493448595,
+                    147.27347351062767
+                ],
+                "i_from_angle": [
+                    1.4808209289942762,
+                    -2.166094333259441,
+                    0.9754045501348673
+                ],
+                "i_to": [
+                    1275.2095325844537,
+                    1275.858049394025,
+                    2551.06755674343
+                ],
+                "i_to_angle": [
+                    0.9753107481485433,
+                    0.9755920587495075,
+                    -2.1661412143842362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.041086459980025e-16,
-                    8.012344526598184e-16,
-                    5.747526034574177
-                ],
-                "i_angle": [
-                    2.009819506321293,
-                    2.0943951023931953,
-                    -0.00011319068303125518
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11705,30 +12655,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637327606,
+                    0.3379261542951378,
+                    0.3379172569106448
+                ],
+                "i_from_angle": [
+                    1.5707894026479001,
+                    -0.19017321460982542,
+                    -2.951570120967575
+                ],
+                "i_to": [
+                    3.3181170939817255,
+                    3.318320965197559,
+                    5.74753864183682
+                ],
+                "i_to_angle": [
+                    -2.6181187229596663,
+                    2.6179984416435325,
+                    -7.787419411035895e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.678093778054823e-12,
-                    6.563712636189232e-12,
-                    55809.55246338669
-                ],
-                "i_angle": [
-                    -1.2325455011922928,
-                    -1.047197551196598,
-                    -3.0506822002324134
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11897,30 +12863,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637298235,
+                    2148.1715393760155,
+                    2148.159944277013
+                ],
+                "i_from_angle": [
+                    1.5707894026532083,
+                    -3.0506480754262904,
+                    0.09088537579086624
+                ],
+                "i_to": [
+                    18603.51048006251,
+                    18603.811729570327,
+                    37207.322062923005
+                ],
+                "i_to_angle": [
+                    0.09082617277932142,
+                    0.09100377989682672,
+                    -3.05067767653272
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.4791126541994492e-12,
-                    1.9913163527955457e-12,
-                    21414.66328546044
-                ],
-                "i_angle": [
-                    -0.4591949476490304,
-                    -0.44491020506163376,
-                    -1.9744015505890122
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12089,30 +13071,46 @@
                 "i_angle": [
                     1.025319345662877,
                     1.024889864742818,
                     1.2284379181811111
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483315470305,
+                    375.18020097053176,
+                    375.15457961966985
+                ],
+                "i_from_angle": [
+                    1.4808209289916572,
+                    -2.116056078824186,
+                    1.0255031377755914
+                ],
+                "i_to": [
+                    3248.712079192715,
+                    3249.3777414137376,
+                    6498.089812433243
+                ],
+                "i_to_angle": [
+                    1.0254696962181118,
+                    1.02557000718902,
+                    -2.1160727967483153
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.3665802467191187e-11,
-                    2.4041979785572785e-11,
-                    142887.18546987922
-                ],
-                "i_angle": [
-                    -0.4591949476490304,
-                    -0.4361221197588865,
-                    -2.099886010564376
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12281,30 +13279,46 @@
                 "i_angle": [
                     -1.5357079079378364,
                     -1.535708738144698,
                     0.9271723990497093
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331468485,
+                    2503.3375124100116,
+                    2503.3136633204977
+                ],
+                "i_from_angle": [
+                    1.4808209290074437,
+                    -2.2416050214736587,
+                    0.8999813789554594
+                ],
+                "i_to": [
+                    21679.125722436325,
+                    21679.745339957582,
+                    43358.871060486556
+                ],
+                "i_to_angle": [
+                    0.899975125675635,
+                    0.8999938851576642,
+                    -2.2416081480391026
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.3446737807538343e-16,
-                    6.334314525508456e-16,
-                    5.7482104232866735
-                ],
-                "i_angle": [
-                    1.6970410846042432,
-                    1.7726445479965531,
-                    -7.72035475155191e-05
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12473,30 +13487,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637305999,
+                    0.33795761603056784,
+                    0.3379509033787293
+                ],
+                "i_from_angle": [
+                    1.5707894026483202,
+                    -0.19013788005869525,
+                    -2.951571856681777
+                ],
+                "i_to": [
+                    3.3183907696533317,
+                    3.3185445840472907,
+                    5.748112837912838
+                ],
+                "i_to_angle": [
+                    -2.618148910164942,
+                    2.6180547595158417,
+                    -6.0452378563216876e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.051160198809135e-12,
-                    1.5654800793643497e-12,
-                    17090.403201116897
-                ],
-                "i_angle": [
-                    -0.11990233319498574,
-                    -0.02805620693024822,
-                    -2.2334690404979747
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12665,30 +13695,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.1277039963731411,
+                    657.8630622977595,
+                    657.7623765890658
+                ],
+                "i_from_angle": [
+                    1.5707894026484857,
+                    -2.2332867983618985,
+                    0.908186438571383
+                ],
+                "i_to": [
+                    5695.517395239622,
+                    5698.13328664812,
+                    11393.650499100764
+                ],
+                "i_to_angle": [
+                    0.9080669853520289,
+                    0.9084252353349437,
+                    -2.2333465021206353
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.975939162417168e-11,
-                    1.640928159047308e-11,
-                    109429.52799393355
-                ],
-                "i_angle": [
-                    -0.9640563193081567,
-                    -1.0471975511965979,
-                    -2.8858160718924175
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12857,30 +13903,46 @@
                 "i_angle": [
                     0.27481839011654013,
                     0.27418646065451635,
                     0.25431504197498955
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331513395,
+                    456.8609540097659,
+                    456.85078314032233
+                ],
+                "i_from_angle": [
+                    1.4808209289950793,
+                    -2.866988989758276,
+                    0.2745453242488635
+                ],
+                "i_to": [
+                    3956.3557705365624,
+                    3956.620017475165,
+                    7912.975757713378
+                ],
+                "i_to_angle": [
+                    0.27448698206872135,
+                    0.27466200081646014,
+                    -2.867018159224903
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.3531440247604774e-11,
-                    1.3531440247604774e-11,
-                    109000.79805496582
-                ],
-                "i_angle": [
-                    -0.8022188880697338,
-                    -0.8022188880697338,
-                    -2.867448118199883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13049,30 +14111,46 @@
                 "i_angle": [
                     -0.24307084547832591,
                     -0.24360472171065572,
                     0.24919233162204132
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483315483538,
+                    455.07137429919163,
+                    455.06071558934633
+                ],
+                "i_from_angle": [
+                    1.4808209289943288,
+                    -2.8486201273776306,
+                    0.29291437758343397
+                ],
+                "i_to": [
+                    3940.8491058380027,
+                    3941.126027241994,
+                    7881.975103097584
+                ],
+                "i_to_angle": [
+                    0.2928562262308527,
+                    0.29303067211683603,
+                    -2.848649201351501
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    8.449575060241683e-16,
-                    6.334314525508456e-16,
-                    5.748520916240127
-                ],
-                "i_angle": [
-                    1.7712901800703182,
-                    1.7726445479965531,
-                    -0.0001686435572958002
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13241,30 +14319,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637324595,
+                    0.337974062036374,
+                    0.3379596005369549
+                ],
+                "i_from_angle": [
+                    1.5707894026485614,
+                    -0.19019030770347214,
+                    -2.9516386000070423
+                ],
+                "i_to": [
+                    3.318398009128972,
+                    3.3187293841463785,
+                    5.748334578718067
+                ],
+                "i_to_angle": [
+                    -2.6182119633953254,
+                    2.6180251114504975,
+                    -0.00012224331602998133
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.7404671430534636e-12,
-                    1.479112654199449e-12,
-                    12209.990635538234
-                ],
-                "i_angle": [
-                    -0.2617993877991497,
-                    -0.0644038279492689,
-                    -2.153614308505161
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13433,30 +14527,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.12770399637322216,
+                    470.00762649888736,
+                    469.90099101100003
+                ],
+                "i_from_angle": [
+                    1.5707894026490994,
+                    -2.153354313084806,
+                    0.9880888257690835
+                ],
+                "i_to": [
+                    4068.5385553882616,
+                    4071.309026569986,
+                    8139.847377249304
+                ],
+                "i_to_angle": [
+                    0.987939243161819,
+                    0.9883877874090334,
+                    -2.1534290619713077
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    3.6692269098233675e-12,
-                    4.102320397618269e-12,
-                    32886.210755032254
-                ],
-                "i_angle": [
-                    -0.5835499421957918,
-                    -0.4036964424033136,
-                    -2.201043367985751
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13625,30 +14735,46 @@
                 "i_angle": [
                     0.9593005053267126,
                     0.9580086668721719,
                     0.9391155077169622
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.02852748331523694,
+                    137.30372779337208,
+                    137.27899008719672
+                ],
+                "i_from_angle": [
+                    1.4808209289891205,
+                    -2.1820581972389173,
+                    0.9594309694521647
+                ],
+                "i_to": [
+                    1188.6567061309008,
+                    1189.299410583394,
+                    2377.95608806413
+                ],
+                "i_to_angle": [
+                    0.959327445251113,
+                    0.9596379059651905,
+                    -2.182109936026602
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.10232039761827e-12,
-                    3.6692269098233675e-12,
-                    32742.559189895976
-                ],
-                "i_angle": [
-                    -0.11990233319498574,
-                    0.059951166597492535,
-                    -2.1974821079105866
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13817,30 +14943,46 @@
                 "i_angle": [
                     0.4270912940029877,
                     0.42539412269122656,
                     0.9191857050597938
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.028527483315338827,
+                    136.70406780028858,
+                    136.67927963903665
+                ],
+                "i_from_angle": [
+                    1.480820928989877,
+                    -2.1784960286619923,
+                    0.9629933293548812
+                ],
+                "i_to": [
+                    1183.462624244449,
+                    1184.106639558292,
+                    2367.5692353830946
+                ],
+                "i_to_angle": [
+                    0.9628899963088875,
+                    0.9631998830458216,
+                    -2.178547671765455
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.74747402954125,
-                    8.041086459980025e-16,
-                    6.009258394948638e-16
-                ],
-                "i_angle": [
-                    -2.094499242824724,
-                    -0.08457559607190217,
-                    0.0
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14009,30 +15151,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33791566956759234,
+                    0.12770399637309612,
+                    0.3379238102470673
+                ],
+                "i_from_angle": [
+                    1.2372270219475148,
+                    -0.5236056997455355,
+                    -2.284563617669219
+                ],
+                "i_to": [
+                    5.74750397032484,
+                    3.318110750024341,
+                    3.3182972821545613
+                ],
+                "i_to_angle": [
+                    -2.094466942439717,
+                    1.5706786199378147,
+                    0.5236052533305937
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    61463.949515399676,
-                    4.011906280418248e-12,
-                    4.6412457148092364e-12
-                ],
-                "i_angle": [
-                    1.0504076684695445,
-                    2.528772451424552,
-                    2.356194490192345
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14201,30 +15359,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2365.819661825651,
+                    0.1277039963730371,
+                    2365.820072653962
+                ],
+                "i_from_angle": [
+                    -2.091211974561429,
+                    -0.5236056997407288,
+                    1.050434657497871
+                ],
+                "i_to": [
+                    40977.20210122772,
+                    20488.59578095684,
+                    20488.606454589426
+                ],
+                "i_to_angle": [
+                    1.0504076682654613,
+                    -2.091265953049525,
+                    -2.09110401764132
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    22402.312747881486,
-                    1.8346134549116837e-12,
-                    2.051160198809135e-12
-                ],
-                "i_angle": [
-                    2.23297612691668,
-                    -2.0344439357957027,
-                    -2.498091544796509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14393,30 +15567,46 @@
                 "i_angle": [
                     -0.8473731745890964,
                     -1.0504973838084937,
                     -1.0508959932953557
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    392.4581915819866,
+                    0.028527483315196944,
+                    392.4840416381267
+                ],
+                "i_from_angle": [
+                    -1.0503052480947048,
+                    -0.6135741734012512,
+                    2.0913181495331368
+                ],
+                "i_to": [
+                    6797.799143915923,
+                    3398.5637734928873,
+                    3399.2353776514447
+                ],
+                "i_to_angle": [
+                    2.0913027780203506,
+                    -1.0503359961830285,
+                    -1.050243764068141
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    205032.25844191352,
-                    2.80401926733944e-11,
-                    2.5047681269829595e-11
-                ],
-                "i_angle": [
-                    2.2049079962374933,
-                    -1.9295669970654687,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14585,30 +15775,46 @@
                 "i_angle": [
                     -1.0512241307607684,
                     2.769081609693555,
                     2.7690738170091738
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    3592.077710973006,
+                    0.028527483314505966,
+                    3592.1032115667294
+                ],
+                "i_from_angle": [
+                    -1.078410677446369,
+                    -0.6135741733901677,
+                    2.0631855362318077
+                ],
+                "i_to": [
+                    62216.831842930784,
+                    31108.084659479322,
+                    31108.7471843386
+                ],
+                "i_to_angle": [
+                    2.0631837561939346,
+                    -1.0784142375853008,
+                    -1.0784035573201483
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.748158405083368,
-                    8.18684547740158e-16,
-                    8.258935698000961e-16
-                ],
-                "i_angle": [
-                    -2.0944632553048095,
-                    -0.2068378622272056,
-                    -0.24497866312686414
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14777,30 +15983,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379493154850622,
+                    0.12770399637317842,
+                    0.33795527136631337
+                ],
+                "i_from_angle": [
+                    1.2372252868487605,
+                    -0.5236056997451537,
+                    -2.2845282826909568
+                ],
+                "i_to": [
+                    5.7480781562560095,
+                    3.3183844217710248,
+                    3.318520895266836
+                ],
+                "i_to_angle": [
+                    -2.0944495201197593,
+                    1.570648433648122,
+                    0.5236615714162574
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    17760.976526474282,
-                    2.051160198809135e-12,
-                    2.469923953021461e-12
-                ],
-                "i_angle": [
-                    1.9601627077040327,
-                    -2.214297435588181,
-                    -2.297438667476622
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14969,30 +16191,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    683.5757682608864,
+                    0.12770399637281488,
+                    683.6768327564602
+                ],
+                "i_from_angle": [
+                    -1.1813690329610833,
+                    -0.5236056997437116,
+                    1.9603378143917738
+                ],
+                "i_to": [
+                    11840.75483941297,
+                    5919.064640268169,
+                    5921.690372851553
+                ],
+                "i_to_angle": [
+                    1.9602807217307257,
+                    -1.1814832604940173,
+                    -1.1811406791928294
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    136915.96230745324,
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11
-                ],
-                "i_angle": [
-                    1.148330201987778,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15161,30 +16399,46 @@
                 "i_angle": [
                     -1.9947264499020332,
                     -1.974244983047042,
                     -1.9747637940348024
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    571.6103589428899,
+                    0.02852748331542307,
+                    571.6163028687619
+                ],
+                "i_from_angle": [
+                    -1.9744992190226975,
+                    -0.6135741733991866,
+                    1.1671422462012484
+                ],
+                "i_to": [
+                    9900.633311177093,
+                    4950.239454995499,
+                    4950.393882719229
+                ],
+                "i_to_angle": [
+                    1.1671178405110643,
+                    -1.9745480316718862,
+                    -1.9744015967696296
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    136727.84188424365,
-                    1.3356187556109646e-11,
-                    1.3127425272378464e-11
-                ],
-                "i_angle": [
-                    1.171820801074162,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15353,30 +16607,46 @@
                 "i_angle": [
                     -1.9947264499020334,
                     -2.487043174079903,
                     -2.4874465649398103
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    570.8247385314772,
+                    0.028527483315286383,
+                    570.8313362052144
+                ],
+                "i_from_angle": [
+                    -1.9510075203121573,
+                    -0.6135741733990432,
+                    1.1906337539848402
+                ],
+                "i_to": [
+                    9887.031628146427,
+                    4943.430120924612,
+                    4943.601533516075
+                ],
+                "i_to_angle": [
+                    1.1906094437717287,
+                    -1.9510561421431893,
+                    -1.9509102800217686
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.748468897310853,
-                    4.344673780753835e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.094554694044177,
-                    -0.39735401778895213,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15545,30 +16815,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795801274392934,
+                    0.1277039963731637,
+                    0.3379717173258611
+                ],
+                "i_from_angle": [
+                    1.237158544639972,
+                    -0.5236056997450331,
+                    -2.2845807091515065
+                ],
+                "i_to": [
+                    5.748299897509254,
+                    3.318391663394129,
+                    3.3187056937756316
+                ],
+                "i_to_angle": [
+                    -2.094511309907328,
+                    1.5705853814019168,
+                    0.5236319245461281
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12543.843934648457,
-                    1.1603114287023091e-12,
-                    1.1603114287023091e-12
-                ],
-                "i_angle": [
-                    2.040795602241189,
-                    -2.356194490192345,
-                    -2.356194490192345
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15737,30 +17023,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    482.7527666890548,
+                    0.12770399637316113,
+                    482.859795045005
+                ],
+                "i_from_angle": [
+                    -1.1006884836561186,
+                    -0.5236056997441245,
+                    2.0410484621992997
+                ],
+                "i_to": [
+                    8362.450064987113,
+                    4179.834791330796,
+                    4182.615469528245
+                ],
+                "i_to_angle": [
+                    2.040976324063154,
+                    -1.1008328399133507,
+                    -1.1003999630799406
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35448.479883073465,
-                    4.10232039761827e-12,
-                    3.1309601587286993e-12
-                ],
-                "i_angle": [
-                    1.9999451994518511,
-                    -2.214297435588181,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15929,30 +17231,46 @@
                 "i_angle": [
                     -1.1430836906933466,
                     -1.1229205767117405,
                     -1.1240992170421655
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    147.97693112895487,
+                    0.028527483315241034,
+                    148.00184016008106
+                ],
+                "i_from_angle": [
+                    -1.1227712824547507,
+                    -0.6135741733992833,
+                    2.018915332629333
+                ],
+                "i_to": [
+                    2563.2513463433024,
+                    1281.3021080979902,
+                    1281.9492637044427
+                ],
+                "i_to_angle": [
+                    2.0188683558360014,
+                    -1.1228652755867088,
+                    -1.1225833910895235
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35279.978347555196,
-                    4.10232039761827e-12,
-                    4.78848169866233e-12
-                ],
-                "i_angle": [
-                    2.0037248298386054,
-                    -2.214297435588181,
-                    -2.32590073027357
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16121,30 +17439,46 @@
                 "i_angle": [
                     -1.162795058082173,
                     -1.6549429599546457,
                     -1.6565097193635687
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    147.27347351062767,
+                    0.02852748331535079,
+                    147.29843493448598
+                ],
+                "i_from_angle": [
+                    -1.1189905522583279,
+                    -0.613574173398919,
+                    2.0226958715269503
+                ],
+                "i_to": [
+                    2551.06755674343,
+                    1275.2095325844537,
+                    1275.8580493940253
+                ],
+                "i_to_angle": [
+                    2.0226489904021547,
+                    -1.1190843542446518,
+                    -1.1188030436436878
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.747526034574178,
-                    8.041086459980025e-16,
-                    8.012344526598184e-16
-                ],
-                "i_angle": [
-                    -2.0945082930762267,
-                    -0.08457559607190217,
-                    0.0
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16313,30 +17647,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33791725691064484,
+                    0.12770399637327606,
+                    0.33792615429513784
+                ],
+                "i_from_angle": [
+                    1.2372200838188165,
+                    -0.5236056997452951,
+                    -2.284568317003021
+                ],
+                "i_to": [
+                    5.7475386418368215,
+                    3.3181170939817246,
+                    3.3183209651975596
+                ],
+                "i_to_angle": [
+                    -2.094472976587306,
+                    1.570671481826725,
+                    0.5236033392503372
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    55809.55246338669,
-                    6.678093778054823e-12,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    1.1381080045539778,
-                    2.9562447035940984,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16505,30 +17855,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2148.1599442770134,
+                    0.12770399637298238,
+                    2148.171539376016
+                ],
+                "i_from_angle": [
+                    -2.003509726602329,
+                    -0.5236056997399869,
+                    1.1381421293601008
+                ],
+                "i_to": [
+                    37207.32206292302,
+                    18603.51048006251,
+                    18603.81172957033
+                ],
+                "i_to_angle": [
+                    1.1381125282536713,
+                    -2.003568929613874,
+                    -2.0033913224963684
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21414.663285460443,
-                    1.4791126541994494e-12,
-                    1.9913163527955457e-12
-                ],
-                "i_angle": [
-                    2.214388654197379,
-                    -2.5535900500422257,
-                    -2.539305307454829
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16697,30 +18063,46 @@
                 "i_angle": [
                     -0.8659571842120841,
                     -1.0690757567303182,
                     -1.0695052376503775
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    375.1545796196698,
+                    0.02852748331547031,
+                    375.18020097053176
+                ],
+                "i_from_angle": [
+                    -1.0688919646176038,
+                    -0.6135741734015381,
+                    2.072734125962205
+                ],
+                "i_to": [
+                    6498.089812433243,
+                    3248.712079192715,
+                    3249.377741413738
+                ],
+                "i_to_angle": [
+                    2.072717408038076,
+                    -1.0689254061750835,
+                    -1.0688250952041753
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    142887.18546987922,
-                    2.366580246719119e-11,
-                    2.4041979785572788e-11
-                ],
-                "i_angle": [
-                    2.0889041942220152,
-                    -2.5535900500422257,
-                    -2.5305172221520817
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16889,30 +18271,46 @@
                 "i_angle": [
                     -1.167222703343486,
                     2.6530822968485546,
                     2.653081466641693
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2503.3136633204977,
+                    0.028527483314684854,
+                    2503.337512410011
+                ],
+                "i_from_angle": [
+                    -1.1944137234377359,
+                    -0.6135741733857517,
+                    1.9471851833127325
+                ],
+                "i_to": [
+                    43358.87106048655,
+                    21679.125722436325,
+                    21679.745339957582
+                ],
+                "i_to_angle": [
+                    1.9471820567472886,
+                    -1.1944199767175603,
+                    -1.194401217235531
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.7482104232866735,
-                    4.344673780753835e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.0944723059407107,
-                    -0.39735401778895213,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17081,30 +18479,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.33795090337872924,
+                    0.12770399637305999,
+                    0.33795761603056784
+                ],
+                "i_from_angle": [
+                    1.2372183481046142,
+                    -0.5236056997448749,
+                    -2.2845329824518905
+                ],
+                "i_to": [
+                    5.748112837912838,
+                    3.3183907696533317,
+                    3.318544584047291
+                ],
+                "i_to_angle": [
+                    -2.0944555547717583,
+                    1.5706412946214492,
+                    0.5236596571226464
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    17090.403201116897,
-                    2.051160198809135e-12,
-                    1.5654800793643497e-12
-                ],
-                "i_angle": [
-                    1.9553211642884165,
-                    -2.214297435588181,
-                    -2.1224513093234436
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17273,30 +18687,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    657.7623765890656,
+                    0.12770399637314112,
+                    657.8630622977595
+                ],
+                "i_from_angle": [
+                    -1.1862086638218121,
+                    -0.5236056997447096,
+                    1.955503406424493
+                ],
+                "i_to": [
+                    11393.650499100764,
+                    5695.517395239622,
+                    5698.13328664812
+                ],
+                "i_to_angle": [
+                    1.9554437026657558,
+                    -1.1863281170411664,
+                    -1.1859698670582517
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109429.52799393355,
-                    1.9759391624171684e-11,
-                    1.640928159047308e-11
-                ],
-                "i_angle": [
-                    1.302974132893974,
-                    -3.058451421701352,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17465,30 +18895,46 @@
                 "i_angle": [
                     -1.8400800604182057,
                     -1.819576712276655,
                     -1.820208641738679
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8507831403224,
+                    0.02852748331513395,
+                    456.8609540097659
+                ],
+                "i_from_angle": [
+                    -1.8198497781443317,
+                    -0.6135741733981159,
+                    1.3218012150281153
+                ],
+                "i_to": [
+                    7912.975757713378,
+                    3956.3557705365633,
+                    3956.6200174751652
+                ],
+                "i_to_angle": [
+                    1.3217720455614885,
+                    -1.819908120324474,
+                    -1.819733101576735
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109000.79805496582,
-                    1.3531440247604774e-11,
-                    1.3531440247604774e-11
-                ],
-                "i_angle": [
-                    1.321342086586508,
-                    -2.896613990462929,
-                    -2.896613990462929
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17657,30 +19103,46 @@
                 "i_angle": [
                     -1.845202770771154,
                     -2.337465947871521,
                     -2.337999824103851
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    455.06071558934633,
+                    0.028527483315483534,
+                    455.07137429919163
+                ],
+                "i_from_angle": [
+                    -1.8014807248097613,
+                    -0.6135741733988664,
+                    1.3401700774087604
+                ],
+                "i_to": [
+                    7881.975103097586,
+                    3940.8491058380027,
+                    3941.126027241994
+                ],
+                "i_to_angle": [
+                    1.3401410034348904,
+                    -1.8015388761623425,
+                    -1.8013644302763592
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    5.7485209162401265,
-                    8.449575060241685e-16,
-                    6.334314525508457e-16
-                ],
-                "i_angle": [
-                    -2.094563745950491,
-                    -0.3231049223228771,
-                    -0.3217505543966422
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17849,30 +19311,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    0.3379596005369549,
+                    0.12770399637324598,
+                    0.337974062036374
+                ],
+                "i_from_angle": [
+                    1.2371516047793492,
+                    -0.523605699744634,
+                    -2.2845854100966676
+                ],
+                "i_to": [
+                    5.748334578718067,
+                    3.318398009128972,
+                    3.3187293841463785
+                ],
+                "i_to_angle": [
+                    -2.0945173457092254,
+                    1.5705782413910658,
+                    0.5236300090573025
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12209.990635538234,
-                    1.740467143053464e-12,
-                    1.4791126541994494e-12
-                ],
-                "i_angle": [
-                    2.0351758962812303,
-                    -2.356194490192345,
-                    -2.158798930342464
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18041,30 +19519,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    469.9009910110001,
+                    0.1277039963732222,
+                    470.0076264988873
+                ],
+                "i_from_angle": [
+                    -1.1063062766241116,
+                    -0.5236056997440959,
+                    2.035435891701585
+                ],
+                "i_to": [
+                    8139.847377249304,
+                    4068.5385553882616,
+                    4071.309026569986
+                ],
+                "i_to_angle": [
+                    2.0353611428150837,
+                    -1.1064558592313762,
+                    -1.1060073149841618
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    32886.210755032254,
-                    3.6692269098233675e-12,
-                    4.10232039761827e-12
-                ],
-                "i_angle": [
-                    1.9877468368006401,
-                    -2.677945044588987,
-                    -2.498091544796509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18233,30 +19727,46 @@
                 "i_angle": [
                     -1.155279594676233,
                     -1.1350945970664827,
                     -1.1363864355210234
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    137.27899008719672,
+                    0.028527483315236944,
+                    137.30372779337205
+                ],
+                "i_from_angle": [
+                    -1.1349641329410305,
+                    -0.6135741734040746,
+                    2.006732007547474
+                ],
+                "i_to": [
+                    2377.95608806413,
+                    1188.656706130901,
+                    1189.299410583394
+                ],
+                "i_to_angle": [
+                    2.0066802687597893,
+                    -1.1350676571420824,
+                    -1.1347571964280048
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    32742.559189895983,
-                    4.10232039761827e-12,
-                    3.6692269098233675e-12
-                ],
-                "i_angle": [
-                    1.9913080968758046,
-                    -2.214297435588181,
-                    -2.0344439357957027
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18425,10 +19935,36 @@
                 "i_angle": [
                     -1.1752093973334015,
                     -1.6673038083902076,
                     -1.6690009797019687
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    136.67927963903668,
+                    0.028527483315338827,
+                    136.70406780028856
+                ],
+                "i_from_angle": [
+                    -1.1314017730383141,
+                    -0.6135741734033183,
+                    2.0102941761243986
+                ],
+                "i_to": [
+                    2367.569235383094,
+                    1183.4626242444488,
+                    1184.106639558292
+                ],
+                "i_to_angle": [
+                    2.010242533020936,
+                    -1.1315051060843078,
+                    -1.1311952193473738
+                ],
+                "id": 6
+            }
         ]
     }
 ]
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -2,16 +2,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -26,16 +26,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -50,16 +50,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -74,16 +74,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -98,16 +98,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -122,16 +122,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -146,16 +146,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -170,16 +170,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -194,16 +194,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -218,16 +218,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -242,16 +242,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -266,16 +266,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -578,16 +578,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -602,16 +602,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -626,16 +626,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -650,16 +650,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -674,16 +674,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -698,16 +698,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -722,16 +722,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -746,16 +746,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -770,16 +770,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -794,16 +794,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -818,16 +818,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -842,16 +842,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 2,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1154,16 +1154,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1178,16 +1178,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1202,16 +1202,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1226,16 +1226,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1250,16 +1250,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1274,16 +1274,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1298,16 +1298,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1322,16 +1322,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1346,16 +1346,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1370,16 +1370,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1394,16 +1394,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1418,16 +1418,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 3,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1730,16 +1730,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1754,16 +1754,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1778,16 +1778,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1802,16 +1802,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1826,16 +1826,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1850,16 +1850,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1874,16 +1874,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1898,16 +1898,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1922,16 +1922,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1946,16 +1946,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1970,16 +1970,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1994,16 +1994,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 1,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/input.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -12,36 +12,36 @@
     ],
     "line": [
         {
             "c0": 6.4e-07,
             "c1": 6.4e-07,
             "from_node": 1,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 7,
             "r0": 0.75,
             "r1": 0.049,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 2,
             "to_status": 1,
             "x0": 0.04,
             "x1": 0.153
         },
         {
             "c0": 3.2e-07,
             "c1": 3.2e-07,
             "from_node": 2,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 8,
             "r0": 0.375,
             "r1": 0.0245,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 3,
             "to_status": 1,
             "x0": 0.02,
             "x1": 0.0765
         }
     ],
     "node": [
@@ -61,60 +61,60 @@
             "id": 3,
             "u_rated": 10000.0
         }
     ],
     "shunt": [
         {
             "b0": 5.0,
-            "b1": 0,
-            "g0": 0,
-            "g1": 0,
+            "b1": 0.0,
+            "g0": 0.0,
+            "g1": 0.0,
             "id": 9,
             "node": 1,
             "status": 1
         }
     ],
     "source": [
         {
             "id": 4,
             "node": 0,
             "rx_ratio": 0.1,
             "sk": 20000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": 0.0,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         },
         {
             "id": 5,
             "node": 2,
             "rx_ratio": 0.1,
             "sk": 2000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": -0.5235987755982988,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         }
     ],
     "transformer": [
         {
             "clock": 1,
             "from_node": 0,
             "from_status": 1,
-            "i0": 0,
+            "i0": 0.0,
             "id": 6,
-            "p0": 0,
-            "pk": 0,
+            "p0": 0.0,
+            "pk": 0.0,
             "sn": 20000000.0,
             "tap_max": 1,
             "tap_min": -1,
             "tap_nom": 0,
             "tap_pos": 0,
             "tap_side": 0,
-            "tap_size": 100,
+            "tap_size": 100.0,
             "to_node": 1,
             "to_status": 1,
             "u1": 150000.0,
             "u2": 10000.0,
             "uk": 0.05,
             "winding_from": 1,
             "winding_to": 2
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {'0': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer': [OrderedDict([('id', 6), "*

 * *      "('energized', 1), ('i_from', [1660.5121389811575, 1660.5121389811572, 1660.512138981157]), "*

 * *      "('i_from_angle', [-1.5688450860816423, 2.619945118704748, 0.525550016311553]), ('i_to', "*

 * *      "[24907.682084717362, 24907.68208471736, 24907.682084717362]), ('i_to_angle', "*

 * *      '[1.049148791909852, -1.0452463104833438, -3.139641412876539])])]}',*

 * * '1': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer […]*

```diff
@@ -1,22 +1,12 @@
 [
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    24907.682084717355,
-                    24907.682084717355,
-                    24907.682084717362
-                ],
-                "i_angle": [
-                    1.0491487919098523,
-                    -1.0452463104833436,
-                    -3.139641412876539
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -185,30 +175,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
-        ]
-    },
-    {
-        "fault": [
+        ],
+        "transformer": [
             {
                 "energized": 1,
-                "i": [
-                    24907.682084717355,
-                    24907.682084717355,
+                "i_from": [
+                    1660.5121389811575,
+                    1660.5121389811572,
+                    1660.512138981157
+                ],
+                "i_from_angle": [
+                    -1.5688450860816423,
+                    2.619945118704748,
+                    0.525550016311553
+                ],
+                "i_to": [
+                    24907.682084717362,
+                    24907.68208471736,
                     24907.682084717362
                 ],
-                "i_angle": [
-                    1.0491487919098523,
-                    -1.0452463104833436,
+                "i_to_angle": [
+                    1.049148791909852,
+                    -1.0452463104833438,
                     -3.139641412876539
                 ],
+                "id": 6
+            }
+        ]
+    },
+    {
+        "fault": [
+            {
+                "energized": 1,
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -377,30 +383,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811575,
+                    1660.5121389811572,
+                    1660.512138981157
+                ],
+                "i_from_angle": [
+                    -1.5688450860816423,
+                    2.619945118704748,
+                    0.525550016311553
+                ],
+                "i_to": [
+                    24907.682084717362,
+                    24907.68208471736,
+                    24907.682084717362
+                ],
+                "i_to_angle": [
+                    1.049148791909852,
+                    -1.0452463104833438,
+                    -3.139641412876539
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    54722.06131378445,
-                    54722.06131378444,
-                    54722.06131378444
-                ],
-                "i_angle": [
-                    1.1908776028886958,
-                    -0.9035174995045,
-                    -2.997912601897695
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -569,30 +591,46 @@
                 "i_angle": [
                     -1.8342075759919427,
                     2.354582628794448,
                     0.26018752640125253
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.512138981158,
+                    1660.5121389811577,
+                    1660.5121389811577
+                ],
+                "i_from_angle": [
+                    -1.568845086081642,
+                    2.6199451187047487,
+                    0.5255500163115532
+                ],
+                "i_to": [
+                    24907.682084717362,
+                    24907.68208471736,
+                    24907.68208471737
+                ],
+                "i_to_angle": [
+                    1.0491487919098523,
+                    -1.0452463104833436,
+                    -3.139641412876539
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    54722.06131378445,
-                    54722.06131378444,
-                    54722.06131378444
-                ],
-                "i_angle": [
-                    1.1908776028886958,
-                    -0.9035174995045,
-                    -2.997912601897695
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -761,30 +799,46 @@
                 "i_angle": [
                     -1.8342075759919427,
                     2.354582628794448,
                     0.26018752640125253
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.512138981158,
+                    1660.5121389811577,
+                    1660.5121389811577
+                ],
+                "i_from_angle": [
+                    -1.568845086081642,
+                    2.6199451187047487,
+                    0.5255500163115532
+                ],
+                "i_to": [
+                    24907.682084717362,
+                    24907.68208471736,
+                    24907.68208471737
+                ],
+                "i_to_angle": [
+                    1.0491487919098523,
+                    -1.0452463104833436,
+                    -3.139641412876539
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15453.59521965815,
-                    15453.59521965815,
-                    15453.59521965815
-                ],
-                "i_angle": [
-                    1.1679303876567342,
-                    -0.9264647147364619,
-                    -3.020859817129657
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -953,30 +1007,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616869,
+                    1030.2238349616869,
+                    1030.2238349616869
+                ],
+                "i_from_angle": [
+                    -1.45005856424171,
+                    2.7387316405446804,
+                    0.6443365381514851
+                ],
+                "i_to": [
+                    15453.357524425304,
+                    15453.357524425302,
+                    15453.357524425304
+                ],
+                "i_to_angle": [
+                    1.1679353137497843,
+                    -0.9264597886434116,
+                    -3.020854891036607
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15453.59521965815,
-                    15453.59521965815,
-                    15453.59521965815
-                ],
-                "i_angle": [
-                    1.1679303876567342,
-                    -0.9264647147364619,
-                    -3.020859817129657
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1145,30 +1215,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616869,
+                    1030.2238349616869,
+                    1030.2238349616869
+                ],
+                "i_from_angle": [
+                    -1.45005856424171,
+                    2.7387316405446804,
+                    0.6443365381514851
+                ],
+                "i_to": [
+                    15453.357524425304,
+                    15453.357524425302,
+                    15453.357524425304
+                ],
+                "i_to_angle": [
+                    1.1679353137497843,
+                    -0.9264597886434116,
+                    -3.020854891036607
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    142467.59801421993,
-                    142467.59801421993,
-                    142467.5980142199
-                ],
-                "i_angle": [
-                    1.1491508886893056,
-                    -0.9452442137038903,
-                    -3.0396393160970856
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1337,30 +1423,46 @@
                 "i_angle": [
                     -1.9947264499020332,
                     2.194063754884357,
                     0.09966865249116198
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    1030.2238349616873,
+                    1030.2238349616873
+                ],
+                "i_from_angle": [
+                    -1.45005856424171,
+                    2.7387316405446804,
+                    0.6443365381514852
+                ],
+                "i_to": [
+                    15453.357524425312,
+                    15453.357524425312,
+                    15453.357524425312
+                ],
+                "i_to_angle": [
+                    1.1679353137497843,
+                    -0.9264597886434115,
+                    -3.0208548910366066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    142467.59801421993,
-                    142467.59801421993,
-                    142467.5980142199
-                ],
-                "i_angle": [
-                    1.1491508886893056,
-                    -0.9452442137038903,
-                    -3.0396393160970856
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1529,30 +1631,46 @@
                 "i_angle": [
                     -1.9947264499020332,
                     2.194063754884357,
                     0.09966865249116198
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    1030.2238349616873,
+                    1030.2238349616873
+                ],
+                "i_from_angle": [
+                    -1.45005856424171,
+                    2.7387316405446804,
+                    0.6443365381514852
+                ],
+                "i_to": [
+                    15453.357524425312,
+                    15453.357524425312,
+                    15453.357524425312
+                ],
+                "i_to_angle": [
+                    1.1679353137497843,
+                    -0.9264597886434115,
+                    -3.0208548910366066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12958.734103946166,
-                    12958.734103946163,
-                    12958.734103946163
-                ],
-                "i_angle": [
-                    1.198758848400844,
-                    -0.8956362539923519,
-                    -2.9900313563855474
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1721,30 +1839,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150775,
+                    863.8857089150775,
+                    863.8857089150775
+                ],
+                "i_from_angle": [
+                    -1.4192239457818372,
+                    2.7695662590045536,
+                    0.6751711566113582
+                ],
+                "i_to": [
+                    12958.285633726166,
+                    12958.285633726164,
+                    12958.285633726162
+                ],
+                "i_to_angle": [
+                    1.1987699322096572,
+                    -0.8956251701835386,
+                    -2.990020272576734
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12958.734103946166,
-                    12958.734103946163,
-                    12958.734103946163
-                ],
-                "i_angle": [
-                    1.198758848400844,
-                    -0.8956362539923519,
-                    -2.9900313563855474
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1913,30 +2047,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150775,
+                    863.8857089150775,
+                    863.8857089150775
+                ],
+                "i_from_angle": [
+                    -1.4192239457818372,
+                    2.7695662590045536,
+                    0.6751711566113582
+                ],
+                "i_to": [
+                    12958.285633726166,
+                    12958.285633726164,
+                    12958.285633726162
+                ],
+                "i_to_angle": [
+                    1.1987699322096572,
+                    -0.8956251701835386,
+                    -2.990020272576734
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    51099.17193306465,
-                    51099.171933064645,
-                    51099.17193306464
-                ],
-                "i_angle": [
-                    1.283006950461127,
-                    -0.8113881519320688,
-                    -2.905783254325264
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2105,30 +2255,46 @@
                 "i_angle": [
                     -1.8608657416098184,
                     2.327924463176572,
                     0.2335293607833768
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.4972624705647,
+                    369.49726247056475,
+                    369.4972624705647
+                ],
+                "i_from_angle": [
+                    -1.3161834464356774,
+                    2.872606758350713,
+                    0.778211655957518
+                ],
+                "i_to": [
+                    5542.458937058473,
+                    5542.458937058473,
+                    5542.458937058474
+                ],
+                "i_to_angle": [
+                    1.301810431555817,
+                    -0.792584670837379,
+                    -2.8869797732305744
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    51099.17193306465,
-                    51099.171933064645,
-                    51099.17193306464
-                ],
-                "i_angle": [
-                    1.283006950461127,
-                    -0.8113881519320688,
-                    -2.905783254325264
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2297,30 +2463,46 @@
                 "i_angle": [
                     -1.8608657416098184,
                     2.327924463176572,
                     0.2335293607833768
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.4972624705647,
+                    369.49726247056475,
+                    369.4972624705647
+                ],
+                "i_from_angle": [
+                    -1.3161834464356774,
+                    2.872606758350713,
+                    0.778211655957518
+                ],
+                "i_to": [
+                    5542.458937058473,
+                    5542.458937058473,
+                    5542.458937058474
+                ],
+                "i_to_angle": [
+                    1.301810431555817,
+                    -0.792584670837379,
+                    -2.8869797732305744
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    23949.012543356162,
-                    23949.012543356162,
-                    23949.012543356166
-                ],
-                "i_angle": [
-                    1.0867910429653747,
-                    -1.0076040594278213,
-                    -3.1019991618210168
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2489,30 +2671,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1596.5960209271025,
+                    1596.5960209271022,
+                    1596.5960209271022
+                ],
+                "i_from_angle": [
+                    -1.531199819003861,
+                    2.65759038578253,
+                    0.5631952833893343
+                ],
+                "i_to": [
+                    23948.940313906536,
+                    23948.940313906533,
+                    23948.940313906536
+                ],
+                "i_to_angle": [
+                    1.0867940589876335,
+                    -1.0076010434055624,
+                    -3.1019961457987577
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    23949.012543356162,
-                    23949.012543356162,
-                    23949.012543356166
-                ],
-                "i_angle": [
-                    1.0867910429653747,
-                    -1.0076040594278213,
-                    -3.1019991618210168
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2681,30 +2879,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1596.5960209271025,
+                    1596.5960209271022,
+                    1596.5960209271022
+                ],
+                "i_from_angle": [
+                    -1.531199819003861,
+                    2.65759038578253,
+                    0.5631952833893343
+                ],
+                "i_to": [
+                    23948.940313906536,
+                    23948.940313906533,
+                    23948.940313906536
+                ],
+                "i_to_angle": [
+                    1.0867940589876335,
+                    -1.0076010434055624,
+                    -3.1019961457987577
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    49745.79732013114,
-                    49745.79732013113,
-                    49745.79732013113
-                ],
-                "i_angle": [
-                    1.2572315242591852,
-                    -0.8371635781340109,
-                    -2.931558680527206
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2873,30 +3087,46 @@
                 "i_angle": [
                     -1.767849047257144,
                     2.4209411575292465,
                     0.3265460551360513
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1509.507681033466,
+                    1509.5076810334665,
+                    1509.5076810334663
+                ],
+                "i_from_angle": [
+                    -1.5024897629871372,
+                    2.6863004417992533,
+                    0.591905339406058
+                ],
+                "i_to": [
+                    22642.615215501995,
+                    22642.61521550199,
+                    22642.61521550199
+                ],
+                "i_to_angle": [
+                    1.1155041150043572,
+                    -0.9788909873888387,
+                    -3.073286089782034
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    49745.79732013114,
-                    49745.79732013113,
-                    49745.79732013113
-                ],
-                "i_angle": [
-                    1.2572315242591852,
-                    -0.8371635781340109,
-                    -2.931558680527206
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3065,30 +3295,46 @@
                 "i_angle": [
                     -1.767849047257144,
                     2.4209411575292465,
                     0.3265460551360513
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1509.507681033466,
+                    1509.5076810334665,
+                    1509.5076810334663
+                ],
+                "i_from_angle": [
+                    -1.5024897629871372,
+                    2.6863004417992533,
+                    0.591905339406058
+                ],
+                "i_to": [
+                    22642.615215501995,
+                    22642.61521550199,
+                    22642.61521550199
+                ],
+                "i_to_angle": [
+                    1.1155041150043572,
+                    -0.9788909873888387,
+                    -3.073286089782034
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15042.876821861519,
-                    15042.876821861515,
-                    15042.876821861519
-                ],
-                "i_angle": [
-                    1.188590553208936,
-                    -0.90580454918426,
-                    -3.0001996515774554
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3257,30 +3503,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1002.8400050881113,
+                    1002.8400050881111,
+                    1002.8400050881111
+                ],
+                "i_from_angle": [
+                    -1.4293953827284975,
+                    2.7593948220578928,
+                    0.6649997196646976
+                ],
+                "i_to": [
+                    15042.600076321669,
+                    15042.600076321669,
+                    15042.600076321669
+                ],
+                "i_to_angle": [
+                    1.1885984952629969,
+                    -0.905796607130199,
+                    -3.0001917095233943
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15042.876821861519,
-                    15042.876821861515,
-                    15042.876821861519
-                ],
-                "i_angle": [
-                    1.188590553208936,
-                    -0.90580454918426,
-                    -3.0001996515774554
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3449,30 +3711,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1002.8400050881113,
+                    1002.8400050881111,
+                    1002.8400050881111
+                ],
+                "i_from_angle": [
+                    -1.4293953827284975,
+                    2.7593948220578928,
+                    0.6649997196646976
+                ],
+                "i_to": [
+                    15042.600076321669,
+                    15042.600076321669,
+                    15042.600076321669
+                ],
+                "i_to_angle": [
+                    1.1885984952629969,
+                    -0.905796607130199,
+                    -3.0001917095233943
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    112890.88928291772,
-                    112890.8892829177,
-                    112890.88928291768
-                ],
-                "i_angle": [
-                    1.308565669076994,
-                    -0.7858294333162018,
-                    -2.880224535709397
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3641,30 +3919,46 @@
                 "i_angle": [
                     -1.835309113464794,
                     2.3534810913215964,
                     0.2590859889284013
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    816.3417279386364,
+                    816.3417279386364,
+                    816.3417279386364
+                ],
+                "i_from_angle": [
+                    -1.2906369345651172,
+                    2.898153270221273,
+                    0.803758167828078
+                ],
+                "i_to": [
+                    12245.125919079552,
+                    12245.125919079552,
+                    12245.12591907955
+                ],
+                "i_to_angle": [
+                    1.3273569434263772,
+                    -0.7670381589668186,
+                    -2.861433261360014
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    112890.88928291772,
-                    112890.8892829177,
-                    112890.88928291768
-                ],
-                "i_angle": [
-                    1.308565669076994,
-                    -0.7858294333162018,
-                    -2.880224535709397
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3833,30 +4127,46 @@
                 "i_angle": [
                     -1.835309113464794,
                     2.3534810913215964,
                     0.2590859889284013
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    816.3417279386364,
+                    816.3417279386364,
+                    816.3417279386364
+                ],
+                "i_from_angle": [
+                    -1.2906369345651172,
+                    2.898153270221273,
+                    0.803758167828078
+                ],
+                "i_to": [
+                    12245.125919079552,
+                    12245.125919079552,
+                    12245.12591907955
+                ],
+                "i_to_angle": [
+                    1.3273569434263772,
+                    -0.7670381589668186,
+                    -2.861433261360014
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12662.534438164219,
-                    12662.534438164219,
-                    12662.534438164217
-                ],
-                "i_angle": [
-                    1.2154569442572354,
-                    -0.8789381581359604,
-                    -2.973333260529156
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4025,30 +4335,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    844.1372020146126,
+                    844.1372020146126,
+                    844.1372020146124
+                ],
+                "i_from_angle": [
+                    -1.4025228339031872,
+                    2.7862673708832033,
+                    0.691872268490008
+                ],
+                "i_to": [
+                    12662.058030219188,
+                    12662.058030219188,
+                    12662.058030219188
+                ],
+                "i_to_angle": [
+                    1.2154710440883072,
+                    -0.8789240583048886,
+                    -2.9733191606980838
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    12662.534438164219,
-                    12662.534438164219,
-                    12662.534438164217
-                ],
-                "i_angle": [
-                    1.2154569442572354,
-                    -0.8789381581359604,
-                    -2.973333260529156
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4217,30 +4543,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    844.1372020146126,
+                    844.1372020146126,
+                    844.1372020146124
+                ],
+                "i_from_angle": [
+                    -1.4025228339031872,
+                    2.7862673708832033,
+                    0.691872268490008
+                ],
+                "i_to": [
+                    12662.058030219188,
+                    12662.058030219188,
+                    12662.058030219188
+                ],
+                "i_to_angle": [
+                    1.2154710440883072,
+                    -0.8789240583048886,
+                    -2.9733191606980838
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    46511.33833905129,
-                    46511.33833905128,
-                    46511.33833905128
-                ],
-                "i_angle": [
-                    1.3371317198246397,
-                    -0.7572633825685562,
-                    -2.8516584849617512
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4409,30 +4751,46 @@
                 "i_angle": [
                     -1.8067384161552897,
                     2.382051788631101,
                     0.28765668623790563
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    336.3208639973492,
+                    336.3208639973492,
+                    336.3208639973492
+                ],
+                "i_from_angle": [
+                    -1.2620518274256365,
+                    2.926738377360754,
+                    0.8323432749675587
+                ],
+                "i_to": [
+                    5044.812959960241,
+                    5044.812959960242,
+                    5044.812959960242
+                ],
+                "i_to_angle": [
+                    1.355942050565858,
+                    -0.738453051827338,
+                    -2.8328481542205335
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    46511.33833905129,
-                    46511.33833905128,
-                    46511.33833905128
-                ],
-                "i_angle": [
-                    1.3371317198246397,
-                    -0.7572633825685562,
-                    -2.8516584849617512
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4601,10 +4959,36 @@
                 "i_angle": [
                     -1.8067384161552897,
                     2.382051788631101,
                     0.28765668623790563
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    336.3208639973492,
+                    336.3208639973492,
+                    336.3208639973492
+                ],
+                "i_from_angle": [
+                    -1.2620518274256365,
+                    2.926738377360754,
+                    0.8323432749675587
+                ],
+                "i_to": [
+                    5044.812959960241,
+                    5044.812959960242,
+                    5044.812959960242
+                ],
+                "i_to_angle": [
+                    1.355942050565858,
+                    -0.738453051827338,
+                    -2.8328481542205335
+                ],
+                "id": 6
+            }
         ]
     }
 ]
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -2,16 +2,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -26,16 +26,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -50,16 +50,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -74,16 +74,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -98,16 +98,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -122,16 +122,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -146,16 +146,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -170,16 +170,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -194,16 +194,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -218,16 +218,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -242,16 +242,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -266,16 +266,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 0,
                 "fault_type": 0,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/input.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -12,36 +12,36 @@
     ],
     "line": [
         {
             "c0": 6.4e-07,
             "c1": 6.4e-07,
             "from_node": 1,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 7,
             "r0": 0.75,
             "r1": 0.049,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 2,
             "to_status": 1,
             "x0": 0.04,
             "x1": 0.153
         },
         {
             "c0": 3.2e-07,
             "c1": 3.2e-07,
             "from_node": 2,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 8,
             "r0": 0.375,
             "r1": 0.0245,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 3,
             "to_status": 1,
             "x0": 0.02,
             "x1": 0.0765
         }
     ],
     "node": [
@@ -61,60 +61,60 @@
             "id": 3,
             "u_rated": 10000.0
         }
     ],
     "shunt": [
         {
             "b0": 5.0,
-            "b1": 0,
-            "g0": 0,
-            "g1": 0,
+            "b1": 0.0,
+            "g0": 0.0,
+            "g1": 0.0,
             "id": 9,
             "node": 1,
             "status": 1
         }
     ],
     "source": [
         {
             "id": 4,
             "node": 0,
             "rx_ratio": 0.1,
             "sk": 20000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": 0.0,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         },
         {
             "id": 5,
             "node": 2,
             "rx_ratio": 0.1,
             "sk": 2000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": -0.5235987755982988,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         }
     ],
     "transformer": [
         {
             "clock": 1,
             "from_node": 0,
             "from_status": 1,
-            "i0": 0,
+            "i0": 0.0,
             "id": 6,
-            "p0": 0,
-            "pk": 0,
+            "p0": 0.0,
+            "pk": 0.0,
             "sn": 20000000.0,
             "tap_max": 1,
             "tap_min": -1,
             "tap_nom": 0,
             "tap_pos": 0,
             "tap_side": 0,
-            "tap_size": 100,
+            "tap_size": 100.0,
             "to_node": 1,
             "to_status": 1,
             "u1": 150000.0,
             "u2": 10000.0,
             "uk": 0.05,
             "winding_from": 1,
             "winding_to": 2
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {'0': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer': [OrderedDict([('id', 6), "*

 * *      "('energized', 1), ('i_from', [830.2562934194068, 1660.5121389811575, 830.2558602935742]), "*

 * *      "('i_from_angle', [-0.5215143293987453, 2.6199451187047487, -0.5217807404408343]), ('i_to', "*

 * *      "[1.9155599455927432, 21570.68733150523, 21570.68358052545]), ('i_to_angle', "*

 * *      '[-2.0944020265399352, -0.5216031330483238, 2.6199007168603066])])]}',*

 * * '1': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transfor […]*

```diff
@@ -1,22 +1,12 @@
 [
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.685434751776,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5216475348850447,
-                    2.6199451187047487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -185,30 +175,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2562934194068,
+                    1660.5121389811575,
+                    830.2558602935742
+                ],
+                "i_from_angle": [
+                    -0.5215143293987453,
+                    2.6199451187047487,
+                    -0.5217807404408343
+                ],
+                "i_to": [
+                    1.9155599455927432,
+                    21570.68733150523,
+                    21570.68358052545
+                ],
+                "i_to_angle": [
+                    -2.0944020265399352,
+                    -0.5216031330483238,
+                    2.6199007168603066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.685434751776,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5216475348850447,
-                    2.6199451187047487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -377,30 +383,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2562934194068,
+                    1660.5121389811575,
+                    830.2558602935742
+                ],
+                "i_from_angle": [
+                    -0.5215143293987453,
+                    2.6199451187047487,
+                    -0.5217807404408343
+                ],
+                "i_to": [
+                    1.9155599455927432,
+                    21570.68733150523,
+                    21570.68358052545
+                ],
+                "i_to_angle": [
+                    -2.0944020265399352,
+                    -0.5216031330483238,
+                    2.6199007168603066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    47390.69524518698,
-                    47390.69524518698
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3799187239062011,
-                    2.7616739296835924
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -569,30 +591,46 @@
                 "i_angle": [
                     1.0730088201607482,
                     2.8782090426917257,
                     -0.2634388878608027
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2583377536442,
+                    1660.5121389811575,
+                    830.2538019564684
+                ],
+                "i_from_angle": [
+                    -0.5216179040936071,
+                    2.6199451187047487,
+                    -0.521677165838359
+                ],
+                "i_to": [
+                    0.4279122497268866,
+                    21570.705076381855,
+                    21570.665795226025
+                ],
+                "i_to_angle": [
+                    -2.1843705002025953,
+                    -0.5216376579365767,
+                    2.6199352417382946
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    47390.69524518698,
-                    47390.69524518698
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3799187239062011,
-                    2.7616739296835924
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -761,30 +799,46 @@
                 "i_angle": [
                     1.0730088201607482,
                     2.8782090426917257,
                     -0.2634388878608027
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2583377536442,
+                    1660.5121389811575,
+                    830.2538019564684
+                ],
+                "i_from_angle": [
+                    -0.5216179040936071,
+                    2.6199451187047487,
+                    -0.521677165838359
+                ],
+                "i_to": [
+                    0.4279122497268866,
+                    21570.705076381855,
+                    21570.665795226025
+                ],
+                "i_to_angle": [
+                    -2.1843705002025953,
+                    -0.5216376579365767,
+                    2.6199352417382946
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13383.20604002572,
-                    13383.20604002572
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4028659391381628,
-                    2.7387267144516305
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -953,30 +1007,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1252505034938,
+                    1030.223834961687,
+                    515.0986078584967
+                ],
+                "i_from_angle": [
+                    -0.40264788101995064,
+                    2.7387316405446804,
+                    -0.40307415609418473
+                ],
+                "i_to": [
+                    1.9155599455926484,
+                    13383.115589730436,
+                    13382.884857651863
+                ],
+                "i_to_angle": [
+                    -2.0944020265407057,
+                    -0.4027899678109325,
+                    2.738660594085622
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13383.20604002572,
-                    13383.20604002572
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4028659391381628,
-                    2.7387267144516305
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1145,30 +1215,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1252505034938,
+                    1030.223834961687,
+                    515.0986078584967
+                ],
+                "i_from_angle": [
+                    -0.40264788101995064,
+                    2.7387316405446804,
+                    -0.40307415609418473
+                ],
+                "i_to": [
+                    1.9155599455926484,
+                    13383.115589730436,
+                    13382.884857651863
+                ],
+                "i_to_angle": [
+                    -2.0944020265407057,
+                    -0.4027899678109325,
+                    2.738660594085622
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    123380.55909646388,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4216454381055914,
-                    2.719947215484202
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1337,30 +1423,46 @@
                 "i_angle": [
                     1.073008820163294,
                     2.7176692834466536,
                     -0.4239368760778828
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.117085389314,
+                    1030.2238349616873,
+                    515.1067507054504
+                ],
+                "i_from_angle": [
+                    -0.40281411285647434,
+                    2.738731640544681,
+                    -0.4029079141747179
+                ],
+                "i_to": [
+                    0.4279122497300422,
+                    13383.044942045051,
+                    13382.955441057302
+                ],
+                "i_to_angle": [
+                    -2.184370500199747,
+                    -0.4028453795443391,
+                    2.7387160069393555
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    123380.55909646388,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4216454381055914,
-                    2.719947215484202
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1529,30 +1631,46 @@
                 "i_angle": [
                     1.073008820163294,
                     2.7176692834466536,
                     -0.4239368760778828
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.117085389314,
+                    1030.2238349616873,
+                    515.1067507054504
+                ],
+                "i_from_angle": [
+                    -0.40281411285647434,
+                    2.738731640544681,
+                    -0.4029079141747179
+                ],
+                "i_to": [
+                    0.4279122497300422,
+                    13383.044942045051,
+                    13382.955441057302
+                ],
+                "i_to_angle": [
+                    -2.184370500199747,
+                    -0.4028453795443391,
+                    2.7387160069393555
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11222.592934905151,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.372037478394053,
-                    2.76955517519574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1721,30 +1839,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.95956806978364,
+                    863.8857089150774,
+                    431.92616851643174
+                ],
+                "i_from_angle": [
+                    -0.37177329958512473,
+                    2.7695662590045536,
+                    -0.37227950915643077
+                ],
+                "i_to": [
+                    1.9155599455931536,
+                    11222.349212554145,
+                    11222.05996392913
+                ],
+                "i_to_angle": [
+                    -2.094402026540306,
+                    -0.37194202740914817,
+                    2.769481889653898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11222.592934905151,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.372037478394053,
-                    2.76955517519574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1913,30 +2047,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.95956806978364,
+                    863.8857089150774,
+                    431.92616851643174
+                ],
+                "i_from_angle": [
+                    -0.37177329958512473,
+                    2.7695662590045536,
+                    -0.37227950915643077
+                ],
+                "i_to": [
+                    1.9155599455931536,
+                    11222.349212554145,
+                    11222.05996392913
+                ],
+                "i_to_angle": [
+                    -2.094402026540306,
+                    -0.37194202740914817,
+                    2.769481889653898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    44253.18100638276,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.28778937633376983,
-                    2.8538032772560236
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2105,30 +2255,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.8515417123339484,
                     -0.29008788851785255
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7569784519952,
+                    369.49726247056475,
+                    184.74028694531052
+                ],
+                "i_from_angle": [
+                    -0.26886003692661353,
+                    2.872606758350713,
+                    -0.2691117649229955
+                ],
+                "i_to": [
+                    0.42791224972830616,
+                    4799.982519493712,
+                    4799.837966804531
+                ],
+                "i_to_angle": [
+                    -2.1843705002023106,
+                    -0.26894394120464277,
+                    2.872564803052782
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    44253.18100638276,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.28778937633376983,
-                    2.8538032772560236
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2297,30 +2463,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.8515417123339484,
                     -0.29008788851785255
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7569784519952,
+                    369.49726247056475,
+                    184.74028694531052
+                ],
+                "i_from_angle": [
+                    -0.26886003692661353,
+                    2.872606758350713,
+                    -0.2691117649229955
+                ],
+                "i_to": [
+                    0.42791224972830616,
+                    4799.982519493712,
+                    4799.837966804531
+                ],
+                "i_to_angle": [
+                    -2.1843705002023106,
+                    -0.26894394120464277,
+                    2.872564803052782
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21151.16859553801,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5024570562950148,
-                    2.6391355972947785
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2489,30 +2671,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1099775899144,
+                    1628.2152623132843,
+                    814.1052997407485
+                ],
+                "i_from_angle": [
+                    -0.5023197310462522,
+                    2.6391371053036337,
+                    -0.5025913663064723
+                ],
+                "i_to": [
+                    1.9155599455923336,
+                    21151.156977249666,
+                    21151.116465887208
+                ],
+                "i_to_angle": [
+                    -2.0944020265395644,
+                    -0.5024102757858984,
+                    2.639091832716661
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21151.16859553801,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5024570562950148,
-                    2.6391355972947785
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2681,30 +2879,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1099775899144,
+                    1628.2152623132843,
+                    814.1052997407485
+                ],
+                "i_from_angle": [
+                    -0.5023197310462522,
+                    2.6391371053036337,
+                    -0.5025913663064723
+                ],
+                "i_to": [
+                    1.9155599455923336,
+                    21151.156977249666,
+                    21151.116465887208
+                ],
+                "i_to_angle": [
+                    -2.0944020265395644,
+                    -0.5024102757858984,
+                    2.639091832716661
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    45158.06210733907,
-                    45158.06210733907
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3451608197526424,
-                    2.796431833837151
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2873,30 +3087,46 @@
                 "i_angle": [
                     1.0730088201594121,
                     2.9129703587914277,
                     -0.22867978838902214
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.1442057334049,
+                    1582.2821677869138,
+                    791.13796281269
+                ],
+                "i_from_angle": [
+                    -0.48685795253524994,
+                    2.6547037237197704,
+                    -0.48691990744924013
+                ],
+                "i_to": [
+                    0.42791224972633846,
+                    20554.475332614144,
+                    20554.421267334797
+                ],
+                "i_to_angle": [
+                    -2.1843705001941167,
+                    -0.4868786040646023,
+                    2.654693397887189
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    45158.06210733907,
-                    45158.06210733907
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3451608197526424,
-                    2.796431833837151
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3065,30 +3295,46 @@
                 "i_angle": [
                     1.0730088201594121,
                     2.9129703587914277,
                     -0.22867978838902214
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.1442057334049,
+                    1582.2821677869138,
+                    791.13796281269
+                ],
+                "i_from_angle": [
+                    -0.48685795253524994,
+                    2.6547037237197704,
+                    -0.48691990744924013
+                ],
+                "i_to": [
+                    0.42791224972633846,
+                    20554.475332614144,
+                    20554.421267334797
+                ],
+                "i_to_angle": [
+                    -2.1843705001941167,
+                    -0.4868786040646023,
+                    2.654693397887189
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13203.66892203938,
-                    13203.66892203938
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.39239672859882896,
-                    2.749195924990964
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3257,30 +3503,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.21535250133576,
+                    1016.4017410507181,
+                    508.1864122050829
+                ],
+                "i_from_angle": [
+                    -0.39217455096988846,
+                    2.749202359062246,
+                    -0.39260605037141116
+                ],
+                "i_to": [
+                    1.91555994559508,
+                    13203.571272315212,
+                    13203.32064199255
+                ],
+                "i_to_angle": [
+                    -2.0944020265394783,
+                    -0.39231837864225394,
+                    2.7491304418118183
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13203.66892203938,
-                    13203.66892203938
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.39239672859882896,
-                    2.749195924990964
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3449,30 +3711,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.21535250133576,
+                    1016.4017410507181,
+                    508.1864122050829
+                ],
+                "i_from_angle": [
+                    -0.39217455096988846,
+                    2.749202359062246,
+                    -0.39260605037141116
+                ],
+                "i_to": [
+                    1.91555994559508,
+                    13203.571272315212,
+                    13203.32064199255
+                ],
+                "i_to_angle": [
+                    -2.0944020265394783,
+                    -0.39231837864225394,
+                    2.7491304418118183
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    109432.87250368723,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3326866610461051,
-                    2.8089059925436883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3641,30 +3919,46 @@
                 "i_angle": [
                     1.0730088201613581,
                     2.80663011907139,
                     -0.33497760154944883
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8865799742911,
+                    913.758572090266,
+                    456.87199333548836
+                ],
+                "i_from_angle": [
+                    -0.3138471476341727,
+                    2.8276938422392,
+                    -0.3139504767164904
+                ],
+                "i_to": [
+                    0.4279122497302406,
+                    11870.135209098555,
+                    11870.008885100815
+                ],
+                "i_to_angle": [
+                    -2.1843705001970752,
+                    -0.3138815899285016,
+                    2.8276766206338335
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    109432.87250368723,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3326866610461051,
-                    2.8089059925436883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3833,30 +4127,46 @@
                 "i_angle": [
                     1.0730088201613581,
                     2.80663011907139,
                     -0.33497760154944883
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8865799742911,
+                    913.758572090266,
+                    456.87199333548836
+                ],
+                "i_from_angle": [
+                    -0.3138471476341727,
+                    2.8276938422392,
+                    -0.3139504767164904
+                ],
+                "i_to": [
+                    0.4279122497302406,
+                    11870.135209098555,
+                    11870.008885100815
+                ],
+                "i_to_angle": [
+                    -2.1843705001970752,
+                    -0.3138815899285016,
+                    2.8276766206338335
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11093.238545275373,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.36359190742848624,
-                    2.778000746161307
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4025,30 +4335,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9811667515429,
+                    853.9270602593755,
+                    426.94592142748786
+                ],
+                "i_from_angle": [
+                    -0.3633236091478327,
+                    2.7780133379789755,
+                    -0.3638350431829332
+                ],
+                "i_to": [
+                    1.915559945597622,
+                    11092.99056448673,
+                    11092.6853310179
+                ],
+                "i_to_angle": [
+                    -2.0944020265392065,
+                    -0.3634940777761748,
+                    2.777928097798873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11093.238545275373,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.36359190742848624,
-                    2.778000746161307
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4217,30 +4543,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9811667515429,
+                    853.9270602593755,
+                    426.94592142748786
+                ],
+                "i_from_angle": [
+                    -0.3633236091478327,
+                    2.7780133379789755,
+                    -0.3638350431829332
+                ],
+                "i_to": [
+                    1.915559945597622,
+                    11092.99056448673,
+                    11092.6853310179
+                ],
+                "i_to_angle": [
+                    -2.0944020265392065,
+                    -0.3634940777761748,
+                    2.777928097798873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    42188.63202898906,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.2594547109415525,
-                    2.882137942648241
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4409,30 +4751,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.879878436319681,
                     -0.26175272566608415
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1380494549726,
+                    352.25809337319913,
+                    176.1200469236376
+                ],
+                "i_from_angle": [
+                    -0.24051718365704125,
+                    2.900944848556775,
+                    -0.2407784397607714
+                ],
+                "i_to": [
+                    0.42791224972473724,
+                    4576.044820833795,
+                    4575.888914337924
+                ],
+                "i_to_angle": [
+                    -2.1843705002037876,
+                    -0.2406042630907098,
+                    2.9009013051309362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    42188.63202898906,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.2594547109415525,
-                    2.882137942648241
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4601,30 +4959,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.879878436319681,
                     -0.26175272566608415
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1380494549726,
+                    352.25809337319913,
+                    176.1200469236376
+                ],
+                "i_from_angle": [
+                    -0.24051718365704125,
+                    2.900944848556775,
+                    -0.2407784397607714
+                ],
+                "i_to": [
+                    0.42791224972473724,
+                    4576.044820833795,
+                    4575.888914337924
+                ],
+                "i_to_angle": [
+                    -2.1843705002037876,
+                    -0.2406042630907098,
+                    2.9009013051309362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.685434751776,
-                    0.0,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.5255500163115527,
-                    0.0,
-                    -2.6160426372782406
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4793,30 +5167,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2558602935742,
+                    830.2562934194068,
+                    1660.5121389811572
+                ],
+                "i_from_angle": [
+                    -2.6161758428340303,
+                    -2.615909431791941,
+                    0.5255500163115525
+                ],
+                "i_to": [
+                    21570.683580525452,
+                    1.9155599455927432,
+                    21570.687331505225
+                ],
+                "i_to_angle": [
+                    0.5255056144671105,
+                    2.0943881782464553,
+                    -2.61599823544152
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.685434751776,
-                    0.0,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.5255500163115527,
-                    0.0,
-                    -2.6160426372782406
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4985,30 +5375,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2558602935742,
+                    830.2562934194068,
+                    1660.5121389811572
+                ],
+                "i_from_angle": [
+                    -2.6161758428340303,
+                    -2.615909431791941,
+                    0.5255500163115525
+                ],
+                "i_to": [
+                    21570.683580525452,
+                    1.9155599455927432,
+                    21570.687331505225
+                ],
+                "i_to_angle": [
+                    0.5255056144671105,
+                    2.0943881782464553,
+                    -2.61599823544152
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    47390.695245186966,
-                    0.0,
-                    47390.695245186966
-                ],
-                "i_angle": [
-                    0.6672788272903962,
-                    0.0,
-                    -2.474313826299397
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5177,30 +5583,46 @@
                 "i_angle": [
                     -2.3578339902539986,
                     -1.0213862822324478,
                     0.7838139402985298
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2538019564685,
+                    830.2583377536444,
+                    1660.5121389811575
+                ],
+                "i_from_angle": [
+                    -2.616072268231555,
+                    -2.6160130064868032,
+                    0.5255500163115527
+                ],
+                "i_to": [
+                    21570.66579522602,
+                    0.4279122497268866,
+                    21570.70507638185
+                ],
+                "i_to_angle": [
+                    0.5255401393450986,
+                    2.0044197045837953,
+                    -2.6160327603297726
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    47390.695245186966,
-                    0.0,
-                    47390.695245186966
-                ],
-                "i_angle": [
-                    0.6672788272903962,
-                    0.0,
-                    -2.474313826299397
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5369,30 +5791,46 @@
                 "i_angle": [
                     -2.3578339902539986,
                     -1.0213862822324478,
                     0.7838139402985298
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2538019564685,
+                    830.2583377536444,
+                    1660.5121389811575
+                ],
+                "i_from_angle": [
+                    -2.616072268231555,
+                    -2.6160130064868032,
+                    0.5255500163115527
+                ],
+                "i_to": [
+                    21570.66579522602,
+                    0.4279122497268866,
+                    21570.70507638185
+                ],
+                "i_to_angle": [
+                    0.5255401393450986,
+                    2.0044197045837953,
+                    -2.6160327603297726
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.206040025716,
-                    0.0,
-                    13383.206040025716
-                ],
-                "i_angle": [
-                    0.6443316120584346,
-                    0.0,
-                    -2.4972610415313587
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5561,30 +5999,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.0986078584966,
+                    515.1252505034938,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.4974692584873806,
+                    -2.4970429834131465,
+                    0.6443365381514847
+                ],
+                "i_to": [
+                    13382.884857651861,
+                    1.9155599455926484,
+                    13383.115589730434
+                ],
+                "i_to_angle": [
+                    0.6442654916924258,
+                    2.094388178245685,
+                    -2.4971850702041283
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.206040025716,
-                    0.0,
-                    13383.206040025716
-                ],
-                "i_angle": [
-                    0.6443316120584346,
-                    0.0,
-                    -2.4972610415313587
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5753,30 +6207,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.0986078584966,
+                    515.1252505034938,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.4974692584873806,
+                    -2.4970429834131465,
+                    0.6443365381514847
+                ],
+                "i_to": [
+                    13382.884857651861,
+                    1.9155599455926484,
+                    13383.115589730434
+                ],
+                "i_to_angle": [
+                    0.6442654916924258,
+                    2.094388178245685,
+                    -2.4971850702041283
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    123380.55909646388,
-                    0.0,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.6255521130910059,
-                    0.0,
-                    -2.5160405404987873
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5945,30 +6415,46 @@
                 "i_angle": [
                     -2.5183319784710787,
                     -1.021386282229902,
                     0.6232741810534576
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1067507054504,
+                    515.117085389314,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.4973030165679138,
+                    -2.4972092152496703,
+                    0.6443365381514848
+                ],
+                "i_to": [
+                    13382.9554410573,
+                    0.42791224973004227,
+                    13383.04494204505
+                ],
+                "i_to_angle": [
+                    0.6443209045461596,
+                    2.0044197045866436,
+                    -2.497240481937535
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    123380.55909646388,
-                    0.0,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.6255521130910059,
-                    0.0,
-                    -2.5160405404987873
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6137,30 +6623,46 @@
                 "i_angle": [
                     -2.5183319784710787,
                     -1.021386282229902,
                     0.6232741810534576
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1067507054504,
+                    515.117085389314,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.4973030165679138,
+                    -2.4972092152496703,
+                    0.6443365381514848
+                ],
+                "i_to": [
+                    13382.9554410573,
+                    0.42791224973004227,
+                    13383.04494204505
+                ],
+                "i_to_angle": [
+                    0.6443209045461596,
+                    2.0044197045866436,
+                    -2.497240481937535
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.592934905151,
-                    0.0,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.6751600728025443,
-                    0.0,
-                    -2.4664325807872487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6329,30 +6831,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.92616851643174,
+                    431.9595680697835,
+                    863.8857089150774
+                ],
+                "i_from_angle": [
+                    -2.4666746115496267,
+                    -2.4661684019783205,
+                    0.6751711566113577
+                ],
+                "i_to": [
+                    11222.05996392913,
+                    1.9155599455931536,
+                    11222.349212554143
+                ],
+                "i_to_angle": [
+                    0.675086787260702,
+                    2.0943881782460845,
+                    -2.466337129802344
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.592934905151,
-                    0.0,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.6751600728025443,
-                    0.0,
-                    -2.4664325807872487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6521,30 +7039,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.92616851643174,
+                    431.9595680697835,
+                    863.8857089150774
+                ],
+                "i_from_angle": [
+                    -2.4666746115496267,
+                    -2.4661684019783205,
+                    0.6751711566113577
+                ],
+                "i_to": [
+                    11222.05996392913,
+                    1.9155599455931536,
+                    11222.349212554143
+                ],
+                "i_to_angle": [
+                    0.675086787260702,
+                    2.0943881782460845,
+                    -2.466337129802344
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    44253.18100638276,
-                    0.0,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.7594081748628275,
-                    0.0,
-                    -2.3821844787269657
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6713,30 +7247,46 @@
                 "i_angle": [
                     -2.3844829909110485,
                     -1.0213862822329738,
                     0.7571466099407527
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7402869453105,
+                    184.7569784519952,
+                    369.49726247056475
+                ],
+                "i_from_angle": [
+                    -2.3635068673161914,
+                    -2.3632551393198096,
+                    0.7782116559575175
+                ],
+                "i_to": [
+                    4799.837966804531,
+                    0.4279122497283061,
+                    4799.982519493711
+                ],
+                "i_to_angle": [
+                    0.7781697006595861,
+                    2.00441970458408,
+                    -2.3633390435978385
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    44253.18100638276,
-                    0.0,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.7594081748628275,
-                    0.0,
-                    -2.3821844787269657
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6905,30 +7455,46 @@
                 "i_angle": [
                     -2.3844829909110485,
                     -1.0213862822329738,
                     0.7571466099407527
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7402869453105,
+                    184.7569784519952,
+                    369.49726247056475
+                ],
+                "i_from_angle": [
+                    -2.3635068673161914,
+                    -2.3632551393198096,
+                    0.7782116559575175
+                ],
+                "i_to": [
+                    4799.837966804531,
+                    0.4279122497283061,
+                    4799.982519493711
+                ],
+                "i_to_angle": [
+                    0.7781697006595861,
+                    2.00441970458408,
+                    -2.3633390435978385
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21151.16859553801,
-                    0.0,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.5447404949015825,
-                    0.0,
-                    -2.5968521586882107
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7097,30 +7663,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1052997407485,
+                    814.1099775899143,
+                    1628.215262313284
+                ],
+                "i_from_angle": [
+                    -2.596986468699668,
+                    -2.596714833439448,
+                    0.5447420029104378
+                ],
+                "i_to": [
+                    21151.116465887208,
+                    1.9155599455923331,
+                    21151.15697724967
+                ],
+                "i_to_angle": [
+                    0.544696730323465,
+                    2.094388178246826,
+                    -2.5968053781790945
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21151.16859553801,
-                    0.0,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.5447404949015825,
-                    0.0,
-                    -2.5968521586882107
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7289,30 +7871,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1052997407485,
+                    814.1099775899143,
+                    1628.215262313284
+                ],
+                "i_from_angle": [
+                    -2.596986468699668,
+                    -2.596714833439448,
+                    0.5447420029104378
+                ],
+                "i_to": [
+                    21151.116465887208,
+                    1.9155599455923331,
+                    21151.15697724967
+                ],
+                "i_to_angle": [
+                    0.544696730323465,
+                    2.094388178246826,
+                    -2.5968053781790945
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    45158.062107339065,
-                    0.0,
-                    45158.062107339065
-                ],
-                "i_angle": [
-                    0.702036731443955,
-                    0.0,
-                    -2.4395559221458383
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7481,30 +8079,46 @@
                 "i_angle": [
                     -2.323074890782218,
                     -1.0213862822337836,
                     0.8185752563982317
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.13796281269,
+                    791.1442057334048,
+                    1582.2821677869138
+                ],
+                "i_from_angle": [
+                    -2.5813150098424362,
+                    -2.581253054928446,
+                    0.5603086213265742
+                ],
+                "i_to": [
+                    20554.421267334794,
+                    0.4279122497263385,
+                    20554.475332614144
+                ],
+                "i_to_angle": [
+                    0.560298295493993,
+                    2.004419704592274,
+                    -2.5812737064577984
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    45158.062107339065,
-                    0.0,
-                    45158.062107339065
-                ],
-                "i_angle": [
-                    0.702036731443955,
-                    0.0,
-                    -2.4395559221458383
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7673,30 +8287,46 @@
                 "i_angle": [
                     -2.323074890782218,
                     -1.0213862822337836,
                     0.8185752563982317
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.13796281269,
+                    791.1442057334048,
+                    1582.2821677869138
+                ],
+                "i_from_angle": [
+                    -2.5813150098424362,
+                    -2.581253054928446,
+                    0.5603086213265742
+                ],
+                "i_to": [
+                    20554.421267334794,
+                    0.4279122497263385,
+                    20554.475332614144
+                ],
+                "i_to_angle": [
+                    0.560298295493993,
+                    2.004419704592274,
+                    -2.5812737064577984
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13203.668922039378,
-                    0.0,
-                    13203.668922039378
-                ],
-                "i_angle": [
-                    0.6548008225977684,
-                    0.0,
-                    -2.4867918309920247
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7865,30 +8495,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.1864122050829,
+                    508.21535250133576,
+                    1016.4017410507181
+                ],
+                "i_from_angle": [
+                    -2.487001152764607,
+                    -2.4865696533630843,
+                    0.6548072566690499
+                ],
+                "i_to": [
+                    13203.32064199255,
+                    1.9155599455950805,
+                    13203.571272315214
+                ],
+                "i_to_angle": [
+                    0.6547353394186225,
+                    2.0943881782469123,
+                    -2.4867134810354496
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13203.668922039378,
-                    0.0,
-                    13203.668922039378
-                ],
-                "i_angle": [
-                    0.6548008225977684,
-                    0.0,
-                    -2.4867918309920247
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8057,30 +8703,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.1864122050829,
+                    508.21535250133576,
+                    1016.4017410507181
+                ],
+                "i_from_angle": [
+                    -2.487001152764607,
+                    -2.4865696533630843,
+                    0.6548072566690499
+                ],
+                "i_to": [
+                    13203.32064199255,
+                    1.9155599455950805,
+                    13203.571272315214
+                ],
+                "i_to_angle": [
+                    0.6547353394186225,
+                    2.0943881782469123,
+                    -2.4867134810354496
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109432.87250368723,
-                    0.0,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.7145108901504922,
-                    0.0,
-                    -2.427081763439301
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8249,30 +8911,46 @@
                 "i_angle": [
                     -2.4293727039426445,
                     -1.0213862822318378,
                     0.712235016678194
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8719933354883,
+                    456.88657997429095,
+                    913.758572090266
+                ],
+                "i_from_angle": [
+                    -2.408345579109686,
+                    -2.4082422500273686,
+                    0.7332987398460042
+                ],
+                "i_to": [
+                    11870.008885100815,
+                    0.42791224973024056,
+                    11870.135209098553
+                ],
+                "i_to_angle": [
+                    0.7332815182406375,
+                    2.0044197045893153,
+                    -2.4082766923216976
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109432.87250368723,
-                    0.0,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.7145108901504922,
-                    0.0,
-                    -2.427081763439301
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8441,30 +9119,46 @@
                 "i_angle": [
                     -2.4293727039426445,
                     -1.0213862822318378,
                     0.712235016678194
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8719933354883,
+                    456.88657997429095,
+                    913.758572090266
+                ],
+                "i_from_angle": [
+                    -2.408345579109686,
+                    -2.4082422500273686,
+                    0.7332987398460042
+                ],
+                "i_to": [
+                    11870.008885100815,
+                    0.42791224973024056,
+                    11870.135209098553
+                ],
+                "i_to_angle": [
+                    0.7332815182406375,
+                    2.0044197045893153,
+                    -2.4082766923216976
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11093.238545275373,
-                    0.0,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.6836056437681111,
-                    0.0,
-                    -2.4579870098216823
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8633,30 +9327,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9459214274878,
+                    426.9811667515429,
+                    853.9270602593754
+                ],
+                "i_from_angle": [
+                    -2.4582301455761293,
+                    -2.4577187115410286,
+                    0.6836182355857796
+                ],
+                "i_to": [
+                    11092.685331017898,
+                    1.915559945597622,
+                    11092.99056448673
+                ],
+                "i_to_angle": [
+                    0.6835329954056775,
+                    2.094388178247184,
+                    -2.4578891801693707
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11093.238545275373,
-                    0.0,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.6836056437681111,
-                    0.0,
-                    -2.4579870098216823
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8825,30 +9535,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9459214274878,
+                    426.9811667515429,
+                    853.9270602593754
+                ],
+                "i_from_angle": [
+                    -2.4582301455761293,
+                    -2.4577187115410286,
+                    0.6836182355857796
+                ],
+                "i_to": [
+                    11092.685331017898,
+                    1.915559945597622,
+                    11092.99056448673
+                ],
+                "i_to_angle": [
+                    0.6835329954056775,
+                    2.094388178247184,
+                    -2.4578891801693707
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    42188.63202898906,
-                    0.0,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.7877428402550448,
-                    0.0,
-                    -2.3538498133347483
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9017,30 +9743,46 @@
                 "i_angle": [
                     -2.3561478280592802,
                     -1.0213862822329738,
                     0.7854833339264852
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1200469236376,
+                    176.1380494549726,
+                    352.25809337319913
+                ],
+                "i_from_angle": [
+                    -2.335173542153967,
+                    -2.334912286050237,
+                    0.8065497461635789
+                ],
+                "i_to": [
+                    4575.888914337924,
+                    0.4279122497247371,
+                    4576.044820833794
+                ],
+                "i_to_angle": [
+                    0.8065062027377404,
+                    2.004419704582603,
+                    -2.3349993654839056
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    42188.63202898906,
-                    0.0,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.7877428402550448,
-                    0.0,
-                    -2.3538498133347483
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9209,30 +9951,46 @@
                 "i_angle": [
                     -2.3561478280592802,
                     -1.0213862822329738,
                     0.7854833339264852
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1200469236376,
+                    176.1380494549726,
+                    352.25809337319913
+                ],
+                "i_from_angle": [
+                    -2.335173542153967,
+                    -2.334912286050237,
+                    0.8065497461635789
+                ],
+                "i_to": [
+                    4575.888914337924,
+                    0.4279122497247371,
+                    4576.044820833794
+                ],
+                "i_to_angle": [
+                    0.8065062027377404,
+                    2.004419704582603,
+                    -2.3349993654839056
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.685434751776,
-                    21570.685434751776,
-                    0.0
-                ],
-                "i_angle": [
-                    1.5727475675081506,
-                    -1.5688450860816425,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9401,30 +10159,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811575,
+                    830.255860293574,
+                    830.2562934194068
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    1.572614361952361,
+                    1.57288077299445
+                ],
+                "i_to": [
+                    21570.687331505225,
+                    21570.68358052545,
+                    1.9155599455927432
+                ],
+                "i_to_angle": [
+                    1.5727919693448715,
+                    -1.5688894879260848,
+                    -6.924146739943854e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.685434751776,
-                    21570.685434751776,
-                    0.0
-                ],
-                "i_angle": [
-                    1.5727475675081506,
-                    -1.5688450860816425,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9593,30 +10367,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811575,
+                    830.255860293574,
+                    830.2562934194068
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    1.572614361952361,
+                    1.57288077299445
+                ],
+                "i_to": [
+                    21570.687331505225,
+                    21570.68358052545,
+                    1.9155599455927432
+                ],
+                "i_to_angle": [
+                    1.5727919693448715,
+                    -1.5688894879260848,
+                    -6.924146739943854e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    47390.69524518697,
-                    47390.69524518697,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7144763784869943,
-                    -1.427116275102799,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9785,30 +10575,46 @@
                 "i_angle": [
                     -1.3105811620946655,
                     1.8309562145323925,
                     -3.115781384625643
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811577,
+                    830.2538019564684,
+                    830.2583377536444
+                ],
+                "i_from_angle": [
+                    -1.5688450860816425,
+                    1.5727179365548363,
+                    1.5727771982995882
+                ],
+                "i_to": [
+                    21570.70507638185,
+                    21570.665795226025,
+                    0.4279122497268865
+                ],
+                "i_to_angle": [
+                    1.5727574444566186,
+                    -1.5688549630480966,
+                    -0.08997539780939984
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    47390.69524518697,
-                    47390.69524518697,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7144763784869943,
-                    -1.427116275102799,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9977,30 +10783,46 @@
                 "i_angle": [
                     -1.3105811620946655,
                     1.8309562145323925,
                     -3.115781384625643
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811577,
+                    830.2538019564684,
+                    830.2583377536444
+                ],
+                "i_from_angle": [
+                    -1.5688450860816425,
+                    1.5727179365548363,
+                    1.5727771982995882
+                ],
+                "i_to": [
+                    21570.70507638185,
+                    21570.665795226025,
+                    0.4279122497268865
+                ],
+                "i_to_angle": [
+                    1.5727574444566186,
+                    -1.5688549630480966,
+                    -0.08997539780939984
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.206040025718,
-                    13383.206040025718,
-                    0.0
-                ],
-                "i_angle": [
-                    1.6915291632550324,
-                    -1.4500634903347607,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10169,30 +10991,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.223834961687,
+                    515.0986078584966,
+                    515.1252505034938
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6913209462990106,
+                    1.6917472213732445
+                ],
+                "i_to": [
+                    13383.115589730436,
+                    13382.88485765186,
+                    1.915559945592648
+                ],
+                "i_to_angle": [
+                    1.6916051345822627,
+                    -1.4501296107007695,
+                    -6.924147510500163e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.206040025718,
-                    13383.206040025718,
-                    0.0
-                ],
-                "i_angle": [
-                    1.6915291632550324,
-                    -1.4500634903347607,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10361,30 +11199,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.223834961687,
+                    515.0986078584966,
+                    515.1252505034938
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6913209462990106,
+                    1.6917472213732445
+                ],
+                "i_to": [
+                    13383.115589730436,
+                    13382.88485765186,
+                    1.915559945592648
+                ],
+                "i_to_angle": [
+                    1.6916051345822627,
+                    -1.4501296107007695,
+                    -6.924147510500163e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    123380.55909646388,
-                    123380.55909646388,
-                    0.0
-                ],
-                "i_angle": [
-                    1.6727496642876039,
-                    -1.4688429893021895,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10553,30 +11407,46 @@
                 "i_angle": [
                     -1.4711209213397376,
                     1.6704582263153125,
                     -3.1157813846230975
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    515.1067507054504,
+                    515.117085389314
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6914871882184774,
+                    1.6915809895367209
+                ],
+                "i_to": [
+                    13383.044942045051,
+                    13382.9554410573,
+                    0.4279122497300422
+                ],
+                "i_to_angle": [
+                    1.6915497228488563,
+                    -1.4500741978470355,
+                    -0.08997539780655145
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    123380.55909646388,
-                    123380.55909646388,
-                    0.0
-                ],
-                "i_angle": [
-                    1.6727496642876039,
-                    -1.4688429893021895,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10745,30 +11615,46 @@
                 "i_angle": [
                     -1.4711209213397376,
                     1.6704582263153125,
                     -3.1157813846230975
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    515.1067507054504,
+                    515.117085389314
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6914871882184774,
+                    1.6915809895367209
+                ],
+                "i_to": [
+                    13383.044942045051,
+                    13382.9554410573,
+                    0.4279122497300422
+                ],
+                "i_to_angle": [
+                    1.6915497228488563,
+                    -1.4500741978470355,
+                    -0.08997539780655145
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.592934905151,
-                    11222.592934905151,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7223576239991423,
-                    -1.419235029590651,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10937,30 +11823,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150773,
+                    431.9261685164318,
+                    431.9595680697836
+                ],
+                "i_from_angle": [
+                    -1.4192239457818376,
+                    1.7221155932367644,
+                    1.7226218028080706
+                ],
+                "i_to": [
+                    11222.349212554143,
+                    11222.059963929132,
+                    1.9155599455931536
+                ],
+                "i_to_angle": [
+                    1.722453074984047,
+                    -1.4193083151324932,
+                    -6.9241471108745026e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.592934905151,
-                    11222.592934905151,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7223576239991423,
-                    -1.419235029590651,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11129,30 +12031,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150773,
+                    431.9261685164318,
+                    431.9595680697836
+                ],
+                "i_from_angle": [
+                    -1.4192239457818376,
+                    1.7221155932367644,
+                    1.7226218028080706
+                ],
+                "i_to": [
+                    11222.349212554143,
+                    11222.059963929132,
+                    1.9155599455931536
+                ],
+                "i_to_angle": [
+                    1.722453074984047,
+                    -1.4193083151324932,
+                    -6.9241471108745026e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    44253.18100638276,
-                    44253.18100638276,
-                    0.0
-                ],
-                "i_angle": [
-                    1.8066057260594255,
-                    -1.3349869275303679,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11321,30 +12239,46 @@
                 "i_angle": [
                     -1.3372484924524426,
                     1.8043072138753427,
                     -3.115781384626169
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.49726247056475,
+                    184.74028694531046,
+                    184.75697845199517
+                ],
+                "i_from_angle": [
+                    -1.3161834464356779,
+                    1.8252833374701998,
+                    1.8255350654665816
+                ],
+                "i_to": [
+                    4799.982519493712,
+                    4799.837966804531,
+                    0.4279122497283061
+                ],
+                "i_to_angle": [
+                    1.8254511611885524,
+                    -1.3162254017336092,
+                    -0.08997539780911551
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    44253.18100638276,
-                    44253.18100638276,
-                    0.0
-                ],
-                "i_angle": [
-                    1.8066057260594255,
-                    -1.3349869275303679,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11513,30 +12447,46 @@
                 "i_angle": [
                     -1.3372484924524426,
                     1.8043072138753427,
                     -3.115781384626169
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.49726247056475,
+                    184.74028694531046,
+                    184.75697845199517
+                ],
+                "i_from_angle": [
+                    -1.3161834464356779,
+                    1.8252833374701998,
+                    1.8255350654665816
+                ],
+                "i_to": [
+                    4799.982519493712,
+                    4799.837966804531,
+                    0.4279122497283061
+                ],
+                "i_to_angle": [
+                    1.8254511611885524,
+                    -1.3162254017336092,
+                    -0.08997539780911551
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21151.16859553801,
-                    21151.16859553801,
-                    0.0
-                ],
-                "i_angle": [
-                    1.5919380460981805,
-                    -1.5496546074916127,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11705,30 +12655,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1628.2152623132843,
+                    814.1052997407484,
+                    814.1099775899143
+                ],
+                "i_from_angle": [
+                    -1.5496530994827575,
+                    1.591803736086723,
+                    1.592075371346943
+                ],
+                "i_to": [
+                    21151.156977249666,
+                    21151.116465887208,
+                    1.9155599455923331
+                ],
+                "i_to_angle": [
+                    1.591984826607297,
+                    -1.5496983720697304,
+                    -6.924146369013203e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21151.16859553801,
-                    21151.16859553801,
-                    0.0
-                ],
-                "i_angle": [
-                    1.5919380460981805,
-                    -1.5496546074916127,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11897,30 +12863,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1628.2152623132843,
+                    814.1052997407484,
+                    814.1099775899143
+                ],
+                "i_from_angle": [
+                    -1.5496530994827575,
+                    1.591803736086723,
+                    1.592075371346943
+                ],
+                "i_to": [
+                    21151.156977249666,
+                    21151.116465887208,
+                    1.9155599455923331
+                ],
+                "i_to_angle": [
+                    1.591984826607297,
+                    -1.5496983720697304,
+                    -6.924146369013203e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    45158.062107339065,
-                    45158.062107339065,
-                    0.0
-                ],
-                "i_angle": [
-                    1.749234282640553,
-                    -1.3923583709492404,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12089,30 +13071,46 @@
                 "i_angle": [
                     -1.2758198459949637,
                     1.8657153140041731,
                     -3.115781384626979
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1582.2821677869138,
+                    791.13796281269,
+                    791.1442057334048
+                ],
+                "i_from_angle": [
+                    -1.534086481066621,
+                    1.6074751949439552,
+                    1.6075371498579454
+                ],
+                "i_to": [
+                    20554.475332614144,
+                    20554.42126733479,
+                    0.42791224972633846
+                ],
+                "i_to_angle": [
+                    1.607516498328593,
+                    -1.5340968068992022,
+                    -0.0899753978009213
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    45158.062107339065,
-                    45158.062107339065,
-                    0.0
-                ],
-                "i_angle": [
-                    1.749234282640553,
-                    -1.3923583709492404,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12281,30 +13279,46 @@
                 "i_angle": [
                     -1.2758198459949637,
                     1.8657153140041731,
                     -3.115781384626979
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1582.2821677869138,
+                    791.13796281269,
+                    791.1442057334048
+                ],
+                "i_from_angle": [
+                    -1.534086481066621,
+                    1.6074751949439552,
+                    1.6075371498579454
+                ],
+                "i_to": [
+                    20554.475332614144,
+                    20554.42126733479,
+                    0.42791224972633846
+                ],
+                "i_to_angle": [
+                    1.607516498328593,
+                    -1.5340968068992022,
+                    -0.0899753978009213
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13203.66892203938,
-                    13203.66892203938,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7019983737943662,
-                    -1.4395942797954269,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12473,30 +13487,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1016.4017410507181,
+                    508.186412205083,
+                    508.21535250133576
+                ],
+                "i_from_angle": [
+                    -1.4395878457241453,
+                    1.7017890520217842,
+                    1.7022205514233069
+                ],
+                "i_to": [
+                    13203.571272315214,
+                    13203.320641992548,
+                    1.91555994559508
+                ],
+                "i_to_angle": [
+                    1.7020767237509413,
+                    -1.4396597629745729,
+                    -6.924146282928173e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13203.66892203938,
-                    13203.66892203938,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7019983737943662,
-                    -1.4395942797954269,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12665,30 +13695,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1016.4017410507181,
+                    508.186412205083,
+                    508.21535250133576
+                ],
+                "i_from_angle": [
+                    -1.4395878457241453,
+                    1.7017890520217842,
+                    1.7022205514233069
+                ],
+                "i_to": [
+                    13203.571272315214,
+                    13203.320641992548,
+                    1.91555994559508
+                ],
+                "i_to_angle": [
+                    1.7020767237509413,
+                    -1.4396597629745729,
+                    -6.924146282928173e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109432.87250368722,
-                    109432.87250368722,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7617084413470903,
-                    -1.379884212242703,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12857,30 +13903,46 @@
                 "i_angle": [
                     -1.3821600857150014,
                     1.7594175008437465,
                     -3.1157813846250333
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    913.7585720902658,
+                    456.87199333548836,
+                    456.886579974291
+                ],
+                "i_from_angle": [
+                    -1.361096362547191,
+                    1.7804446256767048,
+                    1.7805479547590226
+                ],
+                "i_to": [
+                    11870.135209098555,
+                    11870.008885100813,
+                    0.42791224973024067
+                ],
+                "i_to_angle": [
+                    1.7805135124646936,
+                    -1.361113584152558,
+                    -0.08997539780387981
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    109432.87250368722,
-                    109432.87250368722,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7617084413470903,
-                    -1.379884212242703,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13049,30 +14111,46 @@
                 "i_angle": [
                     -1.3821600857150014,
                     1.7594175008437465,
                     -3.1157813846250333
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    913.7585720902658,
+                    456.87199333548836,
+                    456.886579974291
+                ],
+                "i_from_angle": [
+                    -1.361096362547191,
+                    1.7804446256767048,
+                    1.7805479547590226
+                ],
+                "i_to": [
+                    11870.135209098555,
+                    11870.008885100813,
+                    0.42791224973024067
+                ],
+                "i_to_angle": [
+                    1.7805135124646936,
+                    -1.361113584152558,
+                    -0.08997539780387981
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11093.238545275373,
-                    11093.238545275373,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7308031949647091,
-                    -1.4107894586250842,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13241,30 +14319,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    853.9270602593755,
+                    426.94592142748786,
+                    426.98116675154284
+                ],
+                "i_from_angle": [
+                    -1.4107768668074157,
+                    1.7305600592102621,
+                    1.7310714932453626
+                ],
+                "i_to": [
+                    11092.990564486729,
+                    11092.685331017898,
+                    1.9155599455976215
+                ],
+                "i_to_angle": [
+                    1.7309010246170204,
+                    -1.4108621069875178,
+                    -6.924146011377819e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11093.238545275373,
-                    11093.238545275373,
-                    0.0
-                ],
-                "i_angle": [
-                    1.7308031949647091,
-                    -1.4107894586250842,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13433,30 +14527,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    853.9270602593755,
+                    426.94592142748786,
+                    426.98116675154284
+                ],
+                "i_from_angle": [
+                    -1.4107768668074157,
+                    1.7305600592102621,
+                    1.7310714932453626
+                ],
+                "i_to": [
+                    11092.990564486729,
+                    11092.685331017898,
+                    1.9155599455976215
+                ],
+                "i_to_angle": [
+                    1.7309010246170204,
+                    -1.4108621069875178,
+                    -6.924146011377819e-06
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    42188.63202898905,
-                    42188.63202898905,
-                    0.0
-                ],
-                "i_angle": [
-                    1.8349403914516427,
-                    -1.3066522621381504,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13625,30 +14735,46 @@
                 "i_angle": [
                     -1.3089117684667102,
                     1.8326423767271112,
                     -3.115781384626169
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    352.25809337319913,
+                    176.12004692363757,
+                    176.1380494549726
+                ],
+                "i_from_angle": [
+                    -1.2878453562296164,
+                    1.853616662632424,
+                    1.853877918736154
+                ],
+                "i_to": [
+                    4576.044820833795,
+                    4575.888914337923,
+                    0.4279122497247371
+                ],
+                "i_to_angle": [
+                    1.8537908393024856,
+                    -1.287888899655455,
+                    -0.08997539781059222
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    42188.63202898905,
-                    42188.63202898905,
-                    0.0
-                ],
-                "i_angle": [
-                    1.8349403914516427,
-                    -1.3066522621381504,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13817,30 +14943,46 @@
                 "i_angle": [
                     -1.3089117684667102,
                     1.8326423767271112,
                     -3.115781384626169
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    352.25809337319913,
+                    176.12004692363757,
+                    176.1380494549726
+                ],
+                "i_from_angle": [
+                    -1.2878453562296164,
+                    1.853616662632424,
+                    1.853877918736154
+                ],
+                "i_to": [
+                    4576.044820833795,
+                    4575.888914337923,
+                    0.4279122497247371
+                ],
+                "i_to_angle": [
+                    1.8537908393024856,
+                    -1.287888899655455,
+                    -0.08997539781059222
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.685434751776,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5216475348850447,
-                    2.6199451187047487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14009,30 +15151,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2562934194068,
+                    1660.5121389811575,
+                    830.2558602935742
+                ],
+                "i_from_angle": [
+                    -0.5215143293987453,
+                    2.6199451187047487,
+                    -0.5217807404408343
+                ],
+                "i_to": [
+                    1.9155599455927432,
+                    21570.68733150523,
+                    21570.68358052545
+                ],
+                "i_to_angle": [
+                    -2.0944020265399352,
+                    -0.5216031330483238,
+                    2.6199007168603066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.685434751776,
-                    21570.685434751776
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5216475348850447,
-                    2.6199451187047487
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14201,30 +15359,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2562934194068,
+                    1660.5121389811575,
+                    830.2558602935742
+                ],
+                "i_from_angle": [
+                    -0.5215143293987453,
+                    2.6199451187047487,
+                    -0.5217807404408343
+                ],
+                "i_to": [
+                    1.9155599455927432,
+                    21570.68733150523,
+                    21570.68358052545
+                ],
+                "i_to_angle": [
+                    -2.0944020265399352,
+                    -0.5216031330483238,
+                    2.6199007168603066
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    47390.69524518698,
-                    47390.69524518698
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3799187239062011,
-                    2.7616739296835924
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14393,30 +15567,46 @@
                 "i_angle": [
                     1.0730088201607482,
                     2.8782090426917257,
                     -0.2634388878608027
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2583377536442,
+                    1660.5121389811575,
+                    830.2538019564684
+                ],
+                "i_from_angle": [
+                    -0.5216179040936071,
+                    2.6199451187047487,
+                    -0.521677165838359
+                ],
+                "i_to": [
+                    0.4279122497268866,
+                    21570.705076381855,
+                    21570.665795226025
+                ],
+                "i_to_angle": [
+                    -2.1843705002025953,
+                    -0.5216376579365767,
+                    2.6199352417382946
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    47390.69524518698,
-                    47390.69524518698
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3799187239062011,
-                    2.7616739296835924
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14585,30 +15775,46 @@
                 "i_angle": [
                     1.0730088201607482,
                     2.8782090426917257,
                     -0.2634388878608027
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2583377536442,
+                    1660.5121389811575,
+                    830.2538019564684
+                ],
+                "i_from_angle": [
+                    -0.5216179040936071,
+                    2.6199451187047487,
+                    -0.521677165838359
+                ],
+                "i_to": [
+                    0.4279122497268866,
+                    21570.705076381855,
+                    21570.665795226025
+                ],
+                "i_to_angle": [
+                    -2.1843705002025953,
+                    -0.5216376579365767,
+                    2.6199352417382946
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13383.20604002572,
-                    13383.20604002572
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4028659391381628,
-                    2.7387267144516305
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14777,30 +15983,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1252505034938,
+                    1030.223834961687,
+                    515.0986078584967
+                ],
+                "i_from_angle": [
+                    -0.40264788101995064,
+                    2.7387316405446804,
+                    -0.40307415609418473
+                ],
+                "i_to": [
+                    1.9155599455926484,
+                    13383.115589730436,
+                    13382.884857651863
+                ],
+                "i_to_angle": [
+                    -2.0944020265407057,
+                    -0.4027899678109325,
+                    2.738660594085622
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13383.20604002572,
-                    13383.20604002572
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4028659391381628,
-                    2.7387267144516305
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14969,30 +16191,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1252505034938,
+                    1030.223834961687,
+                    515.0986078584967
+                ],
+                "i_from_angle": [
+                    -0.40264788101995064,
+                    2.7387316405446804,
+                    -0.40307415609418473
+                ],
+                "i_to": [
+                    1.9155599455926484,
+                    13383.115589730436,
+                    13382.884857651863
+                ],
+                "i_to_angle": [
+                    -2.0944020265407057,
+                    -0.4027899678109325,
+                    2.738660594085622
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    123380.55909646388,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4216454381055914,
-                    2.719947215484202
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15161,30 +16399,46 @@
                 "i_angle": [
                     1.073008820163294,
                     2.7176692834466536,
                     -0.4239368760778828
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.117085389314,
+                    1030.2238349616873,
+                    515.1067507054504
+                ],
+                "i_from_angle": [
+                    -0.40281411285647434,
+                    2.738731640544681,
+                    -0.4029079141747179
+                ],
+                "i_to": [
+                    0.4279122497300422,
+                    13383.044942045051,
+                    13382.955441057302
+                ],
+                "i_to_angle": [
+                    -2.184370500199747,
+                    -0.4028453795443391,
+                    2.7387160069393555
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    123380.55909646388,
-                    123380.55909646388
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4216454381055914,
-                    2.719947215484202
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15353,30 +16607,46 @@
                 "i_angle": [
                     1.073008820163294,
                     2.7176692834466536,
                     -0.4239368760778828
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.117085389314,
+                    1030.2238349616873,
+                    515.1067507054504
+                ],
+                "i_from_angle": [
+                    -0.40281411285647434,
+                    2.738731640544681,
+                    -0.4029079141747179
+                ],
+                "i_to": [
+                    0.4279122497300422,
+                    13383.044942045051,
+                    13382.955441057302
+                ],
+                "i_to_angle": [
+                    -2.184370500199747,
+                    -0.4028453795443391,
+                    2.7387160069393555
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11222.592934905151,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.372037478394053,
-                    2.76955517519574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15545,30 +16815,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.95956806978364,
+                    863.8857089150774,
+                    431.92616851643174
+                ],
+                "i_from_angle": [
+                    -0.37177329958512473,
+                    2.7695662590045536,
+                    -0.37227950915643077
+                ],
+                "i_to": [
+                    1.9155599455931536,
+                    11222.349212554145,
+                    11222.05996392913
+                ],
+                "i_to_angle": [
+                    -2.094402026540306,
+                    -0.37194202740914817,
+                    2.769481889653898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11222.592934905151,
-                    11222.592934905151
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.372037478394053,
-                    2.76955517519574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15737,30 +17023,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.95956806978364,
+                    863.8857089150774,
+                    431.92616851643174
+                ],
+                "i_from_angle": [
+                    -0.37177329958512473,
+                    2.7695662590045536,
+                    -0.37227950915643077
+                ],
+                "i_to": [
+                    1.9155599455931536,
+                    11222.349212554145,
+                    11222.05996392913
+                ],
+                "i_to_angle": [
+                    -2.094402026540306,
+                    -0.37194202740914817,
+                    2.769481889653898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    44253.18100638276,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.28778937633376983,
-                    2.8538032772560236
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15929,30 +17231,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.8515417123339484,
                     -0.29008788851785255
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7569784519952,
+                    369.49726247056475,
+                    184.74028694531052
+                ],
+                "i_from_angle": [
+                    -0.26886003692661353,
+                    2.872606758350713,
+                    -0.2691117649229955
+                ],
+                "i_to": [
+                    0.42791224972830616,
+                    4799.982519493712,
+                    4799.837966804531
+                ],
+                "i_to_angle": [
+                    -2.1843705002023106,
+                    -0.26894394120464277,
+                    2.872564803052782
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    44253.18100638276,
-                    44253.18100638276
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.28778937633376983,
-                    2.8538032772560236
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16121,30 +17439,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.8515417123339484,
                     -0.29008788851785255
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    184.7569784519952,
+                    369.49726247056475,
+                    184.74028694531052
+                ],
+                "i_from_angle": [
+                    -0.26886003692661353,
+                    2.872606758350713,
+                    -0.2691117649229955
+                ],
+                "i_to": [
+                    0.42791224972830616,
+                    4799.982519493712,
+                    4799.837966804531
+                ],
+                "i_to_angle": [
+                    -2.1843705002023106,
+                    -0.26894394120464277,
+                    2.872564803052782
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21151.16859553801,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5024570562950148,
-                    2.6391355972947785
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16313,30 +17647,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1099775899144,
+                    1628.2152623132843,
+                    814.1052997407485
+                ],
+                "i_from_angle": [
+                    -0.5023197310462522,
+                    2.6391371053036337,
+                    -0.5025913663064723
+                ],
+                "i_to": [
+                    1.9155599455923336,
+                    21151.156977249666,
+                    21151.116465887208
+                ],
+                "i_to_angle": [
+                    -2.0944020265395644,
+                    -0.5024102757858984,
+                    2.639091832716661
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21151.16859553801,
-                    21151.16859553801
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.5024570562950148,
-                    2.6391355972947785
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16505,30 +17855,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    814.1099775899144,
+                    1628.2152623132843,
+                    814.1052997407485
+                ],
+                "i_from_angle": [
+                    -0.5023197310462522,
+                    2.6391371053036337,
+                    -0.5025913663064723
+                ],
+                "i_to": [
+                    1.9155599455923336,
+                    21151.156977249666,
+                    21151.116465887208
+                ],
+                "i_to_angle": [
+                    -2.0944020265395644,
+                    -0.5024102757858984,
+                    2.639091832716661
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    45158.06210733907,
-                    45158.06210733907
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3451608197526424,
-                    2.796431833837151
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16697,30 +18063,46 @@
                 "i_angle": [
                     1.0730088201594121,
                     2.9129703587914277,
                     -0.22867978838902214
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.1442057334049,
+                    1582.2821677869138,
+                    791.13796281269
+                ],
+                "i_from_angle": [
+                    -0.48685795253524994,
+                    2.6547037237197704,
+                    -0.48691990744924013
+                ],
+                "i_to": [
+                    0.42791224972633846,
+                    20554.475332614144,
+                    20554.421267334797
+                ],
+                "i_to_angle": [
+                    -2.1843705001941167,
+                    -0.4868786040646023,
+                    2.654693397887189
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    45158.06210733907,
-                    45158.06210733907
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3451608197526424,
-                    2.796431833837151
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16889,30 +18271,46 @@
                 "i_angle": [
                     1.0730088201594121,
                     2.9129703587914277,
                     -0.22867978838902214
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    791.1442057334049,
+                    1582.2821677869138,
+                    791.13796281269
+                ],
+                "i_from_angle": [
+                    -0.48685795253524994,
+                    2.6547037237197704,
+                    -0.48691990744924013
+                ],
+                "i_to": [
+                    0.42791224972633846,
+                    20554.475332614144,
+                    20554.421267334797
+                ],
+                "i_to_angle": [
+                    -2.1843705001941167,
+                    -0.4868786040646023,
+                    2.654693397887189
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13203.66892203938,
-                    13203.66892203938
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.39239672859882896,
-                    2.749195924990964
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17081,30 +18479,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.21535250133576,
+                    1016.4017410507181,
+                    508.1864122050829
+                ],
+                "i_from_angle": [
+                    -0.39217455096988846,
+                    2.749202359062246,
+                    -0.39260605037141116
+                ],
+                "i_to": [
+                    1.91555994559508,
+                    13203.571272315212,
+                    13203.32064199255
+                ],
+                "i_to_angle": [
+                    -2.0944020265394783,
+                    -0.39231837864225394,
+                    2.7491304418118183
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    13203.66892203938,
-                    13203.66892203938
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.39239672859882896,
-                    2.749195924990964
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17273,30 +18687,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    508.21535250133576,
+                    1016.4017410507181,
+                    508.1864122050829
+                ],
+                "i_from_angle": [
+                    -0.39217455096988846,
+                    2.749202359062246,
+                    -0.39260605037141116
+                ],
+                "i_to": [
+                    1.91555994559508,
+                    13203.571272315212,
+                    13203.32064199255
+                ],
+                "i_to_angle": [
+                    -2.0944020265394783,
+                    -0.39231837864225394,
+                    2.7491304418118183
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    109432.87250368723,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3326866610461051,
-                    2.8089059925436883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17465,30 +18895,46 @@
                 "i_angle": [
                     1.0730088201613581,
                     2.80663011907139,
                     -0.33497760154944883
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8865799742911,
+                    913.758572090266,
+                    456.87199333548836
+                ],
+                "i_from_angle": [
+                    -0.3138471476341727,
+                    2.8276938422392,
+                    -0.3139504767164904
+                ],
+                "i_to": [
+                    0.4279122497302406,
+                    11870.135209098555,
+                    11870.008885100815
+                ],
+                "i_to_angle": [
+                    -2.1843705001970752,
+                    -0.3138815899285016,
+                    2.8276766206338335
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    109432.87250368723,
-                    109432.87250368723
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.3326866610461051,
-                    2.8089059925436883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17657,30 +19103,46 @@
                 "i_angle": [
                     1.0730088201613581,
                     2.80663011907139,
                     -0.33497760154944883
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    456.8865799742911,
+                    913.758572090266,
+                    456.87199333548836
+                ],
+                "i_from_angle": [
+                    -0.3138471476341727,
+                    2.8276938422392,
+                    -0.3139504767164904
+                ],
+                "i_to": [
+                    0.4279122497302406,
+                    11870.135209098555,
+                    11870.008885100815
+                ],
+                "i_to_angle": [
+                    -2.1843705001970752,
+                    -0.3138815899285016,
+                    2.8276766206338335
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11093.238545275373,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.36359190742848624,
-                    2.778000746161307
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17849,30 +19311,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9811667515429,
+                    853.9270602593755,
+                    426.94592142748786
+                ],
+                "i_from_angle": [
+                    -0.3633236091478327,
+                    2.7780133379789755,
+                    -0.3638350431829332
+                ],
+                "i_to": [
+                    1.915559945597622,
+                    11092.99056448673,
+                    11092.6853310179
+                ],
+                "i_to_angle": [
+                    -2.0944020265392065,
+                    -0.3634940777761748,
+                    2.777928097798873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    11093.238545275373,
-                    11093.238545275373
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.36359190742848624,
-                    2.778000746161307
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18041,30 +19519,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    426.9811667515429,
+                    853.9270602593755,
+                    426.94592142748786
+                ],
+                "i_from_angle": [
+                    -0.3633236091478327,
+                    2.7780133379789755,
+                    -0.3638350431829332
+                ],
+                "i_to": [
+                    1.915559945597622,
+                    11092.99056448673,
+                    11092.6853310179
+                ],
+                "i_to_angle": [
+                    -2.0944020265392065,
+                    -0.3634940777761748,
+                    2.777928097798873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    42188.63202898906,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.2594547109415525,
-                    2.882137942648241
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18233,30 +19727,46 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.879878436319681,
                     -0.26175272566608415
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1380494549726,
+                    352.25809337319913,
+                    176.1200469236376
+                ],
+                "i_from_angle": [
+                    -0.24051718365704125,
+                    2.900944848556775,
+                    -0.2407784397607714
+                ],
+                "i_to": [
+                    0.42791224972473724,
+                    4576.044820833795,
+                    4575.888914337924
+                ],
+                "i_to_angle": [
+                    -2.1843705002037876,
+                    -0.2406042630907098,
+                    2.9009013051309362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    42188.63202898906,
-                    42188.63202898906
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.2594547109415525,
-                    2.882137942648241
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18425,10 +19935,36 @@
                 "i_angle": [
                     1.0730088201602221,
                     2.879878436319681,
                     -0.26175272566608415
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    176.1380494549726,
+                    352.25809337319913,
+                    176.1200469236376
+                ],
+                "i_from_angle": [
+                    -0.24051718365704125,
+                    2.900944848556775,
+                    -0.2407784397607714
+                ],
+                "i_to": [
+                    0.42791224972473724,
+                    4576.044820833795,
+                    4575.888914337924
+                ],
+                "i_to_angle": [
+                    -2.1843705002037876,
+                    -0.2406042630907098,
+                    2.9009013051309362
+                ],
+                "id": 6
+            }
         ]
     }
 ]
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -2,16 +2,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -26,16 +26,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -50,16 +50,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -74,16 +74,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -98,16 +98,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -122,16 +122,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -146,16 +146,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -170,16 +170,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -194,16 +194,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -218,16 +218,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -242,16 +242,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -266,16 +266,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -578,16 +578,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -602,16 +602,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -626,16 +626,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -650,16 +650,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -674,16 +674,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -698,16 +698,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -722,16 +722,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -746,16 +746,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -770,16 +770,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -794,16 +794,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -818,16 +818,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -842,16 +842,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1154,16 +1154,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1178,16 +1178,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1202,16 +1202,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1226,16 +1226,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1250,16 +1250,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1274,16 +1274,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1298,16 +1298,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1322,16 +1322,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1346,16 +1346,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1370,16 +1370,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1394,16 +1394,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1418,16 +1418,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1730,16 +1730,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1754,16 +1754,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1778,16 +1778,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1802,16 +1802,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1826,16 +1826,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1850,16 +1850,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1874,16 +1874,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1898,16 +1898,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1922,16 +1922,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1946,16 +1946,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1970,16 +1970,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1994,16 +1994,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 2,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -12,36 +12,36 @@
     ],
     "line": [
         {
             "c0": 6.4e-07,
             "c1": 6.4e-07,
             "from_node": 1,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 7,
             "r0": 0.75,
             "r1": 0.049,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 2,
             "to_status": 1,
             "x0": 0.04,
             "x1": 0.153
         },
         {
             "c0": 3.2e-07,
             "c1": 3.2e-07,
             "from_node": 2,
             "from_status": 1,
-            "i_n": 660,
+            "i_n": 660.0,
             "id": 8,
             "r0": 0.375,
             "r1": 0.0245,
-            "tan0": 0,
-            "tan1": 0,
+            "tan0": 0.0,
+            "tan1": 0.0,
             "to_node": 3,
             "to_status": 1,
             "x0": 0.02,
             "x1": 0.0765
         }
     ],
     "node": [
@@ -61,60 +61,60 @@
             "id": 3,
             "u_rated": 10000.0
         }
     ],
     "shunt": [
         {
             "b0": 5.0,
-            "b1": 0,
-            "g0": 0,
-            "g1": 0,
+            "b1": 0.0,
+            "g0": 0.0,
+            "g1": 0.0,
             "id": 9,
             "node": 1,
             "status": 1
         }
     ],
     "source": [
         {
             "id": 4,
             "node": 0,
             "rx_ratio": 0.1,
             "sk": 20000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": 0.0,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         },
         {
             "id": 5,
             "node": 2,
             "rx_ratio": 0.1,
             "sk": 2000000000.0,
             "status": 1,
             "u_ref": 1.0,
             "u_ref_angle": -0.5235987755982988,
-            "z01_ratio": 1
+            "z01_ratio": 1.0
         }
     ],
     "transformer": [
         {
             "clock": 1,
             "from_node": 0,
             "from_status": 1,
-            "i0": 0,
+            "i0": 0.0,
             "id": 6,
-            "p0": 0,
-            "pk": 0,
+            "p0": 0.0,
+            "pk": 0.0,
             "sn": 20000000.0,
             "tap_max": 1,
             "tap_min": -1,
             "tap_nom": 0,
             "tap_pos": 0,
             "tap_side": 0,
-            "tap_size": 100,
+            "tap_size": 100.0,
             "to_node": 1,
             "to_status": 1,
             "u1": 150000.0,
             "u2": 10000.0,
             "uk": 0.05,
             "winding_from": 1,
             "winding_to": 2
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {'0': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer': [OrderedDict([('id', 6), "*

 * *      "('energized', 1), ('i_from', [830.2564162917024, 1660.5121389811572, 830.2557558382572]), "*

 * *      "('i_from_angle', [-0.5214477200550958, 2.6199451187047487, -0.5218473498739424]), ('i_to', "*

 * *      "[2.87343543512207, 21570.68834244531, 21570.682622750595]), ('i_to_angle', "*

 * *      '[-2.09443440527686, -0.5215809299232796, 2.619878513725322])])]}',*

 * * '1': "{'fault': {0: {delete: ['i', 'i_angle']}}, 'transformer' […]*

```diff
@@ -1,22 +1,12 @@
 [
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.3206228574046182e-12,
-                    21570.688435225937,
-                    21570.68252996795
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.5215809306262733,
-                    2.6198785144277434
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -185,30 +175,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2564162917024,
+                    1660.5121389811572,
+                    830.2557558382572
+                ],
+                "i_from_angle": [
+                    -0.5214477200550958,
+                    2.6199451187047487,
+                    -0.5218473498739424
+                ],
+                "i_to": [
+                    2.87343543512207,
+                    21570.68834244531,
+                    21570.682622750595
+                ],
+                "i_to_angle": [
+                    -2.09443440527686,
+                    -0.5215809299232796,
+                    2.619878513725322
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    69271.82833350313,
-                    69051.16112977838
-                ],
-                "i_angle": [
-                    1.5707963267948966,
-                    0.7271126129620479,
-                    1.3614652463434862
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -377,30 +383,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2666.5638579661513,
+                    1660.5121389811568,
+                    2658.0702723990444
+                ],
+                "i_from_angle": [
+                    0.7271482412599496,
+                    2.6199451187047487,
+                    -1.7801632650905403
+                ],
+                "i_to": [
+                    43813.09752763029,
+                    30826.59870747015,
+                    30661.10744675486
+                ],
+                "i_to_angle": [
+                    -2.0978273968474506,
+                    0.2687422722378037,
+                    1.824088604536336
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    53217.35452201774,
-                    41650.47799042057
-                ],
-                "i_angle": [
-                    -2.0344439357957027,
-                    -0.4176846057328116,
-                    2.809935148173772
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -569,30 +591,46 @@
                 "i_angle": [
                     2.284931919406314,
                     2.8088704601679817,
                     -0.16363568652730645
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    932.3386301325361,
+                    1660.5121389811575,
+                    729.6858726677895
+                ],
+                "i_from_angle": [
+                    -0.5593877059914143,
+                    2.6199451187047487,
+                    -0.4734186876830576
+                ],
+                "i_to": [
+                    1859.294711300958,
+                    22451.063945464975,
+                    20694.61660380312
+                ],
+                "i_to_angle": [
+                    2.2860686967899966,
+                    -0.5352175857970936,
+                    2.6346670022423195
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    70107.07595326328,
-                    40669.78106955473
-                ],
-                "i_angle": [
-                    0.0,
-                    0.019333635690193373,
-                    2.027334533720602
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -761,30 +799,46 @@
                 "i_angle": [
                     1.1919524581391756,
                     2.9410926853327095,
                     -0.3813771714481855
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1228.2532885847236,
+                    1660.5121389811575,
+                    712.5253245869044
+                ],
+                "i_from_angle": [
+                    -0.12237353847849994,
+                    2.6199451187047487,
+                    -1.2560282627683352
+                ],
+                "i_to": [
+                    9779.940162738505,
+                    24531.79733183281,
+                    19406.274106929406
+                ],
+                "i_to_angle": [
+                    -2.655488985127797,
+                    -0.3522771521886929,
+                    2.4052170268269526
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.10232039761827e-13,
-                    13383.37922600466,
-                    13383.033006054702
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4027593660822535,
-                    2.738620138638669
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -953,30 +1007,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1319296741964,
+                    1030.2238349616869,
+                    515.0919579442944
+                ],
+                "i_from_angle": [
+                    -0.4025413005641413,
+                    2.738731640544681,
+                    -0.40318075033614154
+                ],
+                "i_to": [
+                    2.8735126351761697,
+                    13383.173348594773,
+                    13382.827183243764
+                ],
+                "i_to_angle": [
+                    -2.0944183030712735,
+                    -0.40275443945836403,
+                    2.738625064201259
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.3206228574046182e-12,
-                    19456.22057196866,
-                    7419.839685663981
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.45856326690584037,
-                    2.885223564435842
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1145,30 +1215,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    748.8943902614443,
+                    1030.223834961687,
+                    285.5297376956408
+                ],
+                "i_from_angle": [
+                    -0.4584203635769466,
+                    2.7387316405446804,
+                    -0.25669362660345274
+                ],
+                "i_to": [
+                    4093.094131803336,
+                    15401.819741514097,
+                    11374.095419081752
+                ],
+                "i_to_angle": [
+                    2.5618304804945398,
+                    -0.4262468255608965,
+                    2.7704010995702513
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    139780.59033310143,
-                    139964.23210688512
-                ],
-                "i_angle": [
-                    1.1071487177940904,
-                    -0.9125042674064562,
-                    -3.0730804175665227
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1337,30 +1423,46 @@
                 "i_angle": [
                     1.166314152303894,
                     2.1940637548843576,
                     0.09966865249116195
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    583.5770569950439,
+                    1030.2238349616873,
+                    584.3374841752326
+                ],
+                "i_from_angle": [
+                    -0.8936917079295331,
+                    2.7387316405446804,
+                    0.08727429751409356
+                ],
+                "i_to": [
+                    4764.429165204173,
+                    13589.691960460563,
+                    13597.042076182825
+                ],
+                "i_to_angle": [
+                    1.1663683568941703,
+                    -0.5790669065889551,
+                    2.9148412855756898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    3.281856318094616e-11,
-                    142279.75500199184,
-                    137227.55916061436
-                ],
-                "i_angle": [
-                    -2.214297435588181,
-                    -0.9010292594747048,
-                    -3.0646188355296173
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1529,30 +1631,46 @@
                 "i_angle": [
                     0.6753029139001677,
                     2.1940637548843576,
                     0.09966865249116202
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    594.0115417309962,
+                    1030.2238349616875,
+                    572.9115267767704
+                ],
+                "i_from_angle": [
+                    -0.8822169013844455,
+                    2.7387316405446804,
+                    0.0957359459618152
+                ],
+                "i_to": [
+                    4749.68558162131,
+                    13693.595508900993,
+                    13489.795653281992
+                ],
+                "i_to_angle": [
+                    1.2115263018392826,
+                    -0.5770023428263538,
+                    2.9155313915124452
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.051160198809135e-12,
-                    11222.810134708174,
-                    11222.375914852377
-                ],
-                "i_angle": [
-                    0.9272952180016122,
-                    -0.3719109232686938,
-                    2.769428615173669
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1721,30 +1839,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.9679440839958,
+                    863.8857089150778,
+                    431.9178270987636
+                ],
+                "i_from_angle": [
+                    -0.37164673620170424,
+                    2.769566259004554,
+                    -0.37240609702190974
+                ],
+                "i_to": [
+                    2.8735348948440262,
+                    11222.421651103217,
+                    11221.98762525169
+                ],
+                "i_to_angle": [
+                    -2.0944454946764344,
+                    -0.3718998368909085,
+                    2.769439696415429
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.6914300309505968e-12,
-                    15221.049096159133,
-                    7319.189126557197
-                ],
-                "i_angle": [
-                    -1.3258176636680326,
-                    -0.43565879540352337,
-                    2.9021616734947613
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -1913,30 +2047,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    585.8699053462921,
+                    863.8857089150774,
+                    281.6548538632998
+                ],
+                "i_from_angle": [
+                    -0.4354724173500512,
+                    2.7695662590045536,
+                    -0.23975557134706554
+                ],
+                "i_to": [
+                    2722.7856230718176,
+                    12549.167317231457,
+                    9904.591373024126
+                ],
+                "i_to_angle": [
+                    2.5310113393583893,
+                    -0.3976640015037856,
+                    2.802051391398511
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    54337.52726293892,
-                    35029.46911581169
-                ],
-                "i_angle": [
-                    3.141592653589793,
-                    -0.3991275841003275,
-                    3.0270188022642905
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2105,30 +2255,46 @@
                 "i_angle": [
                     2.316186192092367,
                     2.7332887981206406,
                     -0.09927091306014796
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    226.8571813463364,
+                    369.49726247056475,
+                    146.22739049170715
+                ],
+                "i_from_angle": [
+                    -0.38022969558102043,
+                    2.8726067583507136,
+                    -0.09589497606511535
+                ],
+                "i_to": [
+                    829.0823516211838,
+                    5157.05123355352,
+                    4452.728146974395
+                ],
+                "i_to_angle": [
+                    2.3185603847912475,
+                    -0.3112908241912653,
+                    2.921608385302007
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    54275.891073526356,
-                    35070.439826480135
-                ],
-                "i_angle": [
-                    2.0344439357957027,
-                    -0.3979255201256691,
-                    3.0247395718627565
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2297,30 +2463,46 @@
                 "i_angle": [
                     1.7834741527734312,
                     2.725152269512906,
                     -0.08944292119606981
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    226.59987612074252,
+                    369.4972624705649,
+                    146.39848076800456
+                ],
+                "i_from_angle": [
+                    -0.37902745155240836,
+                    2.872606758350713,
+                    -0.0981744743993842
+                ],
+                "i_to": [
+                    823.0345262346136,
+                    5154.989911419625,
+                    4454.553684974288
+                ],
+                "i_to_angle": [
+                    2.3214189975885615,
+                    -0.3108044432994101,
+                    2.9210056647994227
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.688448254623,
-                    21570.682516940993
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.521580930024967,
-                    2.6198785138263565
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2489,30 +2671,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2564167932821,
+                    1660.512138981157,
+                    830.2557553368771
+                ],
+                "i_from_angle": [
+                    -0.5214477194538237,
+                    2.6199451187047487,
+                    -0.5218473504754563
+                ],
+                "i_to": [
+                    2.8734441007062768,
+                    21570.68834678855,
+                    21570.68261840794
+                ],
+                "i_to_angle": [
+                    -2.094437422093706,
+                    -0.5215809297228285,
+                    2.619878513524845
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8564982859236946e-11,
-                    105344.74178499488,
-                    80715.25872943088
-                ],
-                "i_angle": [
-                    -0.7853981633974483,
-                    0.26117391563424647,
-                    0.6476915951933747
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2681,30 +2879,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    4055.0658129596454,
+                    1660.512138981158,
+                    3107.097406011981
+                ],
+                "i_from_angle": [
+                    0.2612041894677123,
+                    2.619945118704749,
+                    -2.4939062964829706
+                ],
+                "i_to": [
+                    60892.07184358473,
+                    46433.55279199729,
+                    25068.632233629523
+                ],
+                "i_to_angle": [
+                    -2.713041756840427,
+                    0.040996403969297296,
+                    1.2039694438565582
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.6412457148092364e-12,
-                    52909.12709036595,
-                    41964.98798893011
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.41929341803740017,
-                    2.8113248055280535
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -2873,30 +3087,46 @@
                 "i_angle": [
                     2.2556470550879726,
                     2.80703192735931,
                     -0.16313188957968786
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    926.9385402759627,
+                    1660.5121389811577,
+                    735.1959590214595
+                ],
+                "i_from_angle": [
+                    -0.560996381759432,
+                    2.6199451187047487,
+                    -0.47202876628344714
+                ],
+                "i_to": [
+                    1778.1116567243553,
+                    22403.99207308366,
+                    20742.00858092387
+                ],
+                "i_to_angle": [
+                    2.256817534624353,
+                    -0.535743359093768,
+                    2.635170475295638
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    76734.0685122063,
-                    31184.17013909327
-                ],
-                "i_angle": [
-                    -1.5707963267948966,
-                    -0.08060001265062024,
-                    1.9498012854290918
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3065,30 +3295,46 @@
                 "i_angle": [
                     0.9016901113897194,
                     2.871212698724256,
                     -0.2493234515842721
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1344.3533014954266,
+                    1660.5121389811577,
+                    546.3425489709848
+                ],
+                "i_from_angle": [
+                    -0.22230936603975465,
+                    2.6199451187047487,
+                    -1.333572968265203
+                ],
+                "i_to": [
+                    10443.603531869712,
+                    25735.213052947638,
+                    17967.252898950905
+                ],
+                "i_to_angle": [
+                    -2.945774800199253,
+                    -0.38784329683887153,
+                    2.4276810032042873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.209167143284393e-12,
-                    13383.379240478609,
-                    13383.032991583173
-                ],
-                "i_angle": [
-                    0.3805063771123649,
-                    -0.4027593652351362,
-                    2.7386201377912993
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3257,30 +3503,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1319302314585,
+                    1030.2238349616869,
+                    515.0919573873116
+                ],
+                "i_from_angle": [
+                    -0.40254129971718866,
+                    2.738731640544681,
+                    -0.4031807511838516
+                ],
+                "i_to": [
+                    2.873521302497315,
+                    13383.173353419996,
+                    13382.82717841934
+                ],
+                "i_to_angle": [
+                    -2.0944213198034936,
+                    -0.40275443917596215,
+                    2.738625063918773
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.594535229648264e-12,
-                    19186.031320276208,
-                    7721.228567385602
-                ],
-                "i_angle": [
-                    -1.892546881191539,
-                    -0.46765951038175707,
-                    2.9003181808877447
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3449,30 +3711,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    738.4926421496681,
+                    1030.2238349616864,
+                    297.13010400412185
+                ],
+                "i_from_angle": [
+                    -0.4675151560525329,
+                    2.7387316405446804,
+                    -0.24158208382348295
+                ],
+                "i_to": [
+                    3930.2119437719102,
+                    15309.748772985855,
+                    11469.274765045517
+                ],
+                "i_to_angle": [
+                    2.5268769184284054,
+                    -0.4298542662960204,
+                    2.774766977765362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8564982859236946e-11,
-                    140755.17391308167,
-                    120361.0200184777
-                ],
-                "i_angle": [
-                    -2.356194490192345,
-                    -0.7287218114926687,
-                    3.081247295959588
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3641,30 +3919,46 @@
                 "i_angle": [
                     1.4161400248092457,
                     2.3896737696059263,
                     -0.03326427683205201
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    587.6500026354183,
+                    1030.2238349616875,
+                    502.4936290101132
+                ],
+                "i_from_angle": [
+                    -0.7099036673031583,
+                    2.7387316405446804,
+                    -0.041592697636606675
+                ],
+                "i_to": [
+                    3173.7626974518193,
+                    13858.808131235688,
+                    13083.547308663361
+                ],
+                "i_to_angle": [
+                    1.4163640952989984,
+                    -0.5140783400883304,
+                    2.856568912059332
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.640928159047308e-11,
-                    141595.5411089959,
-                    119077.38838665358
-                ],
-                "i_angle": [
-                    -2.214297435588181,
-                    -0.7215735305347325,
-                    3.078930942971697
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -3833,30 +4127,46 @@
                 "i_angle": [
                     0.9086888510252009,
                     2.3884070286142562,
                     -0.036560207819890736
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    591.1587840230852,
+                    1030.223834961687,
+                    497.13437207662156
+                ],
+                "i_from_angle": [
+                    -0.7027554214418821,
+                    2.7387316405446804,
+                    -0.043909448750795034
+                ],
+                "i_to": [
+                    3144.7746365857574,
+                    13895.639061055148,
+                    13040.912813484474
+                ],
+                "i_to_angle": [
+                    1.4449905517334045,
+                    -0.5119187270628048,
+                    2.854968561365265
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.784086579150955e-12,
-                    11222.810149527175,
-                    11222.375900036135
-                ],
-                "i_angle": [
-                    1.0303768265243125,
-                    -0.37191092229892897,
-                    2.769428614203532
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4025,30 +4335,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.96794465455815,
+                    863.8857089150774,
+                    431.91782652851936
+                ],
+                "i_from_angle": [
+                    -0.37164673523219915,
+                    2.7695662590045536,
+                    -0.3724060979925305
+                ],
+                "i_to": [
+                    2.87354356134246,
+                    11222.421656043509,
+                    11221.987620312308
+                ],
+                "i_to_angle": [
+                    -2.094448511905002,
+                    -0.3718998365676162,
+                    2.7694396960920127
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8346134549116837e-12,
-                    15094.372232082715,
-                    7457.205399444285
-                ],
-                "i_angle": [
-                    0.4636476090008061,
-                    -0.44024268587885335,
-                    2.907945862380652
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4217,30 +4543,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    580.9930367507461,
+                    863.8857089150778,
+                    286.967185716652
+                ],
+                "i_from_angle": [
+                    -0.4400550763526473,
+                    2.7695662590045536,
+                    -0.23396371610485434
+                ],
+                "i_to": [
+                    2648.220593071964,
+                    12506.056596594462,
+                    9948.91121708362
+                ],
+                "i_to_angle": [
+                    2.508298021625174,
+                    -0.3993785999238423,
+                    2.803951226001291
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.0378140918593056e-11,
-                    53265.51917144258,
-                    36054.19841843337
-                ],
-                "i_angle": [
-                    -2.819842099193151,
-                    -0.3987534505718982,
-                    3.018141161687509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4409,30 +4751,46 @@
                 "i_angle": [
                     2.2739724098831577,
                     2.7335061443913737,
                     -0.10953709248225307
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    222.3814360766278,
+                    369.49726247056464,
+                    150.50588058113135
+                ],
+                "i_from_angle": [
+                    -0.37985312335630084,
+                    2.872606758350713,
+                    -0.10477126433307281
+                ],
+                "i_to": [
+                    759.0859352916882,
+                    5118.433159278243,
+                    4490.882354955285
+                ],
+                "i_to_angle": [
+                    2.2765162135393298,
+                    -0.31062781864822797,
+                    2.920071782017483
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    9.282491429618473e-12,
-                    53218.61411708044,
-                    36083.42218905788
-                ],
-                "i_angle": [
-                    -2.356194490192345,
-                    -0.39764655902623164,
-                    3.0162164988477635
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4601,30 +4959,46 @@
                 "i_angle": [
                     1.7413916314667608,
                     2.7260349625196,
                     -0.10097797014853996
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    222.18563241353277,
+                    369.49726247056475,
+                    150.62792134061246
+                ],
+                "i_from_angle": [
+                    -0.3787460829173903,
+                    2.872606758350713,
+                    -0.10669616122505124
+                ],
+                "i_to": [
+                    754.1000383014048,
+                    5116.888168807475,
+                    4492.222780013275
+                ],
+                "i_to_angle": [
+                    2.2794145833626884,
+                    -0.31018957943673703,
+                    2.9195439685912445
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.682529967948,
-                    2.3206228574046182e-12,
-                    21570.688435225933
-                ],
-                "i_angle": [
-                    0.5254834120345475,
-                    -1.3089969389957476,
-                    -2.6159760330194692
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4793,30 +5167,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2557558382572,
+                    830.2564162917024,
+                    1660.512138981157
+                ],
+                "i_from_angle": [
+                    -2.6162424522671386,
+                    -2.6158428224482915,
+                    0.5255500163115526
+                ],
+                "i_to": [
+                    21570.68262275059,
+                    2.8734354351220692,
+                    21570.688342445308
+                ],
+                "i_to_angle": [
+                    0.5254834113321264,
+                    2.0943557995095303,
+                    -2.6159760323164756
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    69051.16112977837,
-                    6.5637126361892306e-12,
-                    69271.82833350312
-                ],
-                "i_angle": [
-                    -0.7329298560497098,
-                    -0.5235987755982993,
-                    -1.367282489431148
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -4985,30 +5375,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2658.070272399044,
+                    2666.563857966151,
+                    1660.5121389811568
+                ],
+                "i_from_angle": [
+                    2.4086269396958504,
+                    -1.3672468611332462,
+                    0.525550016311553
+                ],
+                "i_to": [
+                    30661.10744675486,
+                    43813.097527630285,
+                    30826.59870747015
+                ],
+                "i_to_angle": [
+                    -0.2703064978568599,
+                    2.09096280793894,
+                    -1.8256528301553923
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    41650.47799042057,
-                    7.338453819646735e-12,
-                    53217.35452201773
-                ],
-                "i_angle": [
-                    0.7155400457805761,
-                    2.154346268990688,
-                    -2.5120797081260076
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5177,30 +5583,46 @@
                 "i_angle": [
                     -2.2580307889205025,
                     0.19053681701311823,
                     0.714475357774786
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    729.6858726677895,
+                    932.3386301325361,
+                    1660.5121389811572
+                ],
+                "i_from_angle": [
+                    -2.5678137900762534,
+                    -2.65378280838461,
+                    0.5255500163115526
+                ],
+                "i_to": [
+                    20694.616603803122,
+                    1859.2947113009575,
+                    22451.063945464975
+                ],
+                "i_to_angle": [
+                    0.5402718998491237,
+                    0.19167359439680046,
+                    -2.6296126881902895
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    40669.78106955473,
-                    6.5637126361892306e-12,
-                    70107.07595326328
-                ],
-                "i_angle": [
-                    -0.06706056867259368,
-                    -2.0943951023931957,
-                    -2.0750614667030023
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5369,30 +5791,46 @@
                 "i_angle": [
                     -2.475772273841381,
                     -0.9024426442540203,
                     0.8466975829395137
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    712.5253245869043,
+                    1228.2532885847234,
+                    1660.5121389811572
+                ],
+                "i_from_angle": [
+                    2.9327619420180553,
+                    -2.216768640871696,
+                    0.5255500163115526
+                ],
+                "i_to": [
+                    19406.274106929402,
+                    9779.940162738505,
+                    24531.797331832808
+                ],
+                "i_to_angle": [
+                    0.3108219244337565,
+                    1.5333012196585933,
+                    -2.446672254581889
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.033006054702,
-                    4.102320397618269e-13,
-                    13383.379226004661
-                ],
-                "i_angle": [
-                    0.6442250362454732,
-                    -2.0943951023931957,
-                    -2.4971544684754496
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5561,30 +5999,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.0919579442944,
+                    515.1319296741963,
+                    1030.2238349616866
+                ],
+                "i_from_angle": [
+                    -2.4975758527293372,
+                    -2.496936402957337,
+                    0.6443365381514848
+                ],
+                "i_to": [
+                    13382.827183243762,
+                    2.8735126351761693,
+                    13383.173348594773
+                ],
+                "i_to_angle": [
+                    0.644229961808063,
+                    2.094371901715117,
+                    -2.49714954185156
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7419.839685663981,
-                    2.3206228574046182e-12,
-                    19456.220571968657
-                ],
-                "i_angle": [
-                    0.7908284620426462,
-                    -1.3089969389957476,
-                    -2.552958369299036
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5753,30 +6207,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    285.5297376956408,
+                    748.8943902614442,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.3510887289966487,
+                    -2.5528154659701423,
+                    0.6443365381514846
+                ],
+                "i_to": [
+                    11374.09541908175,
+                    4093.094131803336,
+                    15401.819741514097
+                ],
+                "i_to_angle": [
+                    0.6760059971770553,
+                    0.4674353781013438,
+                    -2.5206419279540926
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    139964.23210688512,
-                    7.338453819646735e-12,
-                    139780.59033310143
-                ],
-                "i_angle": [
-                    1.1157097872198676,
-                    -0.9872463845991054,
-                    -3.006899369799652
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -5945,30 +6415,46 @@
                 "i_angle": [
                     -1.994726449902034,
                     -0.928080950089302,
                     0.09966865249116147
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    584.3374841752325,
+                    583.5770569950439,
+                    1030.2238349616873
+                ],
+                "i_from_angle": [
+                    -2.0071208048791025,
+                    -2.988086810322729,
+                    0.6443365381514846
+                ],
+                "i_to": [
+                    13597.042076182825,
+                    4764.429165204173,
+                    13589.691960460561
+                ],
+                "i_to_angle": [
+                    0.820446183182494,
+                    -0.9280267454990259,
+                    -2.6734620089821513
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    137227.55916061433,
-                    3.2818563180946154e-11,
-                    142279.75500199184
-                ],
-                "i_angle": [
-                    1.1241713692567732,
-                    1.9744927691982097,
-                    -2.995424361867901
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6137,30 +6623,46 @@
                 "i_angle": [
                     -1.9947264499020338,
                     -1.4190921884930283,
                     0.09966865249116152
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    572.9115267767704,
+                    594.0115417309961,
+                    1030.2238349616873
+                ],
+                "i_from_angle": [
+                    -1.9986591564313807,
+                    -2.9766120037776416,
+                    0.6443365381514845
+                ],
+                "i_to": [
+                    13489.795653281992,
+                    4749.685581621309,
+                    13693.595508900991
+                ],
+                "i_to_angle": [
+                    0.8211362891192492,
+                    -0.8828688005539135,
+                    -2.6713974452195495
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.375914852377,
-                    2.0511601988091346e-12,
-                    11222.810134708174
-                ],
-                "i_angle": [
-                    0.6750335127804729,
-                    -1.1670998843915836,
-                    -2.46630602566189
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6329,30 +6831,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.9178270987636,
+                    431.96794408399575,
+                    863.8857089150777
+                ],
+                "i_from_angle": [
+                    -2.4668011994151056,
+                    -2.4660418385949003,
+                    0.6751711566113578
+                ],
+                "i_to": [
+                    11221.98762525169,
+                    2.8735348948440262,
+                    11222.421651103217
+                ],
+                "i_to_angle": [
+                    0.6750445940222332,
+                    2.094344710109956,
+                    -2.4662949392841043
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7319.189126557197,
-                    1.6914300309505968e-12,
-                    15221.049096159133
-                ],
-                "i_angle": [
-                    0.8077665711015652,
-                    2.862972541118358,
-                    -2.5300538977967193
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6521,30 +7039,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    281.6548538632998,
+                    585.8699053462921,
+                    863.8857089150777
+                ],
+                "i_from_angle": [
+                    -2.3341506737402615,
+                    -2.529867519743247,
+                    0.6751711566113576
+                ],
+                "i_to": [
+                    9904.591373024126,
+                    2722.785623071817,
+                    12549.167317231457
+                ],
+                "i_to_angle": [
+                    0.7076562890053153,
+                    0.43661623696519325,
+                    -2.4920591038969815
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35029.46911581169,
-                    6.5637126361892306e-12,
-                    54337.52726293892
-                ],
-                "i_angle": [
-                    0.9326236998710947,
-                    1.0471975511965974,
-                    -2.4935226864935234
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6713,30 +7247,46 @@
                 "i_angle": [
                     -2.193666015453344,
                     0.22179108969917102,
                     0.6388936957274449
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    146.22739049170715,
+                    226.85718134633638,
+                    369.49726247056475
+                ],
+                "i_from_angle": [
+                    -2.190290078458311,
+                    -2.4746247979742164,
+                    0.7782116559575175
+                ],
+                "i_to": [
+                    4452.728146974394,
+                    829.0823516211839,
+                    5157.051233553519
+                ],
+                "i_to_angle": [
+                    0.8272132829088112,
+                    0.22416528239805164,
+                    -2.4056859265844612
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    35070.43982648012,
-                    7.338453819646735e-12,
-                    54275.89107352634
-                ],
-                "i_angle": [
-                    0.9303444694695607,
-                    -0.05995116659749318,
-                    -2.492320622518865
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -6905,30 +7455,46 @@
                 "i_angle": [
                     -2.183838023589266,
                     -0.31092094961976474,
                     0.6307571671197096
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    146.39848076800456,
+                    226.59987612074252,
+                    369.4972624705648
+                ],
+                "i_from_angle": [
+                    -2.19256957679258,
+                    -2.4734225539456043,
+                    0.7782116559575171
+                ],
+                "i_to": [
+                    4454.5536849742875,
+                    823.0345262346136,
+                    5154.989911419624
+                ],
+                "i_to_angle": [
+                    0.826610562406227,
+                    0.22702389519536564,
+                    -2.405199545692606
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.68251694099,
-                    0.0,
-                    21570.688448254623
-                ],
-                "i_angle": [
-                    0.5254834114331608,
-                    0.0,
-                    -2.6159760324181627
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7097,30 +7663,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2557553368771,
+                    830.2564167932821,
+                    1660.5121389811572
+                ],
+                "i_from_angle": [
+                    -2.616242452868652,
+                    -2.6158428218470196,
+                    0.5255500163115527
+                ],
+                "i_to": [
+                    21570.68261840794,
+                    2.873444100706276,
+                    21570.68834678855
+                ],
+                "i_to_angle": [
+                    0.5254834111316489,
+                    2.0943527826926847,
+                    -2.6159760321160244
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    80715.25872943089,
-                    1.8564982859236946e-11,
-                    105344.74178499487
-                ],
-                "i_angle": [
-                    -1.446703507199821,
-                    -2.8797932657906444,
-                    -1.8332211867589494
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7289,30 +7871,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    3107.0974060119806,
+                    4055.0658129596454,
+                    1660.512138981158
+                ],
+                "i_from_angle": [
+                    1.6948839083034202,
+                    -1.8331909129254835,
+                    0.5255500163115531
+                ],
+                "i_to": [
+                    25068.63223362952,
+                    60892.07184358473,
+                    46433.55279199728
+                ],
+                "i_to_angle": [
+                    -0.8904256585366377,
+                    1.4757484479459637,
+                    -2.0533986984238988
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    41964.9879889301,
-                    4.6412457148092364e-12,
-                    52909.12709036596
-                ],
-                "i_angle": [
-                    0.7169297031348577,
-                    -1.3089969389957476,
-                    -2.513688520430596
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7481,30 +8079,46 @@
                 "i_angle": [
                     -2.2575269919728838,
                     0.1612519526947766,
                     0.7126368249661141
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    735.1959590214594,
+                    926.9385402759626,
+                    1660.5121389811575
+                ],
+                "i_from_angle": [
+                    -2.566423868676643,
+                    -2.655391484152628,
+                    0.5255500163115526
+                ],
+                "i_to": [
+                    20742.008580923866,
+                    1778.1116567243555,
+                    22403.99207308366
+                ],
+                "i_to_angle": [
+                    0.5407753729024419,
+                    0.1624224322311571,
+                    -2.630138461486964
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    31184.17013909326,
-                    6.5637126361892306e-12,
-                    76734.0685122063
-                ],
-                "i_angle": [
-                    -0.14459381696410417,
-                    2.617993877991494,
-                    -2.1749951150438163
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7673,30 +8287,46 @@
                 "i_angle": [
                     -2.343718553977468,
                     -1.1927049910034764,
                     0.7768175963310602
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    546.3425489709848,
+                    1344.3533014954266,
+                    1660.5121389811577
+                ],
+                "i_from_angle": [
+                    2.8552172365211876,
+                    -2.3167044684329503,
+                    0.5255500163115527
+                ],
+                "i_to": [
+                    17967.252898950905,
+                    10443.603531869709,
+                    25735.213052947634
+                ],
+                "i_to_angle": [
+                    0.3332859008110913,
+                    1.2430154045871373,
+                    -2.4822383992320676
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.032991583172,
-                    2.2091671432843936e-12,
-                    13383.379240478607
-                ],
-                "i_angle": [
-                    0.6442250353981036,
-                    -1.713888725280831,
-                    -2.497154467628332
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -7865,30 +8495,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.0919573873116,
+                    515.1319302314583,
+                    1030.2238349616866
+                ],
+                "i_from_angle": [
+                    -2.4975758535770476,
+                    -2.4969364021103844,
+                    0.6443365381514848
+                ],
+                "i_to": [
+                    13382.827178419342,
+                    2.873521302497315,
+                    13383.173353419996
+                ],
+                "i_to_angle": [
+                    0.6442299615255769,
+                    2.094368884982897,
+                    -2.4971495415691582
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7721.228567385602,
-                    2.594535229648264e-12,
-                    19186.031320276204
-                ],
-                "i_angle": [
-                    0.8059230784945488,
-                    2.296243323594852,
-                    -2.562054612774953
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8057,30 +8703,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    297.13010400412185,
+                    738.4926421496681,
+                    1030.2238349616864
+                ],
+                "i_from_angle": [
+                    -2.3359771862166787,
+                    -2.561910258445729,
+                    0.6443365381514847
+                ],
+                "i_to": [
+                    11469.274765045517,
+                    3930.2119437719093,
+                    15309.748772985855
+                ],
+                "i_to_angle": [
+                    0.680371875372166,
+                    0.4324818160352093,
+                    -2.5242493686892162
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    120361.0200184777,
-                    1.8564982859236946e-11,
-                    140755.17391308164
-                ],
-                "i_angle": [
-                    0.986852193566392,
-                    1.8325957145940457,
-                    -2.8231169138858645
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8249,30 +8911,46 @@
                 "i_angle": [
                     -2.127659379225248,
                     -0.6782550775839501,
                     0.2952786672127304
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    502.4936290101132,
+                    587.6500026354182,
+                    1030.2238349616873
+                ],
+                "i_from_angle": [
+                    -2.1359878000298025,
+                    -2.8042987696963544,
+                    0.6443365381514846
+                ],
+                "i_to": [
+                    13083.547308663361,
+                    3173.762697451819,
+                    13858.808131235684
+                ],
+                "i_to_angle": [
+                    0.7621738096661357,
+                    -0.6780310070941973,
+                    -2.608473442481526
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    119077.38838665358,
-                    1.6409281590473077e-11,
-                    141595.5411089959
-                ],
-                "i_angle": [
-                    0.984535840578501,
-                    1.9744927691982097,
-                    -2.8159686329279285
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8441,30 +9119,46 @@
                 "i_angle": [
                     -2.1309553102130865,
                     -1.185706251367995,
                     0.2940119262210602
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    497.13437207662156,
+                    591.1587840230851,
+                    1030.223834961687
+                ],
+                "i_from_angle": [
+                    -2.138304551143991,
+                    -2.797150523835078,
+                    0.6443365381514847
+                ],
+                "i_to": [
+                    13040.912813484474,
+                    3144.7746365857574,
+                    13895.639061055144
+                ],
+                "i_to_angle": [
+                    0.760573458972069,
+                    -0.6494045506597914,
+                    -2.606313829456001
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.375900036133,
-                    4.784086579150955e-12,
-                    11222.810149527173
-                ],
-                "i_angle": [
-                    0.6750335118103362,
-                    -1.0640182758688834,
-                    -2.466306024692125
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8633,30 +9327,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.9178265285193,
+                    431.9679446545581,
+                    863.8857089150774
+                ],
+                "i_from_angle": [
+                    -2.4668012003857265,
+                    -2.466041837625395,
+                    0.6751711566113577
+                ],
+                "i_to": [
+                    11221.987620312308,
+                    2.8735435613424603,
+                    11222.42165604351
+                ],
+                "i_to_angle": [
+                    0.6750445936988166,
+                    2.0943416928813887,
+                    -2.466294938960812
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7457.205399444285,
-                    1.8346134549116837e-12,
-                    15094.372232082711
-                ],
-                "i_angle": [
-                    0.8135507599874563,
-                    -1.6307474933923898,
-                    -2.5346377882720494
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -8825,30 +9535,46 @@
                 "i_angle": [
                     0.0,
                     0.0,
                     0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    286.967185716652,
+                    580.9930367507461,
+                    863.8857089150777
+                ],
+                "i_from_angle": [
+                    -2.3283588184980504,
+                    -2.534450178745843,
+                    0.6751711566113578
+                ],
+                "i_to": [
+                    9948.911217083618,
+                    2648.220593071964,
+                    12506.056596594462
+                ],
+                "i_to_angle": [
+                    0.7095561236080952,
+                    0.4139029192319782,
+                    -2.4937737023170383
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    36054.19841843337,
-                    1.0378140918593053e-11,
-                    53265.519171442575
-                ],
-                "i_angle": [
-                    0.9237460592943133,
-                    1.3689481055932395,
-                    -2.4931485529650943
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9017,30 +9743,46 @@
                 "i_angle": [
                     -2.203932194875449,
                     0.17957730748996176,
                     0.6391110419981778
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    150.50588058113132,
+                    222.38143607662778,
+                    369.49726247056464
+                ],
+                "i_from_angle": [
+                    -2.199166366726269,
+                    -2.4742482257494967,
+                    0.7782116559575174
+                ],
+                "i_to": [
+                    4490.882354955284,
+                    759.0859352916882,
+                    5118.433159278242
+                ],
+                "i_to_angle": [
+                    0.8256766796242868,
+                    0.18212111114613386,
+                    -2.405022921041424
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    36083.42218905787,
-                    9.282491429618473e-12,
-                    53218.61411708043
-                ],
-                "i_angle": [
-                    0.9218213964545677,
-                    1.8325957145940457,
-                    -2.4920416614194276
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9209,30 +9951,46 @@
                 "i_angle": [
                     -2.1953730725417357,
                     -0.3530034709264352,
                     0.6316398601264039
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    150.62792134061246,
+                    222.18563241353274,
+                    369.49726247056475
+                ],
+                "i_from_angle": [
+                    -2.201091263618247,
+                    -2.4731411853105865,
+                    0.7782116559575173
+                ],
+                "i_to": [
+                    4492.222780013274,
+                    754.1000383014048,
+                    5116.888168807475
+                ],
+                "i_to_angle": [
+                    0.8251488661980487,
+                    0.18501948096949236,
+                    -2.404584681829933
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.68843522593,
-                    21570.682529967948,
-                    2.320622857404618e-12
-                ],
-                "i_angle": [
-                    1.572814171766922,
-                    -1.5689116903586477,
-                    2.8797932657906435
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9401,30 +10159,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811572,
+                    830.2557558382571,
+                    830.2564162917023
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    1.5725477525192528,
+                    1.5729473823380995
+                ],
+                "i_to": [
+                    21570.688342445308,
+                    21570.68262275059,
+                    2.873435435122069
+                ],
+                "i_to_angle": [
+                    1.5728141724699156,
+                    -1.568911691061069,
+                    -3.930288366482592e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    69271.82833350312,
-                    69051.16112977838,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    2.821507715355243,
-                    -2.827324958442905,
-                    -2.6179938779914944
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9593,30 +10367,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.512138981157,
+                    2658.0702723990444,
+                    2666.5638579661513
+                ],
+                "i_from_angle": [
+                    -1.5688450860816423,
+                    0.31423183730265486,
+                    2.8215433436531447
+                ],
+                "i_to": [
+                    30826.59870747015,
+                    30661.10744675486,
+                    43813.0975276303
+                ],
+                "i_to_angle": [
+                    2.363137374630999,
+                    -2.364701600250055,
+                    -0.0034322944542554404
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    53217.35452201775,
-                    41650.47799042057,
-                    7.338453819646735e-12
-                ],
-                "i_angle": [
-                    1.6767104966603836,
-                    -1.3788550566126192,
-                    0.059951166597492535
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9785,30 +10575,46 @@
                 "i_angle": [
                     -1.3799197446184093,
                     1.9307594158658887,
                     -1.9038582853800772
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811575,
+                    729.6858726677895,
+                    932.3386301325361
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    1.6209764147101378,
+                    1.535007396401781
+                ],
+                "i_to": [
+                    22451.063945464975,
+                    20694.616603803122,
+                    1859.294711300958
+                ],
+                "i_to_angle": [
+                    1.5591775165961017,
+                    -1.5541232025440717,
+                    -1.9027215079963948
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    70107.07595326328,
-                    40669.78106955474,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    2.1137287380833887,
-                    -2.161455671065789,
-                    2.0943951023931953
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -9977,30 +10783,46 @@
                 "i_angle": [
                     -1.2476975194536815,
                     1.7130179309450098,
                     -2.996837746647216
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811575,
+                    712.5253245869043,
+                    1228.2532885847234
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    0.8383668396248599,
+                    1.9720215639146954
+                ],
+                "i_to": [
+                    24531.79733183281,
+                    19406.274106929402,
+                    9779.940162738505
+                ],
+                "i_to_angle": [
+                    1.7421179502045023,
+                    -1.7835731779594388,
+                    -0.5610938827346019
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.37922600466,
-                    13383.0330060547,
-                    4.10232039761827e-13
-                ],
-                "i_angle": [
-                    1.6916357363109418,
-                    -1.450170066147722,
-                    2.0943951023931953
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10169,30 +10991,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616869,
+                    515.0919579442943,
+                    515.1319296741964
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6912143520570537,
+                    1.691853801829054
+                ],
+                "i_to": [
+                    13383.173348594775,
+                    13382.827183243762,
+                    2.8735126351761693
+                ],
+                "i_to_angle": [
+                    1.6916406629348313,
+                    -1.4501651405851324,
+                    -2.320067807838939e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    19456.22057196866,
-                    7419.839685663983,
-                    2.320622857404618e-12
-                ],
-                "i_angle": [
-                    1.635831835487355,
-                    -1.303566640350549,
-                    2.8797932657906435
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10361,30 +11199,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.223834961687,
+                    285.52973769564085,
+                    748.8943902614442
+                ],
+                "i_from_angle": [
+                    -1.4500585642417108,
+                    1.8377014757897425,
+                    1.6359747388162487
+                ],
+                "i_to": [
+                    15401.819741514097,
+                    11374.095419081752,
+                    4093.094131803335
+                ],
+                "i_to_angle": [
+                    1.6681482768322988,
+                    -1.41838910521614,
+                    -1.6269597242918514
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    139780.5903331014,
-                    139964.23210688512,
-                    7.338453819646735e-12
-                ],
-                "i_angle": [
-                    1.181890834986739,
-                    -0.9786853151733277,
-                    -3.0816414869923006
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10553,30 +11407,46 @@
                 "i_angle": [
                     -1.9947264499020338,
                     2.194063754884357,
                     -3.022476052482497
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    584.3374841752325,
+                    583.5770569950439
+                ],
+                "i_from_angle": [
+                    -1.4500585642417108,
+                    2.181669399907289,
+                    1.2007033944636623
+                ],
+                "i_to": [
+                    13589.691960460561,
+                    13597.042076182825,
+                    4764.429165204173
+                ],
+                "i_to_angle": [
+                    1.5153281958042402,
+                    -1.2739489192107014,
+                    -3.022421847892221
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    142279.7550019918,
-                    137227.55916061433,
-                    3.281856318094616e-11
-                ],
-                "i_angle": [
-                    1.1933658429184906,
-                    -0.9702237331364222,
-                    -0.11990233319498574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10745,30 +11615,46 @@
                 "i_angle": [
                     -1.9947264499020338,
                     2.194063754884357,
                     2.769698016293363
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616875,
+                    572.9115267767705,
+                    594.0115417309961
+                ],
+                "i_from_angle": [
+                    -1.4500585642417108,
+                    2.1901310483550103,
+                    1.2121782010087496
+                ],
+                "i_to": [
+                    13693.595508900993,
+                    13489.795653281994,
+                    4749.685581621309
+                ],
+                "i_to_angle": [
+                    1.5173927595668415,
+                    -1.2732588132739462,
+                    -2.9772639029471084
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.81013470817,
-                    11222.375914852375,
-                    2.051160198809135e-12
-                ],
-                "i_angle": [
-                    1.7224841791245016,
-                    -1.4193615896127225,
-                    3.0216903203948076
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -10937,30 +11823,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150774,
+                    431.9178270987636,
+                    431.9679440839958
+                ],
+                "i_from_angle": [
+                    -1.4192239457818374,
+                    1.7219890053712854,
+                    1.722748366191491
+                ],
+                "i_to": [
+                    11222.421651103217,
+                    11221.987625251688,
+                    2.873534894844026
+                ],
+                "i_to_angle": [
+                    1.7224952655022867,
+                    -1.419350508370962,
+                    -5.039228323897977e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15221.049096159133,
-                    7319.189126557198,
-                    1.6914300309505968e-12
-                ],
-                "i_angle": [
-                    1.658736306989672,
-                    -1.2866285312916301,
-                    0.7685774387251628
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11129,30 +12031,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150773,
+                    281.6548538632998,
+                    585.869905346292
+                ],
+                "i_from_angle": [
+                    -1.4192239457818376,
+                    1.8546395310461297,
+                    1.658922685043144
+                ],
+                "i_to": [
+                    12549.167317231457,
+                    9904.591373024125,
+                    2722.7856230718176
+                ],
+                "i_to_angle": [
+                    1.6967311008894097,
+                    -1.38673881338788,
+                    -1.6577788654280021
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    54337.527262938915,
-                    35029.469115811684,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    1.6952675182928678,
-                    -1.1617714025221006,
-                    -1.047197551196598
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11321,30 +12239,46 @@
                 "i_angle": [
                     -1.4555014066657503,
                     1.9951241893330474,
                     -1.8726040126940242
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.4972624705648,
+                    146.22739049170715,
+                    226.85718134633638
+                ],
+                "i_from_angle": [
+                    -1.3161834464356779,
+                    1.99850012632808,
+                    1.7141654068121748
+                ],
+                "i_to": [
+                    5157.05123355352,
+                    4452.728146974395,
+                    829.0823516211836
+                ],
+                "i_to_angle": [
+                    1.78310427820193,
+                    -1.267181819484384,
+                    -1.8702298199951437
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    54275.89107352634,
-                    35070.43982648013,
-                    7.338453819646735e-12
-                ],
-                "i_angle": [
-                    1.6964695822675262,
-                    -1.1640506329236346,
-                    -2.1543462689906883
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11513,30 +12447,46 @@
                 "i_angle": [
                     -1.4636379352734856,
                     2.0049521811971256,
                     -2.4053160520129597
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.49726247056486,
+                    146.39848076800456,
+                    226.59987612074252
+                ],
+                "i_from_angle": [
+                    -1.3161834464356783,
+                    1.996220627993811,
+                    1.715367650840787
+                ],
+                "i_to": [
+                    5154.989911419624,
+                    4454.553684974288,
+                    823.0345262346136
+                ],
+                "i_to_angle": [
+                    1.7835906590937851,
+                    -1.2677845399869683,
+                    -1.8673712071978297
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    21570.68844825462,
-                    21570.68251694099,
-                    0.0
-                ],
-                "i_angle": [
-                    1.5728141723682283,
-                    -1.5689116909600345,
-                    3.141592653589793
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11705,30 +12655,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811572,
+                    830.2557553368771,
+                    830.256416793282
+                ],
+                "i_from_angle": [
+                    -1.5688450860816425,
+                    1.5725477519177389,
+                    1.5729473829393714
+                ],
+                "i_to": [
+                    21570.688346788542,
+                    21570.682618407944,
+                    2.8734441007062763
+                ],
+                "i_to_angle": [
+                    1.5728141726703666,
+                    -1.5689116912615464,
+                    -4.2319700510579596e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    105344.74178499487,
-                    80715.25872943086,
-                    1.8564982859236942e-11
-                ],
-                "i_angle": [
-                    2.355569018027442,
-                    2.74208669758657,
-                    1.308996938995747
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -11897,30 +12863,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.512138981158,
+                    3107.097406011981,
+                    4055.0658129596454
+                ],
+                "i_from_angle": [
+                    -1.568845086081642,
+                    -0.39951119408977526,
+                    2.3555992918609077
+                ],
+                "i_to": [
+                    46433.55279199728,
+                    25068.632233629516,
+                    60892.07184358473
+                ],
+                "i_to_angle": [
+                    2.1353915063624926,
+                    -2.984820760929833,
+                    -0.6186466544472315
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    52909.12709036596,
-                    41964.987988930094,
-                    4.641245714809236e-12
-                ],
-                "i_angle": [
-                    1.675101684355795,
-                    -1.3774653992583374,
-                    2.8797932657906435
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12089,30 +13071,46 @@
                 "i_angle": [
                     -1.3817582774270811,
                     1.9312632128135074,
                     -1.9331431496984186
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.5121389811577,
+                    735.1959590214595,
+                    926.9385402759627
+                ],
+                "i_from_angle": [
+                    -1.5688450860816427,
+                    1.622366336109748,
+                    1.5333987206337634
+                ],
+                "i_to": [
+                    22403.992073083664,
+                    20742.008580923866,
+                    1778.1116567243553
+                ],
+                "i_to_angle": [
+                    1.5586517432994271,
+                    -1.5536197294907532,
+                    -1.931972670162038
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    76734.0685122063,
-                    31184.17013909326,
-                    6.563712636189232e-12
-                ],
-                "i_angle": [
-                    2.013795089742575,
-                    -2.2389889193572996,
-                    0.5235987755982987
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12281,30 +13279,46 @@
                 "i_angle": [
                     -1.317577506062135,
                     1.845071650808923,
                     2.996085213782915
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1660.512138981158,
+                    546.3425489709848,
+                    1344.3533014954269
+                ],
+                "i_from_angle": [
+                    -1.5688450860816425,
+                    0.7608221341279923,
+                    1.8720857363534407
+                ],
+                "i_to": [
+                    25735.213052947634,
+                    17967.252898950905,
+                    10443.60353186971
+                ],
+                "i_to_angle": [
+                    1.7065518055543236,
+                    -1.761109201582104,
+                    -0.8513796978060578
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    13383.379240478607,
-                    13383.03299158317,
-                    2.209167143284393e-12
-                ],
-                "i_angle": [
-                    1.691635737158059,
-                    -1.4501700669950917,
-                    2.47490147950556
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12473,30 +13487,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616869,
+                    515.0919573873116,
+                    515.1319302314583
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.6912143512093436,
+                    1.6918538026760066
+                ],
+                "i_to": [
+                    13383.173353419992,
+                    13382.82717841934,
+                    2.873521302497314
+                ],
+                "i_to_angle": [
+                    1.6916406632172332,
+                    -1.4501651408676184,
+                    -2.6217410298204696e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    19186.031320276204,
-                    7721.2285673856,
-                    2.5945352296482635e-12
-                ],
-                "i_angle": [
-                    1.6267355920114381,
-                    -1.2884720238986465,
-                    0.20184822120165646
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12665,30 +13695,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616866,
+                    297.13010400412185,
+                    738.492642149668
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    1.8528130185697123,
+                    1.6268799463406622
+                ],
+                "i_to": [
+                    15309.748772985855,
+                    11469.274765045517,
+                    3930.2119437719102
+                ],
+                "i_to_angle": [
+                    1.664540836097175,
+                    -1.4140232270210293,
+                    -1.661913286357986
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    140755.17391308164,
-                    120361.02001847768,
-                    1.8564982859236942e-11
-                ],
-                "i_angle": [
-                    1.3656732909005267,
-                    -1.1075429088268034,
-                    -0.2617993877991497
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -12857,30 +13903,46 @@
                 "i_angle": [
                     -1.799116435180465,
                     2.0611308255611434,
                     -2.7726501799771452
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.2238349616873,
+                    502.4936290101132,
+                    587.6500026354183
+                ],
+                "i_from_angle": [
+                    -1.4500585642417108,
+                    2.0528024047565885,
+                    1.384491435090037
+                ],
+                "i_to": [
+                    13858.808131235688,
+                    13083.547308663365,
+                    3173.7626974518193
+                ],
+                "i_to_angle": [
+                    1.5803167623048648,
+                    -1.3322212927270596,
+                    -2.7724261094873928
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    141595.5411089959,
-                    119077.38838665358,
-                    1.640928159047308e-11
-                ],
-                "i_angle": [
-                    1.3728215718584627,
-                    -1.1098592618146943,
-                    -0.11990233319498574
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13049,30 +14111,46 @@
                 "i_angle": [
                     -1.8003831761721352,
                     2.0578348945733045,
                     3.0030839534183964
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1030.223834961687,
+                    497.13437207662156,
+                    591.1587840230852
+                ],
+                "i_from_angle": [
+                    -1.4500585642417105,
+                    2.0504856536424003,
+                    1.3916396809513132
+                ],
+                "i_to": [
+                    13895.639061055144,
+                    13040.912813484472,
+                    3144.774636585757
+                ],
+                "i_to_angle": [
+                    1.5824763753303903,
+                    -1.3338216434211263,
+                    -2.7437996530529865
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    11222.810149527173,
-                    11222.375900036133,
-                    4.784086579150955e-12
-                ],
-                "i_angle": [
-                    1.7224841800942663,
-                    -1.4193615905828592,
-                    3.1247719289175078
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13241,30 +14319,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150772,
+                    431.91782652851936,
+                    431.96794465455815
+                ],
+                "i_from_angle": [
+                    -1.4192239457818376,
+                    1.7219890044006647,
+                    1.7227483671609962
+                ],
+                "i_to": [
+                    11222.421656043509,
+                    11221.987620312308,
+                    2.87354356134246
+                ],
+                "i_to_angle": [
+                    1.722495265825579,
+                    -1.4193505086943785,
+                    -5.340951180670001e-05
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    15094.372232082711,
-                    7457.205399444285,
-                    1.8346134549116837e-12
-                ],
-                "i_angle": [
-                    1.654152416514342,
-                    -1.280844342405739,
-                    2.5580427113940014
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13433,30 +14527,46 @@
                 "i_angle": [
                     -0.0,
                     -0.0,
                     -0.0
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    863.8857089150775,
+                    286.967185716652,
+                    580.9930367507461
+                ],
+                "i_from_angle": [
+                    -1.4192239457818376,
+                    1.8604313862883408,
+                    1.654340026040548
+                ],
+                "i_to": [
+                    12506.05659659446,
+                    9948.911217083618,
+                    2648.2205930719633
+                ],
+                "i_to_angle": [
+                    1.695016502469353,
+                    -1.3848389787851,
+                    -1.6804921831612172
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    53265.51917144259,
-                    36054.19841843338,
-                    1.0378140918593054e-11
-                ],
-                "i_angle": [
-                    1.6956416518212971,
-                    -1.170649043098882,
-                    -0.7254469967999558
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13625,30 +14735,46 @@
                 "i_angle": [
                     -1.4552840603950175,
                     1.9848580099109423,
                     -1.9148177949032334
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.4972624705646,
+                    150.50588058113132,
+                    222.38143607662778
+                ],
+                "i_from_angle": [
+                    -1.3161834464356779,
+                    1.9896238380601226,
+                    1.7145419790368943
+                ],
+                "i_to": [
+                    5118.433159278243,
+                    4490.882354955284,
+                    759.0859352916881
+                ],
+                "i_to_angle": [
+                    1.7837672837449674,
+                    -1.2687184227689086,
+                    -1.9122739912470614
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    53218.614117080426,
-                    36083.42218905787,
-                    9.282491429618471e-12
-                ],
-                "i_angle": [
-                    1.6967485433669636,
-                    -1.1725737059386276,
-                    -0.2617993877991497
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -13817,30 +14943,46 @@
                 "i_angle": [
                     -1.4627552422667913,
                     1.9934171322446552,
                     -2.44739857331963
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    369.49726247056475,
+                    150.62792134061246,
+                    222.18563241353272
+                ],
+                "i_from_angle": [
+                    -1.3161834464356779,
+                    1.987698941168144,
+                    1.715649019475805
+                ],
+                "i_to": [
+                    5116.888168807474,
+                    4492.222780013273,
+                    754.1000383014047
+                ],
+                "i_to_angle": [
+                    1.7842055229564582,
+                    -1.2692462361951466,
+                    -1.9093756214237028
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.3206228574046182e-12,
-                    21570.688435225937,
-                    21570.68252996795
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.5215809306262733,
-                    2.6198785144277434
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14009,30 +15151,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2564162917024,
+                    1660.5121389811572,
+                    830.2557558382572
+                ],
+                "i_from_angle": [
+                    -0.5214477200550958,
+                    2.6199451187047487,
+                    -0.5218473498739424
+                ],
+                "i_to": [
+                    2.87343543512207,
+                    21570.68834244531,
+                    21570.682622750595
+                ],
+                "i_to_angle": [
+                    -2.09443440527686,
+                    -0.5215809299232796,
+                    2.619878513725322
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    69271.82833350313,
-                    69051.16112977838
-                ],
-                "i_angle": [
-                    1.5707963267948966,
-                    0.7271126129620479,
-                    1.3614652463434862
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14201,30 +15359,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    2666.5638579661513,
+                    1660.5121389811568,
+                    2658.0702723990444
+                ],
+                "i_from_angle": [
+                    0.7271482412599496,
+                    2.6199451187047487,
+                    -1.7801632650905403
+                ],
+                "i_to": [
+                    43813.09752763029,
+                    30826.59870747015,
+                    30661.10744675486
+                ],
+                "i_to_angle": [
+                    -2.0978273968474506,
+                    0.2687422722378037,
+                    1.824088604536336
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    53217.35452201774,
-                    41650.47799042057
-                ],
-                "i_angle": [
-                    -2.0344439357957027,
-                    -0.4176846057328116,
-                    2.809935148173772
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14393,30 +15567,46 @@
                 "i_angle": [
                     2.284931919406314,
                     2.8088704601679817,
                     -0.16363568652730645
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    932.3386301325361,
+                    1660.5121389811575,
+                    729.6858726677895
+                ],
+                "i_from_angle": [
+                    -0.5593877059914143,
+                    2.6199451187047487,
+                    -0.4734186876830576
+                ],
+                "i_to": [
+                    1859.294711300958,
+                    22451.063945464975,
+                    20694.61660380312
+                ],
+                "i_to_angle": [
+                    2.2860686967899966,
+                    -0.5352175857970936,
+                    2.6346670022423195
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    70107.07595326328,
-                    40669.78106955473
-                ],
-                "i_angle": [
-                    0.0,
-                    0.019333635690193373,
-                    2.027334533720602
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14585,30 +15775,46 @@
                 "i_angle": [
                     1.1919524581391756,
                     2.9410926853327095,
                     -0.3813771714481855
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1228.2532885847236,
+                    1660.5121389811575,
+                    712.5253245869044
+                ],
+                "i_from_angle": [
+                    -0.12237353847849994,
+                    2.6199451187047487,
+                    -1.2560282627683352
+                ],
+                "i_to": [
+                    9779.940162738505,
+                    24531.79733183281,
+                    19406.274106929406
+                ],
+                "i_to_angle": [
+                    -2.655488985127797,
+                    -0.3522771521886929,
+                    2.4052170268269526
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.10232039761827e-13,
-                    13383.37922600466,
-                    13383.033006054702
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.4027593660822535,
-                    2.738620138638669
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14777,30 +15983,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1319296741964,
+                    1030.2238349616869,
+                    515.0919579442944
+                ],
+                "i_from_angle": [
+                    -0.4025413005641413,
+                    2.738731640544681,
+                    -0.40318075033614154
+                ],
+                "i_to": [
+                    2.8735126351761697,
+                    13383.173348594773,
+                    13382.827183243764
+                ],
+                "i_to_angle": [
+                    -2.0944183030712735,
+                    -0.40275443945836403,
+                    2.738625064201259
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.3206228574046182e-12,
-                    19456.22057196866,
-                    7419.839685663981
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.45856326690584037,
-                    2.885223564435842
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -14969,30 +16191,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    748.8943902614443,
+                    1030.223834961687,
+                    285.5297376956408
+                ],
+                "i_from_angle": [
+                    -0.4584203635769466,
+                    2.7387316405446804,
+                    -0.25669362660345274
+                ],
+                "i_to": [
+                    4093.094131803336,
+                    15401.819741514097,
+                    11374.095419081752
+                ],
+                "i_to_angle": [
+                    2.5618304804945398,
+                    -0.4262468255608965,
+                    2.7704010995702513
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    139780.59033310143,
-                    139964.23210688512
-                ],
-                "i_angle": [
-                    1.1071487177940904,
-                    -0.9125042674064562,
-                    -3.0730804175665227
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15161,30 +16399,46 @@
                 "i_angle": [
                     1.166314152303894,
                     2.1940637548843576,
                     0.09966865249116195
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    583.5770569950439,
+                    1030.2238349616873,
+                    584.3374841752326
+                ],
+                "i_from_angle": [
+                    -0.8936917079295331,
+                    2.7387316405446804,
+                    0.08727429751409356
+                ],
+                "i_to": [
+                    4764.429165204173,
+                    13589.691960460563,
+                    13597.042076182825
+                ],
+                "i_to_angle": [
+                    1.1663683568941703,
+                    -0.5790669065889551,
+                    2.9148412855756898
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    3.281856318094616e-11,
-                    142279.75500199184,
-                    137227.55916061436
-                ],
-                "i_angle": [
-                    -2.214297435588181,
-                    -0.9010292594747048,
-                    -3.0646188355296173
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15353,30 +16607,46 @@
                 "i_angle": [
                     0.6753029139001677,
                     2.1940637548843576,
                     0.09966865249116202
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    594.0115417309962,
+                    1030.2238349616875,
+                    572.9115267767704
+                ],
+                "i_from_angle": [
+                    -0.8822169013844455,
+                    2.7387316405446804,
+                    0.0957359459618152
+                ],
+                "i_to": [
+                    4749.68558162131,
+                    13693.595508900993,
+                    13489.795653281992
+                ],
+                "i_to_angle": [
+                    1.2115263018392826,
+                    -0.5770023428263538,
+                    2.9155313915124452
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.051160198809135e-12,
-                    11222.810134708174,
-                    11222.375914852377
-                ],
-                "i_angle": [
-                    0.9272952180016122,
-                    -0.3719109232686938,
-                    2.769428615173669
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15545,30 +16815,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.9679440839958,
+                    863.8857089150778,
+                    431.9178270987636
+                ],
+                "i_from_angle": [
+                    -0.37164673620170424,
+                    2.769566259004554,
+                    -0.37240609702190974
+                ],
+                "i_to": [
+                    2.8735348948440262,
+                    11222.421651103217,
+                    11221.98762525169
+                ],
+                "i_to_angle": [
+                    -2.0944454946764344,
+                    -0.3718998368909085,
+                    2.769439696415429
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.6914300309505968e-12,
-                    15221.049096159133,
-                    7319.189126557197
-                ],
-                "i_angle": [
-                    -1.3258176636680326,
-                    -0.43565879540352337,
-                    2.9021616734947613
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15737,30 +17023,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    585.8699053462921,
+                    863.8857089150774,
+                    281.6548538632998
+                ],
+                "i_from_angle": [
+                    -0.4354724173500512,
+                    2.7695662590045536,
+                    -0.23975557134706554
+                ],
+                "i_to": [
+                    2722.7856230718176,
+                    12549.167317231457,
+                    9904.591373024126
+                ],
+                "i_to_angle": [
+                    2.5310113393583893,
+                    -0.3976640015037856,
+                    2.802051391398511
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    54337.52726293892,
-                    35029.46911581169
-                ],
-                "i_angle": [
-                    3.141592653589793,
-                    -0.3991275841003275,
-                    3.0270188022642905
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -15929,30 +17231,46 @@
                 "i_angle": [
                     2.316186192092367,
                     2.7332887981206406,
                     -0.09927091306014796
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    226.8571813463364,
+                    369.49726247056475,
+                    146.22739049170715
+                ],
+                "i_from_angle": [
+                    -0.38022969558102043,
+                    2.8726067583507136,
+                    -0.09589497606511535
+                ],
+                "i_to": [
+                    829.0823516211838,
+                    5157.05123355352,
+                    4452.728146974395
+                ],
+                "i_to_angle": [
+                    2.3185603847912475,
+                    -0.3112908241912653,
+                    2.921608385302007
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    7.338453819646735e-12,
-                    54275.891073526356,
-                    35070.439826480135
-                ],
-                "i_angle": [
-                    2.0344439357957027,
-                    -0.3979255201256691,
-                    3.0247395718627565
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16121,30 +17439,46 @@
                 "i_angle": [
                     1.7834741527734312,
                     2.725152269512906,
                     -0.08944292119606981
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    226.59987612074252,
+                    369.4972624705649,
+                    146.39848076800456
+                ],
+                "i_from_angle": [
+                    -0.37902745155240836,
+                    2.872606758350713,
+                    -0.0981744743993842
+                ],
+                "i_to": [
+                    823.0345262346136,
+                    5154.989911419625,
+                    4454.553684974288
+                ],
+                "i_to_angle": [
+                    2.3214189975885615,
+                    -0.3108044432994101,
+                    2.9210056647994227
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    0.0,
-                    21570.688448254623,
-                    21570.682516940993
-                ],
-                "i_angle": [
-                    0.0,
-                    -0.521580930024967,
-                    2.6198785138263565
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16313,30 +17647,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    830.2564167932821,
+                    1660.512138981157,
+                    830.2557553368771
+                ],
+                "i_from_angle": [
+                    -0.5214477194538237,
+                    2.6199451187047487,
+                    -0.5218473504754563
+                ],
+                "i_to": [
+                    2.8734441007062768,
+                    21570.68834678855,
+                    21570.68261840794
+                ],
+                "i_to_angle": [
+                    -2.094437422093706,
+                    -0.5215809297228285,
+                    2.619878513524845
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8564982859236946e-11,
-                    105344.74178499488,
-                    80715.25872943088
-                ],
-                "i_angle": [
-                    -0.7853981633974483,
-                    0.26117391563424647,
-                    0.6476915951933747
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16505,30 +17855,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    4055.0658129596454,
+                    1660.512138981158,
+                    3107.097406011981
+                ],
+                "i_from_angle": [
+                    0.2612041894677123,
+                    2.619945118704749,
+                    -2.4939062964829706
+                ],
+                "i_to": [
+                    60892.07184358473,
+                    46433.55279199729,
+                    25068.632233629523
+                ],
+                "i_to_angle": [
+                    -2.713041756840427,
+                    0.040996403969297296,
+                    1.2039694438565582
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.6412457148092364e-12,
-                    52909.12709036595,
-                    41964.98798893011
-                ],
-                "i_angle": [
-                    0.7853981633974483,
-                    -0.41929341803740017,
-                    2.8113248055280535
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16697,30 +18063,46 @@
                 "i_angle": [
                     2.2556470550879726,
                     2.80703192735931,
                     -0.16313188957968786
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    926.9385402759627,
+                    1660.5121389811577,
+                    735.1959590214595
+                ],
+                "i_from_angle": [
+                    -0.560996381759432,
+                    2.6199451187047487,
+                    -0.47202876628344714
+                ],
+                "i_to": [
+                    1778.1116567243553,
+                    22403.99207308366,
+                    20742.00858092387
+                ],
+                "i_to_angle": [
+                    2.256817534624353,
+                    -0.535743359093768,
+                    2.635170475295638
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    6.563712636189232e-12,
-                    76734.0685122063,
-                    31184.17013909327
-                ],
-                "i_angle": [
-                    -1.5707963267948966,
-                    -0.08060001265062024,
-                    1.9498012854290918
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -16889,30 +18271,46 @@
                 "i_angle": [
                     0.9016901113897194,
                     2.871212698724256,
                     -0.2493234515842721
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    1344.3533014954266,
+                    1660.5121389811577,
+                    546.3425489709848
+                ],
+                "i_from_angle": [
+                    -0.22230936603975465,
+                    2.6199451187047487,
+                    -1.333572968265203
+                ],
+                "i_to": [
+                    10443.603531869712,
+                    25735.213052947638,
+                    17967.252898950905
+                ],
+                "i_to_angle": [
+                    -2.945774800199253,
+                    -0.38784329683887153,
+                    2.4276810032042873
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.209167143284393e-12,
-                    13383.379240478609,
-                    13383.032991583173
-                ],
-                "i_angle": [
-                    0.3805063771123649,
-                    -0.4027593652351362,
-                    2.7386201377912993
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17081,30 +18479,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    515.1319302314585,
+                    1030.2238349616869,
+                    515.0919573873116
+                ],
+                "i_from_angle": [
+                    -0.40254129971718866,
+                    2.738731640544681,
+                    -0.4031807511838516
+                ],
+                "i_to": [
+                    2.873521302497315,
+                    13383.173353419996,
+                    13382.82717841934
+                ],
+                "i_to_angle": [
+                    -2.0944213198034936,
+                    -0.40275443917596215,
+                    2.738625063918773
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    2.594535229648264e-12,
-                    19186.031320276208,
-                    7721.228567385602
-                ],
-                "i_angle": [
-                    -1.892546881191539,
-                    -0.46765951038175707,
-                    2.9003181808877447
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17273,30 +18687,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    738.4926421496681,
+                    1030.2238349616864,
+                    297.13010400412185
+                ],
+                "i_from_angle": [
+                    -0.4675151560525329,
+                    2.7387316405446804,
+                    -0.24158208382348295
+                ],
+                "i_to": [
+                    3930.2119437719102,
+                    15309.748772985855,
+                    11469.274765045517
+                ],
+                "i_to_angle": [
+                    2.5268769184284054,
+                    -0.4298542662960204,
+                    2.774766977765362
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8564982859236946e-11,
-                    140755.17391308167,
-                    120361.0200184777
-                ],
-                "i_angle": [
-                    -2.356194490192345,
-                    -0.7287218114926687,
-                    3.081247295959588
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17465,30 +18895,46 @@
                 "i_angle": [
                     1.4161400248092457,
                     2.3896737696059263,
                     -0.03326427683205201
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    587.6500026354183,
+                    1030.2238349616875,
+                    502.4936290101132
+                ],
+                "i_from_angle": [
+                    -0.7099036673031583,
+                    2.7387316405446804,
+                    -0.041592697636606675
+                ],
+                "i_to": [
+                    3173.7626974518193,
+                    13858.808131235688,
+                    13083.547308663361
+                ],
+                "i_to_angle": [
+                    1.4163640952989984,
+                    -0.5140783400883304,
+                    2.856568912059332
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.640928159047308e-11,
-                    141595.5411089959,
-                    119077.38838665358
-                ],
-                "i_angle": [
-                    -2.214297435588181,
-                    -0.7215735305347325,
-                    3.078930942971697
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17657,30 +19103,46 @@
                 "i_angle": [
                     0.9086888510252009,
                     2.3884070286142562,
                     -0.036560207819890736
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    591.1587840230852,
+                    1030.223834961687,
+                    497.13437207662156
+                ],
+                "i_from_angle": [
+                    -0.7027554214418821,
+                    2.7387316405446804,
+                    -0.043909448750795034
+                ],
+                "i_to": [
+                    3144.7746365857574,
+                    13895.639061055148,
+                    13040.912813484474
+                ],
+                "i_to_angle": [
+                    1.4449905517334045,
+                    -0.5119187270628048,
+                    2.854968561365265
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    4.784086579150955e-12,
-                    11222.810149527175,
-                    11222.375900036135
-                ],
-                "i_angle": [
-                    1.0303768265243125,
-                    -0.37191092229892897,
-                    2.769428614203532
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -17849,30 +19311,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    431.96794465455815,
+                    863.8857089150774,
+                    431.91782652851936
+                ],
+                "i_from_angle": [
+                    -0.37164673523219915,
+                    2.7695662590045536,
+                    -0.3724060979925305
+                ],
+                "i_to": [
+                    2.87354356134246,
+                    11222.421656043509,
+                    11221.987620312308
+                ],
+                "i_to_angle": [
+                    -2.094448511905002,
+                    -0.3718998365676162,
+                    2.7694396960920127
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.8346134549116837e-12,
-                    15094.372232082715,
-                    7457.205399444285
-                ],
-                "i_angle": [
-                    0.4636476090008061,
-                    -0.44024268587885335,
-                    2.907945862380652
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18041,30 +19519,46 @@
                 "i_angle": [
                     3.141592653589793,
                     3.141592653589793,
                     3.141592653589793
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    580.9930367507461,
+                    863.8857089150778,
+                    286.967185716652
+                ],
+                "i_from_angle": [
+                    -0.4400550763526473,
+                    2.7695662590045536,
+                    -0.23396371610485434
+                ],
+                "i_to": [
+                    2648.220593071964,
+                    12506.056596594462,
+                    9948.91121708362
+                ],
+                "i_to_angle": [
+                    2.508298021625174,
+                    -0.3993785999238423,
+                    2.803951226001291
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    1.0378140918593056e-11,
-                    53265.51917144258,
-                    36054.19841843337
-                ],
-                "i_angle": [
-                    -2.819842099193151,
-                    -0.3987534505718982,
-                    3.018141161687509
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18233,30 +19727,46 @@
                 "i_angle": [
                     2.2739724098831577,
                     2.7335061443913737,
                     -0.10953709248225307
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    222.3814360766278,
+                    369.49726247056464,
+                    150.50588058113135
+                ],
+                "i_from_angle": [
+                    -0.37985312335630084,
+                    2.872606758350713,
+                    -0.10477126433307281
+                ],
+                "i_to": [
+                    759.0859352916882,
+                    5118.433159278243,
+                    4490.882354955285
+                ],
+                "i_to_angle": [
+                    2.2765162135393298,
+                    -0.31062781864822797,
+                    2.920071782017483
+                ],
+                "id": 6
+            }
         ]
     },
     {
         "fault": [
             {
                 "energized": 1,
-                "i": [
-                    9.282491429618473e-12,
-                    53218.61411708044,
-                    36083.42218905788
-                ],
-                "i_angle": [
-                    -2.356194490192345,
-                    -0.39764655902623164,
-                    3.0162164988477635
-                ],
                 "id": 10
             }
         ],
         "line": [
             {
                 "energized": 1,
                 "i_from": [
@@ -18425,10 +19935,36 @@
                 "i_angle": [
                     1.7413916314667608,
                     2.7260349625196,
                     -0.10097797014853996
                 ],
                 "id": 5
             }
+        ],
+        "transformer": [
+            {
+                "energized": 1,
+                "i_from": [
+                    222.18563241353277,
+                    369.49726247056475,
+                    150.62792134061246
+                ],
+                "i_from_angle": [
+                    -0.3787460829173903,
+                    2.872606758350713,
+                    -0.10669616122505124
+                ],
+                "i_to": [
+                    754.1000383014048,
+                    5116.888168807475,
+                    4492.222780013275
+                ],
+                "i_to_angle": [
+                    2.2794145833626884,
+                    -0.31018957943673703,
+                    2.9195439685912445
+                ],
+                "id": 6
+            }
         ]
     }
 ]
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -2,16 +2,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -26,16 +26,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -50,16 +50,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -74,16 +74,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -98,16 +98,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -122,16 +122,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -146,16 +146,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -170,16 +170,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -194,16 +194,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -218,16 +218,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -242,16 +242,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -266,16 +266,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 6,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -578,16 +578,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -602,16 +602,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -626,16 +626,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -650,16 +650,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -674,16 +674,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -698,16 +698,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -722,16 +722,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -746,16 +746,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -770,16 +770,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -794,16 +794,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -818,16 +818,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -842,16 +842,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 5,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1154,16 +1154,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1178,16 +1178,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1202,16 +1202,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1226,16 +1226,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1250,16 +1250,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1274,16 +1274,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1298,16 +1298,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1322,16 +1322,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1346,16 +1346,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1370,16 +1370,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1394,16 +1394,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1418,16 +1418,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": 4,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1730,16 +1730,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1754,16 +1754,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1778,16 +1778,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1802,16 +1802,16 @@
     {
         "fault": [
             {
                 "fault_object": 1,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1826,16 +1826,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1850,16 +1850,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1874,16 +1874,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1898,16 +1898,16 @@
     {
         "fault": [
             {
                 "fault_object": 2,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1922,16 +1922,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1946,16 +1946,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
@@ -1970,16 +1970,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 0
             }
@@ -1994,16 +1994,16 @@
     {
         "fault": [
             {
                 "fault_object": 3,
                 "fault_phase": -1,
                 "fault_type": 3,
                 "id": 10,
-                "r_f": 0,
-                "x_f": 0
+                "r_f": 0.0,
+                "x_f": 0.0
             }
         ],
         "shunt": [
             {
                 "id": 9,
                 "status": 1
             }
```

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9238204632375/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/utils.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9237711575148/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9238204632375/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

