# Comparing `tmp/stellarphot-1.3.9.tar.gz` & `tmp/stellarphot-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellarphot-1.3.9.tar", last modified: Fri Jun 16 20:07:47 2023, max compression
+gzip compressed data, was "stellarphot-1.4.0.tar", last modified: Thu Aug  3 17:25:04 2023, max compression
```

## Comparing `stellarphot-1.3.9.tar` & `stellarphot-1.4.0.tar`

### file list

```diff
@@ -1,134 +1,150 @@
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.813825 stellarphot-1.3.9/
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.731347 stellarphot-1.3.9/.github/
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.745295 stellarphot-1.3.9/.github/workflows/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1229 2022-06-01 15:38:08.000000 stellarphot-1.3.9/.github/workflows/build.yml
--rw-r--r--   0 jv8699qa (145084326) 2132868096      753 2023-06-15 18:08:41.000000 stellarphot-1.3.9/.gitignore
--rw-r--r--   0 jv8699qa (145084326) 2132868096      633 2023-06-16 19:54:25.000000 stellarphot-1.3.9/.readthedocs.yml
--rw-r--r--   0 jv8699qa (145084326) 2132868096      241 2023-06-16 19:54:18.000000 stellarphot-1.3.9/.rtd-environment.yml
--rw-r--r--   0 jv8699qa (145084326) 2132868096     2283 2023-06-16 20:06:42.000000 stellarphot-1.3.9/CHANGES.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096      347 2022-10-18 13:26:31.000000 stellarphot-1.3.9/MANIFEST.in
--rw-r--r--   0 jv8699qa (145084326) 2132868096      439 2023-06-16 20:07:47.813998 stellarphot-1.3.9/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1930 2023-06-15 17:41:12.000000 stellarphot-1.3.9/README.md
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.748079 stellarphot-1.3.9/docs/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4581 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/Makefile
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.731856 stellarphot-1.3.9/docs/_templates/
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.750235 stellarphot-1.3.9/docs/_templates/autosummary/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      250 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/base.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096      251 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/class.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096      252 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/_templates/autosummary/module.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7316 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/conf.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096      482 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/index.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4549 2020-02-18 16:06:39.000000 stellarphot-1.3.9/docs/make.bat
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.750917 stellarphot-1.3.9/docs/stellarphot/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1127 2023-06-15 18:08:41.000000 stellarphot-1.3.9/docs/stellarphot/index.rst
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.753086 stellarphot-1.3.9/licenses/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1482 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/LICENSE.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096      372 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/README.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1659 2020-02-18 16:06:39.000000 stellarphot-1.3.9/licenses/TEMPLATE_LICENCE.rst
--rw-r--r--   0 jv8699qa (145084326) 2132868096      132 2020-02-18 16:06:39.000000 stellarphot-1.3.9/pyproject.toml
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1920 2023-06-16 20:07:47.814967 stellarphot-1.3.9/setup.cfg
--rwxr-xr-x   0 jv8699qa (145084326) 2132868096     1039 2020-02-18 16:06:39.000000 stellarphot-1.3.9/setup.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.756219 stellarphot-1.3.9/stellarphot/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1052 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1476 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/_astropy_init.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.760215 stellarphot-1.3.9/stellarphot/analysis/
--rw-r--r--   0 jv8699qa (145084326) 2132868096       53 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/analysis/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.762503 stellarphot-1.3.9/stellarphot/analysis/data/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1829 2022-03-28 19:21:43.000000 stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-candidate.json
--rw-r--r--   0 jv8699qa (145084326) 2132868096      574 2022-03-28 19:21:43.000000 stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-known.json
--rw-r--r--   0 jv8699qa (145084326) 2132868096     5106 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-candidate.json
--rw-r--r--   0 jv8699qa (145084326) 2132868096     3852 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-known.json
--rw-r--r--   0 jv8699qa (145084326) 2132868096    15542 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/analysis/exotic.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.764019 stellarphot-1.3.9/stellarphot/analysis/tests/
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/analysis/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096      249 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/analysis/tests/test_exotic.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    10169 2021-11-05 21:05:08.000000 stellarphot-1.3.9/stellarphot/analysis/tests/test_transit_fitting.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    20530 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/analysis/transit_fitting.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1166 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/conftest.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     2142 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/core.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.764705 stellarphot-1.3.9/stellarphot/data/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      246 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/data/README.rst
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.766761 stellarphot-1.3.9/stellarphot/differential_photometry/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      120 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/differential_photometry/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7076 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/aij_rel_fluxes.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     9557 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/catalog_search.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    23388 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/differential_photometry/magnitude_transforms.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.769409 stellarphot-1.3.9/stellarphot/differential_photometry/tests/
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.784519 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/
--rw-r--r--   0 jv8699qa (145084326) 2132868096   832320 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    11520 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/comp_stars.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    28800 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096      251 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/mag_transform.csv
--rw-r--r--   0 jv8699qa (145084326) 2132868096     5760 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    23040 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096    25920 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/variables.fits
--rw-r--r--   0 jv8699qa (145084326) 2132868096     5272 2021-11-18 18:30:03.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7885 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_catalog_search.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    12412 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_magnitude_transforms.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1888 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_vsx_mags.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     3858 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/differential_photometry/vsx_mags.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.787327 stellarphot-1.3.9/stellarphot/io/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      104 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     9693 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/aavso_submission_schema.yml
--rw-r--r--   0 jv8699qa (145084326) 2132868096    18826 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/io/aij.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    11551 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/io/tess.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.788735 stellarphot-1.3.9/stellarphot/io/tests/
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/io/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.790125 stellarphot-1.3.9/stellarphot/io/tests/data/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      909 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/io/tests/data/aij-sample-apertures.aperture
--rw-r--r--   0 jv8699qa (145084326) 2132868096      529 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/io/tests/data/apertures_as_table.csv
--rw-r--r--   0 jv8699qa (145084326) 2132868096     2906 2023-06-15 17:36:47.000000 stellarphot-1.3.9/stellarphot/io/tests/test_aij_io.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1904 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/io/tests/test_tess_submission.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.792566 stellarphot-1.3.9/stellarphot/notebooks/
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     5801 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/comp-star-plots.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     9803 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/comp-stars-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096    27859 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/notebooks/image-viewer-working-copy.ipynb
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.804339 stellarphot-1.3.9/stellarphot/notebooks/photometry/
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1869 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096    10203 2022-11-17 19:42:08.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     2501 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
--rwxr-xr-x   0 jv8699qa (145084326) 2132868096     4631 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/03-photometry-template.ipynb
--rwxr-xr-x   0 jv8699qa (145084326) 2132868096     4078 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096    19546 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4377 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7063 2023-06-16 19:34:31.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/0X-comps-star-plot (1).ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     6486 2022-10-20 16:49:16.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/Untitled.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     9511 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096   144711 2023-06-15 17:41:12.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096     5602 2023-06-16 20:04:46.000000 stellarphot-1.3.9/stellarphot/notebooks/photometry/transform-pared-back.ipynb
--rw-r--r--   0 jv8699qa (145084326) 2132868096    25806 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/photometry.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     6216 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/source_detection.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.807479 stellarphot-1.3.9/stellarphot/tests/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      108 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/__init__.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.808226 stellarphot-1.3.9/stellarphot/tests/data/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      160 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/data/test_sources.csv
--rw-r--r--   0 jv8699qa (145084326) 2132868096      265 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/make_wcs.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096      299 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/tests/test_core.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7584 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/tests/test_detection.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4156 2021-05-23 20:38:12.000000 stellarphot-1.3.9/stellarphot/tests/test_photometry.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096      382 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/version.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.812136 stellarphot-1.3.9/stellarphot/visualization/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      298 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/visualization/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4821 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/aij_plots.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    30006 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/comparison_functions.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4294 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/fits_opener.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     7254 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/multi_night_plots.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     2537 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/photometry_widget_functions.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096    22372 2023-06-16 20:04:48.000000 stellarphot-1.3.9/stellarphot/visualization/seeing_profile_functions.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.813183 stellarphot-1.3.9/stellarphot/visualization/tests/
--rw-r--r--   0 jv8699qa (145084326) 2132868096        0 2020-06-25 02:34:16.000000 stellarphot-1.3.9/stellarphot/visualization/tests/__init__.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4237 2023-06-15 18:08:31.000000 stellarphot-1.3.9/stellarphot/visualization/tests/test_seeing_profile.py
--rw-r--r--   0 jv8699qa (145084326) 2132868096     3135 2023-06-15 18:08:41.000000 stellarphot-1.3.9/stellarphot/visualization/transit_plots.py
-drwxr-xr-x   0 jv8699qa (145084326) 2132868096        0 2023-06-16 20:07:47.758942 stellarphot-1.3.9/stellarphot.egg-info/
--rw-r--r--   0 jv8699qa (145084326) 2132868096      439 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/PKG-INFO
--rw-r--r--   0 jv8699qa (145084326) 2132868096     4538 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/SOURCES.txt
--rw-r--r--   0 jv8699qa (145084326) 2132868096        1 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/dependency_links.txt
--rw-r--r--   0 jv8699qa (145084326) 2132868096        1 2022-06-01 15:46:16.000000 stellarphot-1.3.9/stellarphot.egg-info/not-zip-safe
--rw-r--r--   0 jv8699qa (145084326) 2132868096      221 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/requires.txt
--rw-r--r--   0 jv8699qa (145084326) 2132868096       12 2023-06-16 20:07:47.000000 stellarphot-1.3.9/stellarphot.egg-info/top_level.txt
--rw-r--r--   0 jv8699qa (145084326) 2132868096     1238 2021-11-05 21:05:08.000000 stellarphot-1.3.9/tox.ini
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.404397 stellarphot-1.4.0/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.350125 stellarphot-1.4.0/.github/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.353762 stellarphot-1.4.0/.github/workflows/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1229 2023-07-27 17:59:45.000000 stellarphot-1.4.0/.github/workflows/build.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)      753 2023-07-27 17:59:34.000000 stellarphot-1.4.0/.gitignore
+-rw-r--r--   0 mattcraig   (501) staff       (20)      633 2023-07-27 17:59:45.000000 stellarphot-1.4.0/.readthedocs.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)      241 2023-07-27 17:59:45.000000 stellarphot-1.4.0/.rtd-environment.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2394 2023-08-03 17:23:27.000000 stellarphot-1.4.0/CHANGES.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      347 2020-05-29 17:45:42.000000 stellarphot-1.4.0/MANIFEST.in
+-rw-r--r--   0 mattcraig   (501) staff       (20)      439 2023-08-03 17:25:04.404493 stellarphot-1.4.0/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1930 2022-12-11 22:52:57.000000 stellarphot-1.4.0/README.md
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.354410 stellarphot-1.4.0/docs/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4581 2020-05-25 15:45:57.000000 stellarphot-1.4.0/docs/Makefile
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.350376 stellarphot-1.4.0/docs/_templates/
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.355266 stellarphot-1.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      250 2020-05-25 15:45:57.000000 stellarphot-1.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2020-05-25 15:45:57.000000 stellarphot-1.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      252 2020-05-25 15:45:57.000000 stellarphot-1.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7316 2023-07-27 17:59:34.000000 stellarphot-1.4.0/docs/conf.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      482 2023-07-27 17:59:45.000000 stellarphot-1.4.0/docs/index.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4549 2020-05-25 15:45:57.000000 stellarphot-1.4.0/docs/make.bat
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.355516 stellarphot-1.4.0/docs/stellarphot/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1127 2023-07-27 17:59:45.000000 stellarphot-1.4.0/docs/stellarphot/index.rst
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.356030 stellarphot-1.4.0/licenses/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1482 2020-05-25 15:45:57.000000 stellarphot-1.4.0/licenses/LICENSE.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      372 2020-05-25 15:45:57.000000 stellarphot-1.4.0/licenses/README.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1659 2020-05-25 15:45:57.000000 stellarphot-1.4.0/licenses/TEMPLATE_LICENCE.rst
+-rw-r--r--   0 mattcraig   (501) staff       (20)      132 2020-05-25 15:45:57.000000 stellarphot-1.4.0/pyproject.toml
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1920 2023-08-03 17:25:04.404974 stellarphot-1.4.0/setup.cfg
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     1039 2020-05-25 15:45:57.000000 stellarphot-1.4.0/setup.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.357120 stellarphot-1.4.0/stellarphot/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1052 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1476 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/_astropy_init.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.358642 stellarphot-1.4.0/stellarphot/analysis/
+-rw-r--r--   0 mattcraig   (501) staff       (20)       53 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.359509 stellarphot-1.4.0/stellarphot/analysis/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1829 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/data/exotic-to-mod-candidate.json
+-rw-r--r--   0 mattcraig   (501) staff       (20)      574 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/data/exotic-to-mod-known.json
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5106 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/data/tic-template-for-exotic-candidate.json
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3852 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/data/tic-template-for-exotic-known.json
+-rw-r--r--   0 mattcraig   (501) staff       (20)    15542 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/exotic.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.359934 stellarphot-1.4.0/stellarphot/analysis/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/tests/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      249 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/tests/test_exotic.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    10169 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/tests/test_transit_fitting.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    20530 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/analysis/transit_fitting.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1166 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/conftest.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2142 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/core.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.360115 stellarphot-1.4.0/stellarphot/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      246 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/data/README.rst
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.361169 stellarphot-1.4.0/stellarphot/differential_photometry/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      120 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7076 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/aij_rel_fluxes.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9557 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/catalog_search.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    23388 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/magnitude_transforms.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.361895 stellarphot-1.4.0/stellarphot/differential_photometry/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.370020 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)  1299163 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)   832320 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2792 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    28800 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      188 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    23040 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4799 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/comp_stars.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    11520 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/comp_stars.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2782 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    28800 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      251 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/mag_transform.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      393 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    23040 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)      215 2022-07-04 15:45:06.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/variables.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    25920 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/variables.fits
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5272 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7885 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_catalog_search.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    12412 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_magnitude_transforms.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1888 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_vsx_mags.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3858 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/differential_photometry/vsx_mags.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.371071 stellarphot-1.4.0/stellarphot/io/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      125 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/io/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     8103 2023-08-03 13:55:37.000000 stellarphot-1.4.0/stellarphot/io/aavso.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9793 2023-08-01 21:31:45.000000 stellarphot-1.4.0/stellarphot/io/aavso_submission_schema.yml
+-rw-r--r--   0 mattcraig   (501) staff       (20)    18826 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/io/aij.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    11551 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/io/tess.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.371637 stellarphot-1.4.0/stellarphot/io/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/io/tests/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.394698 stellarphot-1.4.0/stellarphot/io/tests/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20) 18499443 2023-07-27 15:13:54.000000 stellarphot-1.4.0/stellarphot/io/tests/data/_her-2023-06-10.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)      909 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/io/tests/data/aij-sample-apertures.aperture
+-rw-r--r--   0 mattcraig   (501) staff       (20)      529 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/io/tests/data/apertures_as_table.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)    12805 2023-08-01 21:54:37.000000 stellarphot-1.4.0/stellarphot/io/tests/data/dy-her-aavso-test-data.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5784 2023-07-27 17:57:35.000000 stellarphot-1.4.0/stellarphot/io/tests/data/wowy.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2904 2023-08-01 23:06:41.000000 stellarphot-1.4.0/stellarphot/io/tests/test_aavso.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2906 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/io/tests/test_aij_io.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1904 2022-12-11 22:52:57.000000 stellarphot-1.4.0/stellarphot/io/tests/test_tess_submission.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.395715 stellarphot-1.4.0/stellarphot/notebooks/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/notebooks/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5801 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/comp-star-plots.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9803 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/comp-stars-template.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    27859 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/image-viewer-working-copy.ipynb
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.402066 stellarphot-1.4.0/stellarphot/notebooks/photometry/
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1869 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    10203 2022-11-17 19:42:08.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2501 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     4631 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/03-photometry-template.ipynb
+-rwxr-xr-x   0 mattcraig   (501) staff       (20)     4078 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4933 2022-12-01 14:10:54.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/06-target-flux-plot-template.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    19546 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4377 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    89292 2022-11-14 01:23:27.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/Untitled.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     9289 2022-11-18 16:16:24.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/Untitled1.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    13810 2022-11-28 17:20:56.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/Untitled2.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2022-12-03 19:59:08.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     8235 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)   144711 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    72371 2022-11-08 14:06:28.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/magnitude-plots.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5549 2022-11-08 14:20:11.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/transform-pared-back-Copy1.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5602 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/notebooks/photometry/transform-pared-back.ipynb
+-rw-r--r--   0 mattcraig   (501) staff       (20)    25806 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/photometry.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     6216 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/source_detection.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.402803 stellarphot-1.4.0/stellarphot/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      108 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/tests/__init__.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.402918 stellarphot-1.4.0/stellarphot/tests/data/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      160 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/tests/data/test_sources.csv
+-rw-r--r--   0 mattcraig   (501) staff       (20)      265 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/tests/make_wcs.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      299 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/tests/test_core.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7584 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/tests/test_detection.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4156 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/tests/test_photometry.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)      382 2020-05-29 17:45:42.000000 stellarphot-1.4.0/stellarphot/version.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.404066 stellarphot-1.4.0/stellarphot/visualization/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      298 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4821 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/aij_plots.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    30006 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/comparison_functions.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4294 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/fits_opener.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     7254 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/multi_night_plots.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     2537 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/photometry_widget_functions.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)    22372 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/seeing_profile_functions.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.404279 stellarphot-1.4.0/stellarphot/visualization/tests/
+-rw-r--r--   0 mattcraig   (501) staff       (20)        0 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/tests/__init__.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     4237 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/tests/test_seeing_profile.py
+-rw-r--r--   0 mattcraig   (501) staff       (20)     3135 2023-07-27 17:59:45.000000 stellarphot-1.4.0/stellarphot/visualization/transit_plots.py
+drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2023-08-03 17:25:04.358156 stellarphot-1.4.0/stellarphot.egg-info/
+-rw-r--r--   0 mattcraig   (501) staff       (20)      439 2023-08-03 17:25:04.000000 stellarphot-1.4.0/stellarphot.egg-info/PKG-INFO
+-rw-r--r--   0 mattcraig   (501) staff       (20)     5472 2023-08-03 17:25:04.000000 stellarphot-1.4.0/stellarphot.egg-info/SOURCES.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2023-08-03 17:25:04.000000 stellarphot-1.4.0/stellarphot.egg-info/dependency_links.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)        1 2022-10-08 21:30:55.000000 stellarphot-1.4.0/stellarphot.egg-info/not-zip-safe
+-rw-r--r--   0 mattcraig   (501) staff       (20)      221 2023-08-03 17:25:04.000000 stellarphot-1.4.0/stellarphot.egg-info/requires.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)       12 2023-08-03 17:25:04.000000 stellarphot-1.4.0/stellarphot.egg-info/top_level.txt
+-rw-r--r--   0 mattcraig   (501) staff       (20)     1238 2023-07-27 17:59:45.000000 stellarphot-1.4.0/tox.ini
```

### Comparing `stellarphot-1.3.9/.github/workflows/build.yml` & `stellarphot-1.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/.gitignore` & `stellarphot-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/.readthedocs.yml` & `stellarphot-1.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/CHANGES.rst` & `stellarphot-1.4.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.4.0 (2023-08-03)
+------------------
+
+New Features
+^^^^^^^^^^^^
+
++ Add class for writing AAVSO files. [#146]
+
 1.3.9 (2023-06-16)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
 
 Other Changes and Additions
```

### Comparing `stellarphot-1.3.9/README.md` & `stellarphot-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/docs/Makefile` & `stellarphot-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/docs/conf.py` & `stellarphot-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/docs/make.bat` & `stellarphot-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/docs/stellarphot/index.rst` & `stellarphot-1.4.0/docs/stellarphot/index.rst`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/licenses/LICENSE.rst` & `stellarphot-1.4.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/licenses/TEMPLATE_LICENCE.rst` & `stellarphot-1.4.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/setup.cfg` & `stellarphot-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/setup.py` & `stellarphot-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/__init__.py` & `stellarphot-1.4.0/stellarphot/__init__.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/_astropy_init.py` & `stellarphot-1.4.0/stellarphot/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-candidate.json` & `stellarphot-1.4.0/stellarphot/analysis/data/exotic-to-mod-candidate.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/data/exotic-to-mod-known.json` & `stellarphot-1.4.0/stellarphot/analysis/data/exotic-to-mod-known.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-candidate.json` & `stellarphot-1.4.0/stellarphot/analysis/data/tic-template-for-exotic-candidate.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/data/tic-template-for-exotic-known.json` & `stellarphot-1.4.0/stellarphot/analysis/data/tic-template-for-exotic-known.json`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/exotic.py` & `stellarphot-1.4.0/stellarphot/analysis/exotic.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/tests/test_transit_fitting.py` & `stellarphot-1.4.0/stellarphot/analysis/tests/test_transit_fitting.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/analysis/transit_fitting.py` & `stellarphot-1.4.0/stellarphot/analysis/transit_fitting.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/conftest.py` & `stellarphot-1.4.0/stellarphot/conftest.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/core.py` & `stellarphot-1.4.0/stellarphot/core.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/aij_rel_fluxes.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/aij_rel_fluxes.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/catalog_search.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/catalog_search.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/magnitude_transforms.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/magnitude_transforms.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/comp_stars.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/comp_stars.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/data/variables.fits` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/data/variables.fits`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_catalog_search.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_catalog_search.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_magnitude_transforms.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_magnitude_transforms.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/tests/test_vsx_mags.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/tests/test_vsx_mags.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/differential_photometry/vsx_mags.py` & `stellarphot-1.4.0/stellarphot/differential_photometry/vsx_mags.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/aavso_submission_schema.yml` & `stellarphot-1.4.0/stellarphot/io/aavso_submission_schema.yml`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,16 @@
     summary: |
       Check star name or label such as the AUID (much preferred)
       or the chart label for the check star. If not present,
       use "na".
       Limit: 20 characters.
   KMAG:
     summary: |
-      Instrumental magnitude of the check star.
+      Instrumental magnitude of the check star, unless doing "ensemble" photometry
+      in which case the calibrated magnitude should be reported.
       If "ensemble" see example below. If not present, use "na".
       Limit: 8 characters.
   AIRMASS:
     summary: |
       Airmass of observation Limit 7 characters - entry will be truncated
       if longer than that. If not present, use "na".
   GROUP:
```

### Comparing `stellarphot-1.3.9/stellarphot/io/aij.py` & `stellarphot-1.4.0/stellarphot/io/aij.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/tess.py` & `stellarphot-1.4.0/stellarphot/io/tess.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/tests/data/aij-sample-apertures.aperture` & `stellarphot-1.4.0/stellarphot/io/tests/data/aij-sample-apertures.aperture`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/tests/data/apertures_as_table.csv` & `stellarphot-1.4.0/stellarphot/io/tests/data/apertures_as_table.csv`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/tests/test_aij_io.py` & `stellarphot-1.4.0/stellarphot/io/tests/test_aij_io.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/io/tests/test_tess_submission.py` & `stellarphot-1.4.0/stellarphot/io/tests/test_tess_submission.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/comp-star-plots.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/comp-star-plots.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/comp-stars-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/comp-stars-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/image-viewer-working-copy.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/image-viewer-working-copy.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/03-photometry-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/03-photometry-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/06-transit-fit-template.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/0X-comps-star-plot (1).ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/transform-pared-back.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8211123537410302%*

 * *Differences: {"'cells'": "{0: {'execution_count': None, 'source': {insert: [(0, 'from pathlib import Path\\n'), "*

 * *            "(2, 'from scipy.optimize import curve_fit\\n'), (3, '\\n'), (4, 'from astropy.table "*

 * *            "import Table, vstack\\n'), (5, 'from astropy.coordinates import SkyCoord\\n'), (6, "*

 * *            "'\\n'), (7, '%matplotlib inline\\n'), (8, 'import matplotlib.pyplot as plt\\n'), (9, "*

 * *            "'\\n'), (10, 'from fit_functions import get_cat, f, opts_to_str, calc_residual\\n'), "*

 * *            "( […]*

```diff
@@ -1,228 +1,202 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "id": "e5ef9308-7aa7-44b4-9510-4aa4f08a388b",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import ipywidgets as ipw\n",
-                "from astropy.table import Table\n",
-                "%matplotlib widget\n",
-                "from matplotlib import pyplot as plt\n",
+                "from pathlib import Path\n",
                 "import numpy as np\n",
-                "from scipy.optimize import curve_fit"
+                "from scipy.optimize import curve_fit\n",
+                "\n",
+                "from astropy.table import Table, vstack\n",
+                "from astropy.coordinates import SkyCoord\n",
+                "\n",
+                "%matplotlib inline\n",
+                "import matplotlib.pyplot as plt\n",
+                "\n",
+                "from fit_functions import get_cat, f, opts_to_str, calc_residual\n",
+                "from calib_function import transform_to_catalog"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1c48ee26-1df1-455b-a12f-6387ffaf4f2f",
             "metadata": {},
             "source": [
-                "#  You will need to change some values in the cell below "
+                "# Parameters\n",
+                "\n",
+                "The magnitudes in each image are fit using this model:\n",
+                "\n",
+                "$$\n",
+                "r_{p, c} = a r_{p, inst} + b r_{p, inst}^2 + c (B_c - V_c) + d (B_c - V_c)^2 + z\n",
+                "$$\n",
+                "\n",
+                "The parameters in the cell below set the range of values the fit is constrained to. The way to fix a parameter is to give it a very, very small range for the constraint.\n",
+                "\n",
+                "More specifically, each of the fit values is subject to these constraints:\n",
+                "\n",
+                "+ $1 - a_{delta} < a < 1 + a_{delta}$\n",
+                "+ $b_{min} < b < -b_{min}$\n",
+                "+ $c_{min} < c < -c_{min}$\n",
+                "+ $d_{min} < d < -d_{min}$\n",
+                "+ The range for the zero point is $18 < z < 22$.\n",
+                "\n",
+                "\n",
+                "`output_dir` is where the PNG and FITS files generated by this notebook are stored. `run_name` is a descriptive name for the settings you have chosen that gets included in the output file names.\n",
+                "\n",
+                "### *Recommendation:*\n",
+                "\n",
+                "+ Keep $b$ essentially fixed. \n",
+                "+ Fixing $d$ is ok for now too, I think.\n",
+                "\n",
+                "In both cases, setting a min of `1e-6` or something should do the trick.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "380930ba-c708-4202-b0a6-32f70a24c677",
-            "metadata": {},
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "parameters"
+                ]
+            },
             "outputs": [],
             "source": [
-                "comp_locations = Table.read('aperture_locations.csv')\n",
-                "flux_table = Table.read('some_name.csv')"
+                "a_delta = 0.5\n",
+                "b_min = -0.1\n",
+                "c_min = -0.5\n",
+                "d_min = -1e-6\n",
+                "\n",
+                "our_filters = ['B', 'V', 'rp']\n",
+                "\n",
+                "aavso_band_names = dict(\n",
+                "    B='B', \n",
+                "    V='V',\n",
+                "    gp='SG',\n",
+                "    rp='SR',\n",
+                "    ip='SI'\n",
+                ")\n",
+                "\n",
+                "cat_color_colums = dict(\n",
+                "    B=('Bmag', 'Vmag'),\n",
+                "    V=('Bmag', 'Vmag'),\n",
+                "    gp=('g_mag', 'r_mag'),\n",
+                "    rp=('r_mag', 'i_mag'),\n",
+                "    ip=('r_mag', 'i_mag'),\n",
+                "    \n",
+                ")\n",
+                "\n",
+                "cat_filter = dict(\n",
+                "    B='Bmag', \n",
+                "    V='Vmag',\n",
+                "    gp='g_mag',\n",
+                "    rp='r_mag',\n",
+                "    ip='i_mag')\n",
+                "\n",
+                "input_photometry_file = 'm13-2021-09-28.csv'\n",
+                "output_photometry_file = 'some_name.csv'"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "id": "7c7503b6-49a2-4585-90b2-c36039a50298",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "flux_table = flux_table[flux_table['filter']=='rp']"
+                "all_mags = Table.read(input_photometry_file)\n",
+                "\n",
+                "# Ensure we have the right table ordering later\n",
+                "all_mags.sort(['filter', 'BJD'])"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 8,
-            "id": "0a32157b-764b-4cc1-8f17-09383762f0ef",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "present_ids = sorted(set(flux_table['star_id']))\n",
-                "\n",
-                "star_type = {sid: desc for sid, desc in comp_locations['star_id', 'marker name']}\n",
-                "    \n",
-                "select_multi = ipw.SelectMultiple(options=[(f'{sid:3d} {star_type[sid]}', sid) for sid in present_ids],\n",
-                "                                  description='For these objects')\n",
-                "select_multi.rows = 10\n",
-                "\n",
-                "columns = sorted(flux_table.colnames)\n",
-                "\n",
-                "y_axis = ipw.Dropdown(options=columns, description=\"Graph this\")\n",
-                "y_axis.value = 'mag_inst'\n",
-                "\n",
-                "y_offset = ipw.FloatSlider(min=0, max=1, value=0, step=0.01, description='Offset by')\n",
-                "\n",
-                "detrend_by = ipw.Dropdown(options=columns, description='Detrend by', value=None)\n",
-                "\n",
-                "title = ipw.Text(description='Title')"
+                "## Get ready for the transform"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "id": "97ecc2a2-8625-415c-a06b-29c71abb151c",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.ioff()\n",
+                "filter_groups = all_mags.group_by('filter')\n",
                 "\n",
-                "fig, ax = plt.subplots()\n",
-                "fig.canvas.header_visible = False\n",
-                "ax.grid()\n",
                 "\n",
-                "ax.set_xlabel('BJD')\n",
-                "ax.set_ylabel('Flux');"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 10,
-            "id": "9acfca14-6e29-43f6-a844-656baab07e14",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "def linear_detrend(data, parameter):\n",
-                "    def f(x, slope, intercept):\n",
-                "        return slope * x + intercept\n",
+                "# Check: do we have any unexpected filters?\n",
                 "\n",
-                "    popt, pcov = curve_fit(f, parameter, data)\n",
-                "    \n",
-                "    return data - popt[0] * parameter"
+                "assert all(k[0] in cat_filter.keys() for k in filter_groups.groups.keys)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 11,
-            "id": "4ab6eda3-6f6c-4c7c-912d-1757e7ab731e",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "def update_plot(change):\n",
-                "    ax.lines.clear()\n",
-                "    min = 100\n",
-                "    max = -100\n",
-                "    data_col = y_axis.value\n",
-                "    for idx, star_id in enumerate(select_multi.value):\n",
-                "        data = flux_table[flux_table['star_id'] == star_id]\n",
-                "        \n",
-                "        norm_flux = data[data_col] / data[data_col].mean()\n",
-                "        if detrend_by.value:\n",
-                "            print(detrend_by.value)\n",
-                "            norm_flux = linear_detrend(norm_flux, data[detrend_by.value])\n",
-                "            norm_flux = norm_flux / norm_flux.mean()\n",
-                "            \n",
-                "        norm_flux += y_offset.value * idx\n",
-                "\n",
-                "        ax.plot(data['BJD'], norm_flux, label=f'{star_id}')\n",
-                "        #lines[0].set_data(data['BJD'], norm_flux)\n",
-                "        ax.set_xlim(data['BJD'].min(), data['BJD'].max())  \n",
-                "        min = norm_flux.min() if norm_flux.min() < min else min\n",
-                "        max = norm_flux.max() if norm_flux.max() > max else max\n",
-                "        \n",
-                "    ax.set_ylim(0.8 * min, 1.1 * max)\n",
-                "    ax.set_xlabel('BJD')\n",
-                "    ax.set_ylabel(data_col)\n",
-                "    if title.value:\n",
-                "        ax.set_title(title.value)\n",
-                "    ax.legend()\n",
-                "    fig.canvas.draw()\n",
-                "    fig.canvas.flush_events()"
+                "## Do the transforms, one filter at a time"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "b15b13f9-b1f4-4f6e-ba29-b621b714dcd7",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "vb = ipw.VBox(children=[y_axis, select_multi, y_offset, detrend_by, title])\n",
+                "output_table = [] \n",
                 "\n",
-                "for wid in vb.children:\n",
-                "    wid.observe(update_plot, names='value')"
+                "for k, group in zip(our_filters, filter_groups.groups):\n",
+                "    print(f'Transforming band {k}')\n",
+                "    by_bjd = group.group_by('BJD')\n",
+                "    \n",
+                "    transform_to_catalog(by_bjd, f'mag_inst', aavso_band_names[k], \n",
+                "                     obs_error_column='mag_error', \n",
+                "                     zero_point_range=[12, 25],\n",
+                "                     c_delta=0.5, # b_delta=0.1, \n",
+                "                     cat_filter=cat_filter[k], cat_color=cat_color_colums[k],\n",
+                "                     in_place=True);\n",
+                "    output_table.append(by_bjd.copy())\n",
+                "\n",
+                "output_table = vstack(output_table, join_type='outer')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "id": "2a1cc161-ea49-4a42-8943-0873b35de425",
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "9bb5c4613a3f480e8de49e13461c70fd",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "AppLayout(children=(VBox(children=(Dropdown(description='Graph this', index=26, options=('BJD', 'Dec', 'RA', '\u2026"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "ipw.AppLayout(\n",
-                "    center=fig.canvas,\n",
-                "    right_sidebar=vb,  # select_multi,\n",
-                "    pane_heights=[0, 6, 1]\n",
-                ")"
+                "plt.plot(by_bjd['mag_inst_cal'], by_bjd['mag_cat'], 'o')\n",
+                "plt.grid()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "id": "25c2c5ba-ff16-4363-8f3d-f10c3bcf2098",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "start = 2459910.8122\n",
-                "end   = 2459910.9032\n",
-                "low = 0.8\n",
-                "high = 2.0\n",
-                "plt.vlines(start, low, high, colors='r', linestyle='--', alpha=0.5)\n",
-                "plt.vlines(end, low, high, colors='r', linestyle='--', alpha=0.5)\n",
-                "plt.text(start, low+0.0005, f'Predicted\\nIngress\\n{start-2400000-int(start - 2400000):.3f}', horizontalalignment='center',c='r')\n",
-                "plt.text(end, low+0.0005, f'Predicted\\nEgress\\n{end-2400000-int(end - 2400000):.3f}', horizontalalignment='center',c='r')\n",
-                "fig.canvas.draw()"
+                "plt.plot(by_bjd['mag_cat'] - by_bjd['mag_inst_cal'], 'o')\n",
+                "plt.grid()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "b7a84ba0-c362-4acd-90b4-3079bdd67a9a",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ax.set_title('TIC 467615239.01 UT2022.11.27\\n Paul P. Feder Observatory 0.4m (ip filter,120 exp,fap 11-21-26)')\n",
-                "       \n",
-                "fig.canvas.draw()"
+                "output_table.write(output_photometry_file)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8f7234c9-2b67-4835-9b9c-1ba075377bd4",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -240,9 +214,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9845783932592176%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, '\\n'), (2, 'import numpy as np\\n'), (3, '\\n')]}}, 5: "*

 * *            '{\'source\': {insert: [(1, "check_star_auid = comp_stars_check_only[\'auid\'][0]")], '*

 * *            'delete: [2, 1]}}, 8: {\'source\': {insert: [(6, \'airmass = []\\n\'), (15, "    '*

 * *            'airmass.append(rows[\'airmass\'][0])\\n")]}}, 9: {\'source\': {insert: [(0, "table = '*

 * *            "Table(data=[times, cal_mag, cal_mag_err, airmass], names=['time', 'mag', 'err', "*

 * *            '\'airmass […]*

```diff
@@ -4,14 +4,17 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "6d973d4c-b1db-4f8b-82a2-e64990c07776",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
+                "\n",
+                "import numpy as np\n",
+                "\n",
                 "from astropy.coordinates import SkyCoord\n",
                 "from astropy.table import Table\n",
                 "from astropy.time import Time\n",
                 "from astropy.timeseries import TimeSeries\n",
                 "\n",
                 "from matplotlib import pyplot as plt\n",
                 "\n",
@@ -88,16 +91,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "cdab5216-9a6a-4db4-8508-f5e0b5dd0ece",
             "metadata": {},
             "outputs": [],
             "source": [
                 "comp_stars_check_only = comp_stars[comp_stars['label'] == int(check_star_label)]\n",
-                "check_star_auid = comp_stars_check_only['auid'][0]\n",
-                "check_star_auid"
+                "check_star_auid = comp_stars_check_only['auid'][0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "aa43ad37-6ef2-4d29-b1cd-2b1652ac8ec9",
             "metadata": {},
@@ -123,53 +125,40 @@
             "source": [
                 "this_filter = 'ip'\n",
                 "\n",
                 "this_phot = your_photometry[your_photometry['band'] == this_filter]\n",
                 "                                                                                                                                                                                                                                                                                                                                                                                              \n",
                 "this_phot_grp = this_phot.group_by('BJD')\n",
                 "\n",
+                "airmass = []\n",
                 "times = []\n",
                 "cal_mag = []\n",
                 "cal_mag_err = []\n",
                 "for time, rows in zip(this_phot_grp.groups.keys, this_phot_grp.groups):\n",
                 "    mag, err = vsx_mags.calc_vmag(vc, rows, comp_stars_no_check, band=filter_mapping[this_filter], star_data_mag_column=f'mag_inst')\n",
                 "    cal_mag.append(mag)\n",
                 "    cal_mag_err.append(err)\n",
                 "    times.append(time[0])\n",
+                "    airmass.append(rows['airmass'][0])\n",
                 "    "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cc814ba5-d71d-46ce-924c-3f0889b27729",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from astropy.timeseries import TimeSeries\n",
-                "from astropy import units as u\n",
-                "from astropy.time import Time\n",
-                "import numpy as np\n",
-                "\n",
-                "good_time = Time(times,scale = 'tdb', format= 'jd')\n",
-                "\n",
-                "series = TimeSeries(time=good_time, data=[cal_mag, cal_mag_err], names=['mag', 'err'])\n",
-                "\n",
-                "day = [np.floor(bjd.value) for bjd in series.time]\n",
-                "series['day'] = day\n",
-                "\n",
-                "#series_grouped = series.group_by('day')\n",
-                "\n",
-                "table = Table(data=[times, cal_mag, cal_mag_err], names=['time', 'mag', 'err'])\n",
-                "table['day']  = day\n",
+                "table = Table(data=[times, cal_mag, cal_mag_err, airmass], names=['time', 'mag', 'err', 'airmass'])\n",
+                "table['day']  = [np.floor(bjd) for bjd in table['time']]\n",
                 "\n",
                 "table = table.group_by('day')\n",
                 "\n",
-                "table_grouped = table\n",
-                "series_folded = series.fold(period=3.5*u.hour, epoch_time ='1963-01-30T00:00:00')\n"
+                "table_grouped = table"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c2564919-46e9-4ce9-b6ec-a4dbf04a1a41",
             "metadata": {},
@@ -206,65 +195,43 @@
             "source": [
                 "your_coords = SkyCoord(ra=your_photometry['RA'], dec=your_photometry['Dec'])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "560ab802-170e-4ed2-9fb2-b7ca970fe6a9",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "check_coord.match_to_catalog_sky(your_coords)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "61f51fb1-14dd-4d77-ae25-e7bf62e591f9",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "your_photometry[28141]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "65d3dab3-c4bd-4206-8773-2dfa274df0be",
             "metadata": {},
             "outputs": [],
             "source": [
                 "kc = dict(coords=check_coord)\n",
-                "this_filter = 'ip'\n",
-                "\n",
-                "this_phot = your_photometry[your_photometry['band'] == this_filter]\n",
-                "                                                                                                                                                                                                                                                                                                                                                                                              \n",
-                "this_phot_grp = this_phot.group_by('BJD')\n",
                 "\n",
-                "times = []\n",
+                "airmass_k = []\n",
+                "times_k = []\n",
                 "cal_mag_k = []\n",
                 "cal_mag_err_k = []\n",
                 "for time, rows in zip(this_phot_grp.groups.keys, this_phot_grp.groups):\n",
                 "    mag, err = vsx_mags.calc_vmag(kc, rows, comp_stars_no_check, band=filter_mapping[this_filter], star_data_mag_column=f'mag_inst')\n",
                 "    cal_mag_k.append(mag)\n",
                 "    cal_mag_err_k.append(err)\n",
-                "    times.append(time[0])\n",
-                "    "
+                "    times_k.append(time[0])\n",
+                "    airmass_k.append(rows['airmass'][0])\n",
+                "    \n",
+                "assert times_k == times"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "811274f8-5138-4d51-9b47-217f7f40b956",
             "metadata": {},
             "outputs": [],
             "source": [
-                "table_k = Table(data=[times, cal_mag_k, cal_mag_err_k], names=['time', 'mag', 'err'])\n",
-                "table_k['day']  = day\n",
+                "table_k = Table(data=[times_k, cal_mag_k, cal_mag_err_k, airmass_k], names=['time', 'mag', 'err', 'airmass'])\n",
+                "table_k['day']  = table['day']\n",
                 "\n",
                 "table_k = table_k.group_by('day')\n",
                 "\n",
                 "table_grouped_k = table_k"
             ]
         },
         {
@@ -285,15 +252,15 @@
                 "plt.legend()\n",
                 "plt.ylim(15.2, 14.7)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8c0be3a2-30c2-47c7-a8a5-d7d9c922e2b7",
+            "id": "9d78f9e7-d00d-4905-b376-d9e7a1dbf56f",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/notebooks/photometry/transform-pared-back.ipynb` & `stellarphot-1.4.0/stellarphot/notebooks/photometry/transform-pared-back-Copy1.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997596153846153%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, 'from stellarphot.differential_photometry import "*

 * *            "transform_to_catalog')], delete: [11, 10]}}}"}*

```diff
@@ -12,16 +12,15 @@
                 "\n",
                 "from astropy.table import Table, vstack\n",
                 "from astropy.coordinates import SkyCoord\n",
                 "\n",
                 "%matplotlib inline\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "from fit_functions import get_cat, f, opts_to_str, calc_residual\n",
-                "from calib_function import transform_to_catalog"
+                "from stellarphot.differential_photometry import transform_to_catalog"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Parameters\n",
```

### Comparing `stellarphot-1.3.9/stellarphot/photometry.py` & `stellarphot-1.4.0/stellarphot/photometry.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/source_detection.py` & `stellarphot-1.4.0/stellarphot/source_detection.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/tests/test_detection.py` & `stellarphot-1.4.0/stellarphot/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/tests/test_photometry.py` & `stellarphot-1.4.0/stellarphot/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/aij_plots.py` & `stellarphot-1.4.0/stellarphot/visualization/aij_plots.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/comparison_functions.py` & `stellarphot-1.4.0/stellarphot/visualization/comparison_functions.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/fits_opener.py` & `stellarphot-1.4.0/stellarphot/visualization/fits_opener.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/multi_night_plots.py` & `stellarphot-1.4.0/stellarphot/visualization/multi_night_plots.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/photometry_widget_functions.py` & `stellarphot-1.4.0/stellarphot/visualization/photometry_widget_functions.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/seeing_profile_functions.py` & `stellarphot-1.4.0/stellarphot/visualization/seeing_profile_functions.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/tests/test_seeing_profile.py` & `stellarphot-1.4.0/stellarphot/visualization/tests/test_seeing_profile.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot/visualization/transit_plots.py` & `stellarphot-1.4.0/stellarphot/visualization/transit_plots.py`

 * *Files identical despite different names*

### Comparing `stellarphot-1.3.9/stellarphot.egg-info/SOURCES.txt` & `stellarphot-1.4.0/stellarphot.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -50,48 +50,64 @@
 stellarphot/differential_photometry/magnitude_transforms.py
 stellarphot/differential_photometry/vsx_mags.py
 stellarphot/differential_photometry/tests/__init__.py
 stellarphot/differential_photometry/tests/test_aij_rel_fluxes.py
 stellarphot/differential_photometry/tests/test_catalog_search.py
 stellarphot/differential_photometry/tests/test_magnitude_transforms.py
 stellarphot/differential_photometry/tests/test_vsx_mags.py
+stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.csv
 stellarphot/differential_photometry/tests/data/2014-12-29-ey-uma-9.fits
+stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.csv
 stellarphot/differential_photometry/tests/data/all_apass_ey_uma_sorted_ra_first_20.fits
+stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.csv
 stellarphot/differential_photometry/tests/data/clipped_ey_uma_vsx.fits
+stellarphot/differential_photometry/tests/data/comp_stars.csv
 stellarphot/differential_photometry/tests/data/comp_stars.fits
+stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.csv
 stellarphot/differential_photometry/tests/data/low_error_apass_ey_uma_sorted_ra_first_20.fits
 stellarphot/differential_photometry/tests/data/mag_transform.csv
 stellarphot/differential_photometry/tests/data/sample_wcs_ey_uma.fits
+stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.csv
 stellarphot/differential_photometry/tests/data/unclipped_ey_uma_vsx.fits
+stellarphot/differential_photometry/tests/data/variables.csv
 stellarphot/differential_photometry/tests/data/variables.fits
 stellarphot/io/__init__.py
+stellarphot/io/aavso.py
 stellarphot/io/aavso_submission_schema.yml
 stellarphot/io/aij.py
 stellarphot/io/tess.py
 stellarphot/io/tests/__init__.py
+stellarphot/io/tests/test_aavso.py
 stellarphot/io/tests/test_aij_io.py
 stellarphot/io/tests/test_tess_submission.py
+stellarphot/io/tests/data/_her-2023-06-10.csv
 stellarphot/io/tests/data/aij-sample-apertures.aperture
 stellarphot/io/tests/data/apertures_as_table.csv
+stellarphot/io/tests/data/dy-her-aavso-test-data.csv
+stellarphot/io/tests/data/wowy.csv
 stellarphot/notebooks/__init__.py
 stellarphot/notebooks/comp-star-plots.ipynb
 stellarphot/notebooks/comp-stars-template.ipynb
 stellarphot/notebooks/image-viewer-working-copy.ipynb
 stellarphot/notebooks/photometry/01-viewer-seeing-template.ipynb
 stellarphot/notebooks/photometry/02-comp-star-plotter-template-OG.ipynb
 stellarphot/notebooks/photometry/02-comp-star-plotter-template.ipynb
 stellarphot/notebooks/photometry/03-photometry-template.ipynb
 stellarphot/notebooks/photometry/05-relative-flux-calculation-template.ipynb
+stellarphot/notebooks/photometry/06-target-flux-plot-template.ipynb
 stellarphot/notebooks/photometry/06-transit-fit-template.ipynb
 stellarphot/notebooks/photometry/07-transit-fit-with-exotic.ipynb
-stellarphot/notebooks/photometry/0X-comps-star-plot (1).ipynb
 stellarphot/notebooks/photometry/Untitled.ipynb
+stellarphot/notebooks/photometry/Untitled1.ipynb
+stellarphot/notebooks/photometry/Untitled2.ipynb
 stellarphot/notebooks/photometry/__init__.py
 stellarphot/notebooks/photometry/calculate_aavso_mags_draft.ipynb
 stellarphot/notebooks/photometry/get_apass_comp_mags.ipynb
+stellarphot/notebooks/photometry/magnitude-plots.ipynb
+stellarphot/notebooks/photometry/transform-pared-back-Copy1.ipynb
 stellarphot/notebooks/photometry/transform-pared-back.ipynb
 stellarphot/tests/__init__.py
 stellarphot/tests/make_wcs.py
 stellarphot/tests/test_core.py
 stellarphot/tests/test_detection.py
 stellarphot/tests/test_photometry.py
 stellarphot/tests/data/test_sources.csv
```

### Comparing `stellarphot-1.3.9/tox.ini` & `stellarphot-1.4.0/tox.ini`

 * *Files identical despite different names*

