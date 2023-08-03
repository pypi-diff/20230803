# Comparing `tmp/pyglove-0.4.3.dev20230801.tar.gz` & `tmp/pyglove-0.4.3.dev20230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.3.dev20230801.tar", last modified: Tue Aug  1 08:06:50 2023, max compression
+gzip compressed data, was "pyglove-0.4.3.dev20230802.tar", last modified: Wed Aug  2 08:06:47 2023, max compression
```

## Comparing `pyglove-0.4.3.dev20230801.tar` & `pyglove-0.4.3.dev20230802.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-01 08:06:48.000000 pyglove-0.4.3.dev20230801/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.024967 pyglove-0.4.3.dev20230801/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.028967 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73654 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    64587 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24126 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57908 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    82689 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.028967 pyglove-0.4.3.dev20230801/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.032967 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 08:06:50.020967 pyglove-0.4.3.dev20230801/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 08:06:49.000000 pyglove-0.4.3.dev20230801/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 08:06:50.036967 pyglove-0.4.3.dev20230801/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-01 08:06:37.000000 pyglove-0.4.3.dev20230801/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.395855 pyglove-0.4.3.dev20230802/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-02 08:06:47.395855 pyglove-0.4.3.dev20230802/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-02 08:06:45.000000 pyglove-0.4.3.dev20230802/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.371855 pyglove-0.4.3.dev20230802/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.375855 pyglove-0.4.3.dev20230802/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.375855 pyglove-0.4.3.dev20230802/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.379855 pyglove-0.4.3.dev20230802/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64411 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.379855 pyglove-0.4.3.dev20230802/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.383855 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15301 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.383855 pyglove-0.4.3.dev20230802/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.387855 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73628 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64587 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24126 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/inferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/inferred_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29759 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57908 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82689 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/ref_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.387855 pyglove-0.4.3.dev20230802/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.391855 pyglove-0.4.3.dev20230802/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.391855 pyglove-0.4.3.dev20230802/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.391855 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.391855 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.395855 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.395855 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:06:47.375855 pyglove-0.4.3.dev20230802/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-02 08:06:47.000000 pyglove-0.4.3.dev20230802/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-08-02 08:06:47.000000 pyglove-0.4.3.dev20230802/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:06:47.000000 pyglove-0.4.3.dev20230802/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 08:06:47.000000 pyglove-0.4.3.dev20230802/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 08:06:47.000000 pyglove-0.4.3.dev20230802/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:06:47.395855 pyglove-0.4.3.dev20230802/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-02 08:06:33.000000 pyglove-0.4.3.dev20230802/setup.py
```

### Comparing `pyglove-0.4.3.dev20230801/LICENSE` & `pyglove-0.4.3.dev20230802/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/PKG-INFO` & `pyglove-0.4.3.dev20230802/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230801
+Version: 0.4.3.dev20230802
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230801/README.md` & `pyglove-0.4.3.dev20230802/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/detouring/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.3.dev20230802/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/base.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/custom.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/custom_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/random.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/random_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/space.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/space_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/base.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/logging.py` & `pyglove-0.4.3.dev20230802/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/logging_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     Raises:
       AttributeError: If the value cannot be inferred.
     """
 
 
 # Value marker for raising errors if a attribute does not exist or cannot
 # be computed.
-_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
+RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
 
 
 class Symbolic(
     TopologyAware,
     object_utils.JSONConvertible,
     object_utils.MaybePartial,
     object_utils.Formattable,
@@ -414,43 +414,43 @@
       True if the path exists in current sub-tree, otherwise False.
     """
     return object_utils.KeyPath.from_value(path).exists(self)
 
   def sym_get(
       self,
       path: Union[object_utils.KeyPath, str, int],
-      default: Any = object_utils.MISSING_VALUE) -> Any:
+      default: Any = RAISE_IF_NOT_FOUND) -> Any:
     """Returns a sub-node by path.
 
     NOTE: there is no `sym_set`, use `sym_rebind`.
 
     Args:
       path: A KeyPath object or equivalence.
       default: Default value if path does not exists. If absent, `KeyError` will
         be thrown.
 
     Returns:
       Value of symbolic attribute specified by path if found, otherwise the
       default value if it's specified.
 
     Raises:
-      KeyError if `path` does not exist and `default` is `pg.MISSING_VALUE`.
+      KeyError if `path` does not exist and `default` is not specified.
     """
     path = object_utils.KeyPath.from_value(path)
