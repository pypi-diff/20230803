# Comparing `tmp/cosmosis-3.0.3.tar.gz` & `tmp/cosmosis-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-3.0.3.tar", last modified: Fri Jul 28 18:31:33 2023, max compression
+gzip compressed data, was "cosmosis-3.1.tar", last modified: Thu Aug  3 11:07:51 2023, max compression
```

## Comparing `cosmosis-3.0.3.tar` & `cosmosis-3.1.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.566161 cosmosis-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-28 18:31:29.000000 cosmosis-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-28 18:31:29.000000 cosmosis-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 18:31:33.566161 cosmosis-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-28 18:31:29.000000 cosmosis-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.538161 cosmosis-3.0.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-campaign
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-28 18:31:29.000000 cosmosis-3.0.3/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/astropy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.546161 cosmosis-3.0.3/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49133 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    31638 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    55669 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2176 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.550161 cosmosis-3.0.3/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7516 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6642 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4745 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4666 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7323 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.554161 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   107766 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.558161 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2017 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4468 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.562161 cosmosis-3.0.3/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/campaign.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example-priors.ini
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example-values.ini
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example.ini
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/example_module4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.566161 cosmosis-3.0.3/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 18:31:29.000000 cosmosis-3.0.3/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:33.542161 cosmosis-3.0.3/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:31:33.000000 cosmosis-3.0.3/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 18:31:29.000000 cosmosis-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:31:33.566161 cosmosis-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-28 18:31:29.000000 cosmosis-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.042641 cosmosis-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-03 11:07:44.000000 cosmosis-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-03 11:07:44.000000 cosmosis-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 11:07:51.042641 cosmosis-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 11:07:44.000000 cosmosis-3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.022641 cosmosis-3.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-08-03 11:07:44.000000 cosmosis-3.1/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.022641 cosmosis-3.1/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.022641 cosmosis-3.1/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.026641 cosmosis-3.1/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.026641 cosmosis-3.1/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22922 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.026641 cosmosis-3.1/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.026641 cosmosis-3.1/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5392 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16175 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50217 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31638 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55670 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2766 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7516 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6642 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4745 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4370 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4888 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4666 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.030641 cosmosis-3.1/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7323 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   107766 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4151 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.034641 cosmosis-3.1/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2017 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4468 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.038641 cosmosis-3.1/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/example_module4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.042641 cosmosis-3.1/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 11:07:44.000000 cosmosis-3.1/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:51.022641 cosmosis-3.1/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 11:07:50.000000 cosmosis-3.1/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-08-03 11:07:50.000000 cosmosis-3.1/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:07:50.000000 cosmosis-3.1/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 11:07:50.000000 cosmosis-3.1/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 11:07:50.000000 cosmosis-3.1/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 11:07:44.000000 cosmosis-3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:07:51.042641 cosmosis-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-08-03 11:07:44.000000 cosmosis-3.1/setup.py
```

### Comparing `cosmosis-3.0.3/LICENSE` & `cosmosis-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/MANIFEST.in` & `cosmosis-3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/bin/cosmosis-configure` & `cosmosis-3.1/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/bin/cosmosis-extract` & `cosmosis-3.1/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/bin/cosmosis-sample-fisher` & `cosmosis-3.1/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/__init__.py` & `cosmosis-3.1/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/campaign.py` & `cosmosis-3.1/cosmosis/campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/config/compilers.mk` & `cosmosis-3.1/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/configure.py` & `cosmosis-3.1/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/constants.py` & `cosmosis-3.1/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/Makefile` & `cosmosis-3.1/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.1/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/c_datablock.h` & `cosmosis-3.1/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/clamp.hh` & `cosmosis-3.1/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.1/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.1/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.1/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.1/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.1/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.1/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.1/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.1/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.1/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/datablock.cc` & `cosmosis-3.1/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/datablock.hh` & `cosmosis-3.1/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.1/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.1/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/datablock_status.h` & `cosmosis-3.1/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/entry.cc` & `cosmosis-3.1/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/entry.hh` & `cosmosis-3.1/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/generate_sections.py` & `cosmosis-3.1/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/handler.c` & `cosmosis-3.1/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/ndarray.hh` & `cosmosis-3.1/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/section.cc` & `cosmosis-3.1/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/section.hh` & `cosmosis-3.1/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/section_names.h` & `cosmosis-3.1/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/datablock/section_names.txt` & `cosmosis-3.1/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/gaussian_likelihood.py` & `cosmosis-3.1/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/main.py` & `cosmosis-3.1/cosmosis/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/__init__.py` & `cosmosis-3.1/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/astropy_output.py` & `cosmosis-3.1/cosmosis/output/astropy_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/cosmomc_output.py` & `cosmosis-3.1/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/fits_output.py` & `cosmosis-3.1/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/in_memory_output.py` & `cosmosis-3.1/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/null_output.py` & `cosmosis-3.1/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/output_base.py` & `cosmosis-3.1/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/text_output.py` & `cosmosis-3.1/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/output/utils.py` & `cosmosis-3.1/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/plotting/chain_plots.py` & `cosmosis-3.1/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/plotting/grid_plots.py` & `cosmosis-3.1/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/plotting/kde.py` & `cosmosis-3.1/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/plotting/plotter.py` & `cosmosis-3.1/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocess.py` & `cosmosis-3.1/cosmosis/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/__init__.py` & `cosmosis-3.1/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.1/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/density.py` & `cosmosis-3.1/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/elements.py` & `cosmosis-3.1/cosmosis/postprocessing/elements.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 class PostProcessorElement(Loadable):
     def __init__(self, data_source, **options):
         super(PostProcessorElement,self).__init__()
         self.source = data_source
         self.options = {}
         self.options.update(options)
 
