# Comparing `tmp/fortlab-1.1.1.tar.gz` & `tmp/fortlab-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortlab-1.1.1.tar", last modified: Thu Aug  3 14:32:44 2023, max compression
+gzip compressed data, was "fortlab-1.1.2.tar", last modified: Thu Aug  3 14:50:21 2023, max compression
```

## Comparing `fortlab-1.1.1.tar` & `fortlab-1.1.2.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.616001 fortlab-1.1.1/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1070 2020-06-30 17:42:41.000000 fortlab-1.1.1/LICENSE
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      834 2023-08-03 14:32:44.615997 fortlab-1.1.1/PKG-INFO
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1038 2022-05-16 12:38:00.000000 fortlab-1.1.1/README.rst
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.356006 fortlab-1.1.1/fortlab/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       51 2021-10-15 18:34:54.000000 fortlab-1.1.1/fortlab/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      190 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/__main__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.373002 fortlab-1.1.1/fortlab/kernel/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       46 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/__init__.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)    42214 2022-10-04 16:06:48.000000 fortlab-1.1.1/fortlab/kernel/kernelgen.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.377000 fortlab-1.1.1/fortlab/kernel/plugins/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.381003 fortlab-1.1.1/fortlab/kernel/plugins/coverage/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/coverage/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10697 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/coverage/gen_coverage_files.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.385999 fortlab-1.1.1/fortlab/kernel/plugins/debug/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/debug/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7936 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/debug/debug_add_sum.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.423006 fortlab-1.1.1/fortlab/kernel/plugins/gencore/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    26368 2020-07-28 20:08:40.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_driver.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    15849 2020-07-28 20:09:55.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_kernel_callsite_file.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1076 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_kernel_files.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    60653 2021-05-03 15:36:44.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_state_callsite_file.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    25274 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_type.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    36736 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_module.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    34382 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_parentblock.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    25356 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_type.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    32870 2021-05-03 15:36:44.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_write_in_module.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19040 2020-07-24 15:08:22.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gencore_subr.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19656 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/gencore/gencore_utils.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.428999 fortlab-1.1.1/fortlab/kernel/plugins/perturb/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/perturb/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1318 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/perturb/perturb_kernel_callsite_file.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.433007 fortlab-1.1.1/fortlab/kernel/plugins/simple_timing/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/simple_timing/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     8287 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/simple_timing/simple_timing.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.453009 fortlab-1.1.1/fortlab/kernel/plugins/verification/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7418 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_callsite_file.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    31145 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_subr.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    43091 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_type.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7350 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_typedecl_in_module.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3404 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_typedecl_in_parentblock.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6464 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_utils.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    17140 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/kgextra.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    56972 2021-07-08 13:57:12.000000 fortlab-1.1.1/fortlab/kggenfile.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      264 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/kgplugin.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    11492 2022-09-29 22:02:46.000000 fortlab-1.1.1/fortlab/kgutils.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1444 2023-08-03 14:29:41.000000 fortlab-1.1.1/fortlab/main.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.511999 fortlab-1.1.1/fortlab/resolver/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)   255503 2021-03-18 23:02:58.000000 fortlab-1.1.1/fortlab/resolver/Fortran2003.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       39 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/resolver/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7921 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/resolver/api.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    81328 2021-07-12 00:16:03.000000 fortlab-1.1.1/fortlab/resolver/base_classes.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    57882 2021-07-09 14:46:45.000000 fortlab-1.1.1/fortlab/resolver/block_statements.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)    10723 2022-09-30 19:00:36.000000 fortlab-1.1.1/fortlab/resolver/kganalyze.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4032 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/resolver/kgintrinsics.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)    17196 2022-10-01 15:01:24.000000 fortlab-1.1.1/fortlab/resolver/kgparse.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    52121 2022-10-01 15:01:52.000000 fortlab-1.1.1/fortlab/resolver/kgsearch.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)    58357 2022-10-04 16:10:48.000000 fortlab-1.1.1/fortlab/resolver/main.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6011 2021-01-06 20:07:39.000000 fortlab-1.1.1/fortlab/resolver/parsefortran.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    17379 2021-07-09 14:43:12.000000 fortlab-1.1.1/fortlab/resolver/pattern_tools.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    51233 2022-02-11 19:30:07.000000 fortlab-1.1.1/fortlab/resolver/readfortran.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3960 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/resolver/sourceinfo.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    14400 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/resolver/splitline.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)   106345 2022-05-16 15:12:03.000000 fortlab-1.1.1/fortlab/resolver/statements.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    26949 2021-07-12 00:16:13.000000 fortlab-1.1.1/fortlab/resolver/typedecl_statements.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     9974 2022-05-16 13:02:16.000000 fortlab-1.1.1/fortlab/resolver/utils.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.516998 fortlab-1.1.1/fortlab/scanner/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       82 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.523002 fortlab-1.1.1/fortlab/scanner/compile/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       42 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/compile/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10194 2023-08-03 14:29:41.000000 fortlab-1.1.1/fortlab/scanner/compile/kgcompiler.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     8437 2022-10-01 15:07:05.000000 fortlab-1.1.1/fortlab/scanner/compile/option.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10664 2022-10-01 15:06:18.000000 fortlab-1.1.1/fortlab/scanner/main.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.530003 fortlab-1.1.1/fortlab/scanner/timing/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      117 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/timing/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.532999 fortlab-1.1.1/fortlab/scanner/timing/plugins/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/timing/plugins/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.536000 fortlab-1.1.1/fortlab/scanner/timing/plugins/gencore/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/timing/plugins/gencore/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    29539 2020-06-30 17:42:41.000000 fortlab-1.1.1/fortlab/scanner/timing/plugins/gencore/gen_etime_files.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)    11706 2022-10-01 15:07:48.000000 fortlab-1.1.1/fortlab/scanner/timing/timinggen.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     5515 2022-10-01 15:09:03.000000 fortlab-1.1.1/fortlab/scanner/timing/timingmodel.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.541001 fortlab-1.1.1/fortlab/state/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       44 2020-07-24 15:08:23.000000 fortlab-1.1.1/fortlab/state/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      433 2022-10-01 15:10:02.000000 fortlab-1.1.1/fortlab/state/stategen.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.546001 fortlab-1.1.1/fortlab/vargen/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       44 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.549001 fortlab-1.1.1/fortlab/vargen/plugins/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/__init__.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.553000 fortlab-1.1.1/fortlab/vargen/plugins/coverage/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/coverage/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10697 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/coverage/gen_coverage_files.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.557002 fortlab-1.1.1/fortlab/vargen/plugins/debug/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/debug/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7936 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/debug/debug_add_sum.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.573999 fortlab-1.1.1/fortlab/vargen/plugins/gencore/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    13473 2021-07-08 18:53:57.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_kernel_callsite_file.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1076 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_kernel_files.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    28611 2021-07-12 12:43:39.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_typedecl_in_module.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    35798 2021-07-09 17:57:23.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_typedecl_in_parentblock.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19935 2021-07-12 12:41:48.000000 fortlab-1.1.1/fortlab/vargen/plugins/gencore/gencore_utils.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.578002 fortlab-1.1.1/fortlab/vargen/plugins/genvarlist/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:39:37.000000 fortlab-1.1.1/fortlab/vargen/plugins/genvarlist/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     9529 2021-07-12 00:26:16.000000 fortlab-1.1.1/fortlab/vargen/plugins/genvarlist/genvarlist.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.582999 fortlab-1.1.1/fortlab/vargen/plugins/perturb/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/perturb/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1318 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/perturb/perturb_kernel_callsite_file.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.586998 fortlab-1.1.1/fortlab/vargen/plugins/simple_timing/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/simple_timing/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     8287 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/simple_timing/simple_timing.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.605003 fortlab-1.1.1/fortlab/vargen/plugins/verification/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/__init__.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7418 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_callsite_file.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    31145 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_subr.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    43091 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_type.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7350 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_typedecl_in_module.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3404 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_typedecl_in_parentblock.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6464 2021-07-06 17:35:26.000000 fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_utils.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     7914 2022-10-01 15:10:19.000000 fortlab-1.1.1/fortlab/vargen/vargen.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.368005 fortlab-1.1.1/fortlab.egg-info/
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      834 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/PKG-INFO
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     4239 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/SOURCES.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)        1 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/dependency_links.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       89 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/entry_points.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       34 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/requires.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)        8 2023-08-03 14:32:44.000000 fortlab-1.1.1/fortlab.egg-info/top_level.txt
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       38 2023-08-03 14:32:44.617002 fortlab-1.1.1/setup.cfg
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1535 2022-09-30 18:59:27.000000 fortlab-1.1.1/setup.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:32:44.612999 fortlab-1.1.1/tests/
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6283 2021-05-04 17:54:20.000000 fortlab-1.1.1/tests/test_basic.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4514 2020-11-05 21:45:17.000000 fortlab-1.1.1/tests/test_e3sm.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4931 2020-11-14 00:43:56.000000 fortlab-1.1.1/tests/test_e3sm_mpaso.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.172720 fortlab-1.1.2/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1070 2020-06-30 17:42:41.000000 fortlab-1.1.2/LICENSE
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      834 2023-08-03 14:50:21.171728 fortlab-1.1.2/PKG-INFO
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1038 2022-05-16 12:38:00.000000 fortlab-1.1.2/README.rst
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:20.986719 fortlab-1.1.2/fortlab/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       51 2021-10-15 18:34:54.000000 fortlab-1.1.2/fortlab/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      190 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/__main__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:20.999725 fortlab-1.1.2/fortlab/kernel/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       46 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/__init__.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)    42214 2022-10-04 16:06:48.000000 fortlab-1.1.2/fortlab/kernel/kernelgen.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.002722 fortlab-1.1.2/fortlab/kernel/plugins/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.005722 fortlab-1.1.2/fortlab/kernel/plugins/coverage/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/coverage/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10697 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/coverage/gen_coverage_files.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.009720 fortlab-1.1.2/fortlab/kernel/plugins/debug/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/debug/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7936 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/debug/debug_add_sum.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.034724 fortlab-1.1.2/fortlab/kernel/plugins/gencore/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    26368 2020-07-28 20:08:40.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_driver.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    15849 2020-07-28 20:09:55.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_kernel_callsite_file.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1076 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_kernel_files.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    60653 2021-05-03 15:36:44.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_state_callsite_file.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    25274 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_type.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    36736 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_module.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    34382 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_parentblock.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    25356 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_type.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    32870 2021-05-03 15:36:44.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_write_in_module.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19040 2020-07-24 15:08:22.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gencore_subr.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19656 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/gencore/gencore_utils.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.038720 fortlab-1.1.2/fortlab/kernel/plugins/perturb/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/perturb/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1318 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/perturb/perturb_kernel_callsite_file.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.041723 fortlab-1.1.2/fortlab/kernel/plugins/simple_timing/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/simple_timing/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     8287 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/simple_timing/simple_timing.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.055720 fortlab-1.1.2/fortlab/kernel/plugins/verification/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7418 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_callsite_file.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    31145 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_subr.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    43091 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_type.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7350 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_typedecl_in_module.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3404 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_typedecl_in_parentblock.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6464 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_utils.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    17140 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/kgextra.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    56972 2021-07-08 13:57:12.000000 fortlab-1.1.2/fortlab/kggenfile.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      264 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/kgplugin.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    11492 2022-09-29 22:02:46.000000 fortlab-1.1.2/fortlab/kgutils.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1444 2023-08-03 14:48:59.000000 fortlab-1.1.2/fortlab/main.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.092724 fortlab-1.1.2/fortlab/resolver/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)   255503 2021-03-18 23:02:58.000000 fortlab-1.1.2/fortlab/resolver/Fortran2003.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       39 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/resolver/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7921 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/resolver/api.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    81328 2021-07-12 00:16:03.000000 fortlab-1.1.2/fortlab/resolver/base_classes.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    57882 2021-07-09 14:46:45.000000 fortlab-1.1.2/fortlab/resolver/block_statements.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)    10723 2022-09-30 19:00:36.000000 fortlab-1.1.2/fortlab/resolver/kganalyze.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4032 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/resolver/kgintrinsics.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)    17196 2022-10-01 15:01:24.000000 fortlab-1.1.2/fortlab/resolver/kgparse.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    52121 2022-10-01 15:01:52.000000 fortlab-1.1.2/fortlab/resolver/kgsearch.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)    58357 2022-10-04 16:10:48.000000 fortlab-1.1.2/fortlab/resolver/main.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6011 2021-01-06 20:07:39.000000 fortlab-1.1.2/fortlab/resolver/parsefortran.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    17379 2021-07-09 14:43:12.000000 fortlab-1.1.2/fortlab/resolver/pattern_tools.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    51233 2022-02-11 19:30:07.000000 fortlab-1.1.2/fortlab/resolver/readfortran.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3960 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/resolver/sourceinfo.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    14400 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/resolver/splitline.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)   106345 2022-05-16 15:12:03.000000 fortlab-1.1.2/fortlab/resolver/statements.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    26949 2021-07-12 00:16:13.000000 fortlab-1.1.2/fortlab/resolver/typedecl_statements.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     9974 2022-05-16 13:02:16.000000 fortlab-1.1.2/fortlab/resolver/utils.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.096737 fortlab-1.1.2/fortlab/scanner/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       82 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.102720 fortlab-1.1.2/fortlab/scanner/compile/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       42 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/compile/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10194 2023-08-03 14:29:41.000000 fortlab-1.1.2/fortlab/scanner/compile/kgcompiler.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     8437 2022-10-01 15:07:05.000000 fortlab-1.1.2/fortlab/scanner/compile/option.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10664 2022-10-01 15:06:18.000000 fortlab-1.1.2/fortlab/scanner/main.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.107727 fortlab-1.1.2/fortlab/scanner/timing/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      117 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/timing/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.109722 fortlab-1.1.2/fortlab/scanner/timing/plugins/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/timing/plugins/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.112722 fortlab-1.1.2/fortlab/scanner/timing/plugins/gencore/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/timing/plugins/gencore/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    29539 2020-06-30 17:42:41.000000 fortlab-1.1.2/fortlab/scanner/timing/plugins/gencore/gen_etime_files.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)    11706 2022-10-01 15:07:48.000000 fortlab-1.1.2/fortlab/scanner/timing/timinggen.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     5574 2023-08-03 14:48:36.000000 fortlab-1.1.2/fortlab/scanner/timing/timingmodel.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.116720 fortlab-1.1.2/fortlab/state/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       44 2020-07-24 15:08:23.000000 fortlab-1.1.2/fortlab/state/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      433 2022-10-01 15:10:02.000000 fortlab-1.1.2/fortlab/state/stategen.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.120718 fortlab-1.1.2/fortlab/vargen/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       44 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.121724 fortlab-1.1.2/fortlab/vargen/plugins/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/__init__.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.124730 fortlab-1.1.2/fortlab/vargen/plugins/coverage/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/coverage/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    10697 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/coverage/gen_coverage_files.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.128721 fortlab-1.1.2/fortlab/vargen/plugins/debug/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/debug/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7936 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/debug/debug_add_sum.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.139723 fortlab-1.1.2/fortlab/vargen/plugins/gencore/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    13473 2021-07-08 18:53:57.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_kernel_callsite_file.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1076 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_kernel_files.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    28611 2021-07-12 12:43:39.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_typedecl_in_module.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    35798 2021-07-09 17:57:23.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_typedecl_in_parentblock.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    19935 2021-07-12 12:41:48.000000 fortlab-1.1.2/fortlab/vargen/plugins/gencore/gencore_utils.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.143717 fortlab-1.1.2/fortlab/vargen/plugins/genvarlist/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:39:37.000000 fortlab-1.1.2/fortlab/vargen/plugins/genvarlist/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     9529 2021-07-12 00:26:16.000000 fortlab-1.1.2/fortlab/vargen/plugins/genvarlist/genvarlist.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.146721 fortlab-1.1.2/fortlab/vargen/plugins/perturb/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/perturb/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1318 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/perturb/perturb_kernel_callsite_file.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.149727 fortlab-1.1.2/fortlab/vargen/plugins/simple_timing/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/simple_timing/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     8287 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/simple_timing/simple_timing.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.163723 fortlab-1.1.2/fortlab/vargen/plugins/verification/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)        0 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/__init__.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7418 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_callsite_file.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    31145 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_subr.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)    43091 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_type.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     7350 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_typedecl_in_module.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     3404 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_typedecl_in_parentblock.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6464 2021-07-06 17:35:26.000000 fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_utils.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     7914 2022-10-01 15:10:19.000000 fortlab-1.1.2/fortlab/vargen/vargen.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:20.996722 fortlab-1.1.2/fortlab.egg-info/
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      834 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/PKG-INFO
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     4239 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/SOURCES.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)        1 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/dependency_links.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       89 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/entry_points.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       34 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/requires.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)        8 2023-08-03 14:50:20.000000 fortlab-1.1.2/fortlab.egg-info/top_level.txt
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       38 2023-08-03 14:50:21.172724 fortlab-1.1.2/setup.cfg
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1535 2022-09-30 18:59:27.000000 fortlab-1.1.2/setup.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:50:21.169730 fortlab-1.1.2/tests/
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     6283 2021-05-04 17:54:20.000000 fortlab-1.1.2/tests/test_basic.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4514 2020-11-05 21:45:17.000000 fortlab-1.1.2/tests/test_e3sm.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     4931 2020-11-14 00:43:56.000000 fortlab-1.1.2/tests/test_e3sm_mpaso.py
```

### Comparing `fortlab-1.1.1/LICENSE` & `fortlab-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/PKG-INFO` & `fortlab-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortlab
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fortran Kernel and Analysis Framework
 Author: Youngsung Kim
 Author-email: youngsung.kim.act2@gmail.com
 Project-URL: Bug Reports, https://github.com/grnydawn/fortlab/issues
 Project-URL: Source, https://github.com/grnydawn/fortlab
 Keywords: microapp fortlab
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fortlab-1.1.1/README.rst` & `fortlab-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/kernelgen.py` & `fortlab-1.1.2/fortlab/kernel/kernelgen.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/coverage/gen_coverage_files.py` & `fortlab-1.1.2/fortlab/kernel/plugins/coverage/gen_coverage_files.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/debug/debug_add_sum.py` & `fortlab-1.1.2/fortlab/kernel/plugins/debug/debug_add_sum.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_driver.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_driver.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_kernel_callsite_file.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_kernel_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_kernel_files.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_kernel_files.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_state_callsite_file.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_state_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_type.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_type.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_module.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_module.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_parentblock.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_parentblock.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_typedecl_in_type.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_typedecl_in_type.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gen_write_in_module.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gen_write_in_module.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gencore_subr.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gencore_subr.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/gencore/gencore_utils.py` & `fortlab-1.1.2/fortlab/kernel/plugins/gencore/gencore_utils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/perturb/perturb_kernel_callsite_file.py` & `fortlab-1.1.2/fortlab/kernel/plugins/perturb/perturb_kernel_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/simple_timing/simple_timing.py` & `fortlab-1.1.2/fortlab/kernel/plugins/simple_timing/simple_timing.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_callsite_file.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_subr.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_subr.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_type.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_type.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_typedecl_in_module.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_typedecl_in_module.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_typedecl_in_parentblock.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_typedecl_in_parentblock.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kernel/plugins/verification/verify_utils.py` & `fortlab-1.1.2/fortlab/kernel/plugins/verification/verify_utils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kgextra.py` & `fortlab-1.1.2/fortlab/kgextra.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kggenfile.py` & `fortlab-1.1.2/fortlab/kggenfile.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/kgutils.py` & `fortlab-1.1.2/fortlab/kgutils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/main.py` & `fortlab-1.1.2/fortlab/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fortlab.resolver import FortranNameResolver
 from fortlab.kernel import FortranKernelGenerator
 from fortlab.state import FortranStateGenerator
 from fortlab.vargen import FortranVariableAnalyzer
 
 class Fortlab(Project):
     _name_ = "fortlab"