-    if default == object_utils.MISSING_VALUE:
+    if default is RAISE_IF_NOT_FOUND:
       return path.query(self)
     else:
       return path.get(self, default)
 
   @abc.abstractmethod
   def sym_hasattr(self, key: Union[str, int]) -> bool:
     """Returns if a symbolic attribute exists."""
 
   def sym_getattr(
-      self, key: Union[str, int], default: Any = _RAISE_IF_NOT_FOUND
+      self, key: Union[str, int], default: Any = RAISE_IF_NOT_FOUND
   ) -> Any:
     """Gets a symbolic attribute.
 
     Args:
       key: Key of symbolic attribute.
       default: Default value if attribute does not exist. If absent,
 
@@ -458,15 +458,15 @@
       Value of symbolic attribute if found, otherwise the default value
       if it's specified.
 
     Raises:
       AttributeError if `key` does not exist and `default` is not provided.
     """
     if not self.sym_hasattr(key):
-      if default is _RAISE_IF_NOT_FOUND:
+      if default is RAISE_IF_NOT_FOUND:
         raise AttributeError(
             self._error_message(
                 f'{self.__class__!r} object has no symbolic attribute {key!r}.'
             )
         )
       return default
     return self._sym_getattr(key)
@@ -477,19 +477,19 @@
         self.sym_inferred(key, pg_typing.MISSING_VALUE, **kwargs)
         != pg_typing.MISSING_VALUE
     )
 
   def sym_inferred(
       self,
       key: Union[str, int],
-      default: Any = _RAISE_IF_NOT_FOUND,
+      default: Any = RAISE_IF_NOT_FOUND,
       **kwargs,
   ) -> Any:
     """Returns the inferred value of the attribute under key."""
-    if default is _RAISE_IF_NOT_FOUND:
+    if default is RAISE_IF_NOT_FOUND:
       return self._sym_inferred(key, **kwargs)
     else:
       try:
         return self._sym_inferred(key, **kwargs)
       except Exception:  # pylint: disable=broad-exception-caught
         return default
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,14 @@
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
 