+    def reduced_col(self, name, stacked=True):
+        return self.source.reduced_col(name, stacked=stacked)
+
     def get_output(self, name):
         return self.source.outputs.get(name)
 
     def filename(self, ftype, base, *bases):
         if bases:
             base = base + "_" + ("_".join(bases))
         output_dir = self.options.get("outdir", ".")
@@ -60,17 +63,14 @@
         print("I do not know how to produce some results for this kind of data")
         return []
 
     def finalize(self):
         pass
 
 class MCMCPostProcessorElement(PostProcessorElement):
-    def reduced_col(self, name, stacked=True):
-        return self.source.reduced_col(name, stacked=stacked)
-
     def posterior_sample(self):
         return self.source.posterior_sample()
 
 class WeightedMCMCPostProcessorElement(MCMCPostProcessorElement):
     def weight_col(self):
         return self.source.weight_col()
```

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/inputs.py` & `cosmosis-3.1/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/latex.ini` & `cosmosis-3.1/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.1/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/main.py` & `cosmosis-3.1/cosmosis/postprocessing/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/outputs.py` & `cosmosis-3.1/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/plots.py` & `cosmosis-3.1/cosmosis/postprocessing/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1326,7 +1326,39 @@
 
 class PolychordPlots2D(PolychordPlots):
     def run(self):
         warnings.warn('Polychord2D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
         return self.run_2d()
     def smooth_likelihood(self, x, y, xname, yname):
         return self.smooth_likelihood_2d(x, y, xname, yname)
+
+
+class AprioriPlots1D(Plots):
+    def run(self):
+        cols = self.source.colnames[:]
+        filenames = []
+        for col in cols:
+            fig, filename = self.figure(col)
+            pylab.hist(self.reduced_col(col), bins=30, histtype='step')
+            pylab.xlabel(self.latex(col))
+            pylab.ylabel('Number of samples')
+            filenames.append(filename)
+        return filenames
+
+class AprioriPlots2D(Plots):
+    def run(self):
+        filenames = []
+        post = self.source.get_col("post")
+        for col1, col2 in self.parameter_pairs():
+            fig, filename = self.figure("2D", col1, col2)
+            x1 = self.source.get_col(col1)
+            x2 = self.source.get_col(col2)
+            good = np.isfinite(post)
+            bad = ~good
+            if np.any(good):
+                pylab.plot(x1[good], x2[good], '.')
+            if np.any(bad):
+                pylab.plot(x1[bad], x2[bad], 'x')
+            pylab.xlabel(self.latex(col1))
+            pylab.ylabel(self.latex(col2))
+            filenames.append(filename)
+        return filenames
```

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.1/cosmosis/postprocessing/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,7 +382,23 @@
 class StarProcessor(PostProcessor):
 	sampler='star'
 	elements=[
 		plots.StarPlots,
 	]
 
 