-    _version_ = "1.1.1"
+    _version_ = "1.1.2"
     _description_ = "Fortran Kernel and Analysis Framework"
     _long_description_ = "Tools for Analysis of Fortran Application and Source code"
     _author_ = "Youngsung Kim"
     _author_email_ = "youngsung.kim.act2@gmail.com"
     _url_ = "https://github.com/grnydawn/fortlab"
     _builtin_apps_ = [MicroappBuildScanner, MicroappRunScanner,
                       FortranCompilerOption, FortranNameResolver,
```

### Comparing `fortlab-1.1.1/fortlab/resolver/Fortran2003.py` & `fortlab-1.1.2/fortlab/resolver/Fortran2003.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/api.py` & `fortlab-1.1.2/fortlab/resolver/api.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/base_classes.py` & `fortlab-1.1.2/fortlab/resolver/base_classes.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/block_statements.py` & `fortlab-1.1.2/fortlab/resolver/block_statements.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/kganalyze.py` & `fortlab-1.1.2/fortlab/resolver/kganalyze.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/kgintrinsics.py` & `fortlab-1.1.2/fortlab/resolver/kgintrinsics.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/kgparse.py` & `fortlab-1.1.2/fortlab/resolver/kgparse.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/kgsearch.py` & `fortlab-1.1.2/fortlab/resolver/kgsearch.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/main.py` & `fortlab-1.1.2/fortlab/resolver/main.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/parsefortran.py` & `fortlab-1.1.2/fortlab/resolver/parsefortran.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/pattern_tools.py` & `fortlab-1.1.2/fortlab/resolver/pattern_tools.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/readfortran.py` & `fortlab-1.1.2/fortlab/resolver/readfortran.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/sourceinfo.py` & `fortlab-1.1.2/fortlab/resolver/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/splitline.py` & `fortlab-1.1.2/fortlab/resolver/splitline.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/statements.py` & `fortlab-1.1.2/fortlab/resolver/statements.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/typedecl_statements.py` & `fortlab-1.1.2/fortlab/resolver/typedecl_statements.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/resolver/utils.py` & `fortlab-1.1.2/fortlab/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/compile/kgcompiler.py` & `fortlab-1.1.2/fortlab/scanner/compile/kgcompiler.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/compile/option.py` & `fortlab-1.1.2/fortlab/scanner/compile/option.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/main.py` & `fortlab-1.1.2/fortlab/scanner/main.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/timing/plugins/gencore/gen_etime_files.py` & `fortlab-1.1.2/fortlab/scanner/timing/plugins/gencore/gen_etime_files.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/timing/timinggen.py` & `fortlab-1.1.2/fortlab/scanner/timing/timinggen.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/scanner/timing/timingmodel.py` & `fortlab-1.1.2/fortlab/scanner/timing/timingmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """Microapp compiler inspector"""
 
 import os, shutil, multiprocessing
 
-from collections import Mapping
+try:
+    from collections import Mapping
+except:
+    from collections.abc import Mapping
+
+
 
 from microapp import App, register_appclass, unregister_appclass
 
 def _update(d, u):
     for k, v in u.items():
         if isinstance(v, Mapping):
             r = _update(d.get(k, {}), v)
```

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/coverage/gen_coverage_files.py` & `fortlab-1.1.2/fortlab/vargen/plugins/coverage/gen_coverage_files.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/debug/debug_add_sum.py` & `fortlab-1.1.2/fortlab/vargen/plugins/debug/debug_add_sum.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_kernel_callsite_file.py` & `fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_kernel_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_kernel_files.py` & `fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_kernel_files.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_typedecl_in_module.py` & `fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_typedecl_in_module.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/gencore/gen_typedecl_in_parentblock.py` & `fortlab-1.1.2/fortlab/vargen/plugins/gencore/gen_typedecl_in_parentblock.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/gencore/gencore_utils.py` & `fortlab-1.1.2/fortlab/vargen/plugins/gencore/gencore_utils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/genvarlist/genvarlist.py` & `fortlab-1.1.2/fortlab/vargen/plugins/genvarlist/genvarlist.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/perturb/perturb_kernel_callsite_file.py` & `fortlab-1.1.2/fortlab/vargen/plugins/perturb/perturb_kernel_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/simple_timing/simple_timing.py` & `fortlab-1.1.2/fortlab/vargen/plugins/simple_timing/simple_timing.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_callsite_file.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_callsite_file.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_subr.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_subr.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_type.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_type.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_typedecl_in_module.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_typedecl_in_module.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_typedecl_in_parentblock.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_typedecl_in_parentblock.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/plugins/verification/verify_utils.py` & `fortlab-1.1.2/fortlab/vargen/plugins/verification/verify_utils.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab/vargen/vargen.py` & `fortlab-1.1.2/fortlab/vargen/vargen.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/fortlab.egg-info/PKG-INFO` & `fortlab-1.1.2/fortlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortlab
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fortran Kernel and Analysis Framework
 Author: Youngsung Kim
 Author-email: youngsung.kim.act2@gmail.com
 Project-URL: Bug Reports, https://github.com/grnydawn/fortlab/issues
 Project-URL: Source, https://github.com/grnydawn/fortlab
 Keywords: microapp fortlab
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fortlab-1.1.1/fortlab.egg-info/SOURCES.txt` & `fortlab-1.1.2/fortlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/setup.py` & `fortlab-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/tests/test_basic.py` & `fortlab-1.1.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/tests/test_e3sm.py` & `fortlab-1.1.2/tests/test_e3sm.py`

 * *Files identical despite different names*

### Comparing `fortlab-1.1.1/tests/test_e3sm_mpaso.py` & `fortlab-1.1.2/tests/test_e3sm_mpaso.py`

 * *Files identical despite different names*