-# Special default value to detect missing keys in a Dict. Though its values is
-# the same as `base._RAISE_IF_NOT_FOUND`, they are different instances so
-# `pg.Dict` and `pg.Symbolic` could use their own instances to control error
-# raising separately.
-_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
-
-
 class Dict(dict, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic dict.
 
   ``pg.Dict`` implements a dict type whose instances are symbolically
   programmable, which is a subclass of the built-in Python ``dict`` and
   a subclass of :class:`pyglove.Symbolic`.
 
@@ -736,23 +729,23 @@
     return self.sym_values()
 
   def copy(self) -> 'Dict':
     """Overridden copy using symbolic copy."""
     return self.sym_clone(deep=False)
 
   def pop(
-      self, key: Any, default: Any = pg_typing.MISSING_VALUE
+      self, key: Any, default: Any = base.RAISE_IF_NOT_FOUND  # pylint: disable=protected-access
   ) -> Any:
     """Pops a key from current dict."""
     if key in self:
       value = self[key]
       with flags.allow_writable_accessors(True):
         del self[key]
       return value if value != pg_typing.MISSING_VALUE else default
-    if default == pg_typing.MISSING_VALUE:
+    if default is base.RAISE_IF_NOT_FOUND:
       raise KeyError(key)
     return default
 
   def popitem(self) -> Tuple[str, Any]:
     if self._value_spec is not None:
       raise ValueError(
           '\'popitem\' cannot be performed on a Dict with value spec.')
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/inferred.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/inferred_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/inferred_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
 
-# Special default value to detect missing keys in a List. Though its values is
-# the same as `base._RAISE_IF_NOT_FOUND`, they are different instances so
-# `pg.List` and `pg.Symbolic` could use their own instances to control error
-# raising separately.
-_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
-
-
 class List(list, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic list.
 
   ``pg.List`` implements a list type whose instances are symbolically
   programmable, which is a subclass of the built-in Python ``list``,
   and the subclass of ``pg.Symbolic``.
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/origin.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tracking the origin of a symbolic object."""
 
 import traceback
-from typing import Any, List, Optional
+from typing import Any, Callable, List, Optional
 
 from pyglove.core import object_utils
 from pyglove.core.symbolic import flags
 
 
 class Origin(object_utils.Formattable):
   """Class that represents the origin of a symbolic value.
@@ -82,14 +82,47 @@
 
   @property
   def source(self) -> Any:
     """Returns the source object."""
     return self._source
 
   @property
+  def root(self) -> 'Origin':
+    """Returns the root source of the origin."""
+    current = self
+    while True:
+      parent = getattr(current.source, 'sym_origin', None)
+      if parent is None:
+        break
+      current = parent
+    return current
+
+  def history(
+      self,
+      condition: Optional[Callable[['Origin'], bool]] = None) -> List['Origin']:
+    """Returns a history of origins with an optional filter.
+    
+    Args:
+      condition: An optional callable object with signature
+        (origin) -> should_list. If None, all origins will be listed.
+
+    Returns:
+      A list of filtered origin from the earliest (root) to the most recent.
+    """
+    condition = condition or (lambda o: True)
+    current = self
+    history = []
+    while current is not None:
+      if condition(current):
+        history.append(current)
+      current = getattr(current.source, 'sym_origin', None)
+    history.reverse()
+    return history
+
+  @property
   def tag(self) -> str:
     """Returns tag."""
     return self._tag
 
   @property
   def stack(self) -> Optional[List[traceback.FrameSummary]]:
     """Returns the frame summary of original stack."""
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/origin_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,49 @@
     self.assertEqual(len(o.stack), 3)
     self.assertIsNotNone(o.stacktrace)
 
     flags.set_origin_stacktrace_limit(2)
     o = Origin(a, '__init__', stacktrace=True)
     self.assertEqual(len(o.stack), 2)
 
+  def test_root(self):
+    a = Dict(a=1)
+    b = Dict(b=2)
+    c = Dict(c=3)
+
+    c.sym_setorigin(b, 'foo')
+    b.sym_setorigin(a, 'bar')
+    self.assertIs(c.sym_origin.root.source, a)
+
+  def test_history(self):
+    a = Dict(a=1)
+    b = Dict(b=2)
+    c = Dict(c=3)
+
+    c.sym_setorigin(b, 'foo')
+    b.sym_setorigin(a, 'bar')
+    self.assertEqual(
+        c.sym_origin.history(),
+        [
+            Origin(a, 'bar'),
+            Origin(b, 'foo'),
+        ])
+
+    self.assertEqual(
+        c.sym_origin.history(lambda o: o.tag == 'foo'),
+        [
+            Origin(b, 'foo'),
+        ])
+
+    self.assertEqual(
+        c.sym_origin.history(lambda o: o.tag == 'bar'),
+        [
+            Origin(a, 'bar'),
+        ])
+
   def test_eq_ne(self):
     a = Dict(a=1)
     self.assertEqual(Origin(None, '__init__'), Origin(None, '__init__'))
     self.assertEqual(Origin(a, 'builder'), Origin(a, 'builder'))
     self.assertNotEqual(Origin(a, 'builder'), a)
     self.assertNotEqual(Origin(a, 'builder'), Origin(a, 'return'))
     self.assertNotEqual(Origin(a, 'builder'), Origin(Dict(a=1), 'builder'))
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/ref.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/ref_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/ref_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/early_stopping.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/generic.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/generic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/generic_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/generic_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.3.dev20230802/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.3.dev20230802/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.3.dev20230802/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.3.dev20230801
+Version: 0.4.3.dev20230802
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.3.dev20230801/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.3.dev20230802/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.3.dev20230801/setup.py` & `pyglove-0.4.3.dev20230802/setup.py`

 * *Files identical despite different names*