+class AprioriProcessor(PostProcessor):
+	sampler='apriori'
+	elements=[
+		plots.AprioriPlots1D,
+		plots.AprioriPlots2D,
+	]
+	def reduced_col(self, name, stacked=True):
+		cols = self.get_col(name, stacked=False)
+		likes = self.get_col("post", stacked=False)
+		cols = [col[np.isfinite(like)] for col, like in zip(cols, likes)]
+
+		if stacked:
+			return np.concatenate(cols)
+		else:
+			return cols
+
```

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.1/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/reruns.py` & `cosmosis-3.1/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/statistics.py` & `cosmosis-3.1/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/postprocessing/utils.py` & `cosmosis-3.1/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/analytics.py` & `cosmosis-3.1/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/attribution.py` & `cosmosis-3.1/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/config.py` & `cosmosis-3.1/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/declare.py` & `cosmosis-3.1/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.1/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/logs.py` & `cosmosis-3.1/cosmosis/runtime/logs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/memmon.py` & `cosmosis-3.1/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/module.py` & `cosmosis-3.1/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.1/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/parameter.py` & `cosmosis-3.1/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/pipeline.py` & `cosmosis-3.1/cosmosis/runtime/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
                     data_package.print_log()
                     logs.noisy("Because you set debug verbosity I printed a log of "
                                    "all access to data printed above. "
                                    "Look for the word 'FAIL' \n"
                                    "Though the error message could also be "
                                    "somewhere above that.\n")
 
-                logs.warning("Error running pipeline ({status}). Returning zero likelihood. Error may be above.")
+                logs.warning(f"Error running pipeline ({status}). Returning zero likelihood. Error may be above.")
                 if not logs.is_enabled_for(logs.logging.DEBUG):
                     logs.warning("Set log level to 'debug' for more info.")
                 return None
 
             # If we are using a fast/slow split (and we are not already running on a cached subset)
             # Then see if it wants to cache these results
             if self.slow_subspace_cache and first_module==0:
```

### Comparing `cosmosis-3.0.3/cosmosis/runtime/prior.py` & `cosmosis-3.1/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/runtime/process_pool.py` & `cosmosis-3.1/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/__init__.py` & `cosmosis-3.1/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.1/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.1/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.1/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,27 +16,39 @@
     return (r.prior, r.post, r.extra)
 
 
 
 
 class AprioriSampler(ParallelSampler):
     parallel_output = False
+    supports_resume = True
     sampler_outputs = [("prior", float), ("post", float)]
 
     def config(self):
         global sampler
         sampler = self
 
         self.converged = False
         self.save_name = self.read_ini("save", str, "")
         self.nsample = self.read_ini("nsample", int, 1)
+        self.n = 0
+
+    def resume(self):
+        if self.output.resumed:
+            data = np.genfromtxt(self.output._filename, invalid_raise=False)
+            self.n = len(data)
+            if self.n >= self.nsample:
+                logs.error(f"You told me to resume the apriori sampler - it has already completed (with {self.n} samples), so sampling will end.")
+                logs.error("Increase the 'nsample' parameter to keep going.")
+            else:
+                logs.overview(f"Continuing apriori sampling - have {self.n} samples already")
 
 
     def execute(self):
-        n = 0
+        n = self.n
         nparam = len(self.pipeline.varied_params)
 
         if self.pool:
             chunk_size = self.pool.size
 
         def sample_from_prior():
             x = np.random.uniform(0.0,1.0,size=nparam)
```

### Comparing `cosmosis-3.0.3/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.1/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.1/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.1/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.1/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.1/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.1/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/hints.py` & `cosmosis-3.1/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.1/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.1/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.1/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.1/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.1/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.1/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-3.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.1/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.1/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.1/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.1/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.1/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.1/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.1/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.1/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.1/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.1/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/sampler.py` & `cosmosis-3.1/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/snake/snake.py` & `cosmosis-3.1/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.1/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.1/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.1/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.1/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/example_module2.py` & `cosmosis-3.1/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/Makefile` & `cosmosis-3.1/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.1/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.1/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.1/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.1/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.1/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.1/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.1/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.1/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_block.py` & `cosmosis-3.1/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_campaign.py` & `cosmosis-3.1/cosmosis/test/test_campaign.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_chaining.py` & `cosmosis-3.1/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_gaussian.py` & `cosmosis-3.1/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_lib.py` & `cosmosis-3.1/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_modules.py` & `cosmosis-3.1/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_parameters.py` & `cosmosis-3.1/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_pipeline.py` & `cosmosis-3.1/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_polychord.py` & `cosmosis-3.1/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_samplers.py` & `cosmosis-3.1/cosmosis/test/test_samplers.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_text_output.py` & `cosmosis-3.1/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/test/test_utils.py` & `cosmosis-3.1/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis/utils.py` & `cosmosis-3.1/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.1/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.0.3/setup.py` & `cosmosis-3.1/setup.py`

 * *Files identical despite different names*

