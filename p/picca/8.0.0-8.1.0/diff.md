# Comparing `tmp/picca-8.0.0.tar.gz` & `tmp/picca-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picca-8.0.0.tar", last modified: Wed Aug  2 08:40:33 2023, max compression
+gzip compressed data, was "picca-8.1.0.tar", last modified: Thu Aug  3 14:30:20 2023, max compression
```

## Comparing `picca-8.0.0.tar` & `picca-8.1.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.976513 picca-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-02 08:40:18.000000 picca-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-02 08:40:33.972512 picca-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-08-02 08:40:18.000000 picca-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.944512 picca-8.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xwick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.936512 picca-8.0.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.948512 picca-8.0.0/py/picca/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.956512 picca-8.0.0/py/picca/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xwick.py
--rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/co.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/calibration_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/dust_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/ivar_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.964512 picca-8.0.0/py/picca/delta_extraction/data_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.964512 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29855 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
--rw-r--r--   0 runner    (1001) docker     (123)    98923 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/least_squares/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/masks/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/absorber_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/bal_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/dla_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/lines_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/rejection_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/utils_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/pk1d/
--rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/compute_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/postproc_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/prep_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/prep_del.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/raw_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/tests/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/correction_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/mask_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/scripts_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_2_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_3_cor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/wedgize.py
--rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/xcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.948512 picca-8.0.0/py/picca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 08:40:20.000000 picca-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:40:33.976513 picca-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 08:40:20.000000 picca-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.822627 picca-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-03 14:30:09.000000 picca-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-03 14:30:20.822627 picca-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-08-03 14:30:09.000000 picca-8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.810627 picca-8.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-03 14:30:09.000000 picca-8.1.0/bin/picca_xwick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.802627 picca-8.1.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.810627 picca-8.1.0/py/picca/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.814627 picca-8.1.0/py/picca/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/bin/picca_xwick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.814627 picca-8.1.0/py/picca/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.814627 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27150 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/corrections/calibration_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/corrections/dust_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/corrections/ivar_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/data_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29855 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)    98923 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/expected_fluxes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/least_squares/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/least_squares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/masks/absorber_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/masks/bal_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/masks/dla_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/masks/lines_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/quasar_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.818627 picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/rejection_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.822627 picca-8.1.0/py/picca/delta_extraction/rejection_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/rejection_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/delta_extraction/utils_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.822627 picca-8.1.0/py/picca/pk1d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/pk1d/compute_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39831 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/pk1d/postproc_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/pk1d/prep_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/pk1d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/prep_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/raw_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.822627 picca-8.1.0/py/picca/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.822627 picca-8.1.0/py/picca/tests/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/delta_extraction/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/delta_extraction/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-03 14:30:09.000000 picca-8.1.0/py/picca/tests/delta_extraction/correction_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/mask_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/scripts_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/delta_extraction/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/test_2_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/test_3_cor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/wedgize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-08-03 14:30:11.000000 picca-8.1.0/py/picca/xcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:30:20.810627 picca-8.1.0/py/picca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-03 14:30:20.000000 picca-8.1.0/py/picca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-08-03 14:30:20.000000 picca-8.1.0/py/picca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:30:20.000000 picca-8.1.0/py/picca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 14:30:20.000000 picca-8.1.0/py/picca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 14:30:20.000000 picca-8.1.0/py/picca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 14:30:11.000000 picca-8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:30:20.822627 picca-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 14:30:11.000000 picca-8.1.0/setup.py
```

### Comparing `picca-8.0.0/LICENSE` & `picca-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/PKG-INFO` & `picca-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 8.0.0
+Version: 8.1.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-8.0.0/README.md` & `picca-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_Pk1D.py` & `picca-8.1.0/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_Pk1D_postprocess.py` & `picca-8.1.0/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_cf.py` & `picca-8.1.0/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_cf1d.py` & `picca-8.1.0/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_cf_angl.py` & `picca-8.1.0/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_co.py` & `picca-8.1.0/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_coadd_zint.py` & `picca-8.1.0/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_compute_fvoigt.py` & `picca-8.1.0/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_compute_pk_pksb.py` & `picca-8.1.0/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_convert_transmission.py` & `picca-8.1.0/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_delta_extraction.py` & `picca-8.1.0/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_dmat.py` & `picca-8.1.0/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_export.py` & `picca-8.1.0/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_export_co.py` & `picca-8.1.0/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_export_cross_covariance.py` & `picca-8.1.0/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_metal_dmat.py` & `picca-8.1.0/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_metal_xdmat.py` & `picca-8.1.0/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_nersc_submit.py` & `picca-8.1.0/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_pk2fits.py` & `picca-8.1.0/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_plot_pk1d.py` & `picca-8.1.0/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_reduce_spall.py` & `picca-8.1.0/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_wick.py` & `picca-8.1.0/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_xcf.py` & `picca-8.1.0/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_xcf1d.py` & `picca-8.1.0/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_xcf_angl.py` & `picca-8.1.0/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_xdmat.py` & `picca-8.1.0/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/bin/picca_xwick.py` & `picca-8.1.0/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_Pk1D.py` & `picca-8.1.0/py/picca/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_Pk1D_postprocess.py` & `picca-8.1.0/py/picca/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_cf.py` & `picca-8.1.0/py/picca/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_cf1d.py` & `picca-8.1.0/py/picca/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_cf_angl.py` & `picca-8.1.0/py/picca/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_co.py` & `picca-8.1.0/py/picca/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_coadd_zint.py` & `picca-8.1.0/py/picca/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_compute_fvoigt.py` & `picca-8.1.0/py/picca/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_compute_pk_pksb.py` & `picca-8.1.0/py/picca/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_convert_transmission.py` & `picca-8.1.0/py/picca/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_delta_extraction.py` & `picca-8.1.0/py/picca/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_dmat.py` & `picca-8.1.0/py/picca/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_export.py` & `picca-8.1.0/py/picca/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_export_co.py` & `picca-8.1.0/py/picca/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_export_cross_covariance.py` & `picca-8.1.0/py/picca/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_metal_dmat.py` & `picca-8.1.0/py/picca/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_metal_xdmat.py` & `picca-8.1.0/py/picca/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_nersc_submit.py` & `picca-8.1.0/py/picca/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_pk2fits.py` & `picca-8.1.0/py/picca/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_plot_pk1d.py` & `picca-8.1.0/py/picca/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_reduce_spall.py` & `picca-8.1.0/py/picca/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_wick.py` & `picca-8.1.0/py/picca/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_xcf.py` & `picca-8.1.0/py/picca/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_xcf1d.py` & `picca-8.1.0/py/picca/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_xcf_angl.py` & `picca-8.1.0/py/picca/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_xdmat.py` & `picca-8.1.0/py/picca/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/bin/picca_xwick.py` & `picca-8.1.0/py/picca/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/cf.py` & `picca-8.1.0/py/picca/cf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/co.py` & `picca-8.1.0/py/picca/co.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/constants.py` & `picca-8.1.0/py/picca/constants.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/converters.py` & `picca-8.1.0/py/picca/converters.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/data.py` & `picca-8.1.0/py/picca/data.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_object.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_object.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py` & `picca-8.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/config.py` & `picca-8.1.0/py/picca/delta_extraction/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 try:
     THIS_DIR = os.path.dirname(os.path.abspath(__file__))
     PICCA_BASE = THIS_DIR.split("py/picca")[0]
     git_hash = git.Repo(PICCA_BASE).head.object.hexsha
 except InvalidGitRepositoryError:  # pragma: no cover
     git_hash = metadata.metadata('picca')['Summary'].split(':')[-1]
+picca_version = metadata.metadata('picca')['Version']
 
 accepted_corrections_options = [
     "num corrections", "type {int}", "module name {int}"
 ]
 accepted_data_options = ["type", "module name"]
 accepted_expected_flux_options = ["type", "module name"]
 accepted_general_options = [
@@ -45,14 +46,15 @@
         "logging level console": "PROGRESS",
         "logging level file": "PROGRESS",
         "num processors": 0,
     },
     "run specs": {
         "git hash": git_hash,
         "timestamp": str(datetime.now()),
+        "version": picca_version,
     }
 }
 
 
 class Config:
     """Class to manage the configuration file
```

### Comparing `picca-8.0.0/py/picca/delta_extraction/correction.py` & `picca-8.1.0/py/picca/delta_extraction/correction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/corrections/calibration_correction.py` & `picca-8.1.0/py/picca/delta_extraction/corrections/calibration_correction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/corrections/dust_correction.py` & `picca-8.1.0/py/picca/delta_extraction/corrections/dust_correction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/corrections/ivar_correction.py` & `picca-8.1.0/py/picca/delta_extraction/corrections/ivar_correction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py` & `picca-8.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data.py` & `picca-8.1.0/py/picca/delta_extraction/data.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py` & `picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py` & `picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py` & `picca-8.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py` & `picca-8.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py` & `picca-8.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/errors.py` & `picca-8.1.0/py/picca/delta_extraction/errors.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/utils.py` & `picca-8.1.0/py/picca/delta_extraction/expected_fluxes/utils.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py` & `picca-8.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py` & `picca-8.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/mask.py` & `picca-8.1.0/py/picca/delta_extraction/mask.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/masks/absorber_mask.py` & `picca-8.1.0/py/picca/delta_extraction/masks/absorber_mask.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/masks/bal_mask.py` & `picca-8.1.0/py/picca/delta_extraction/masks/bal_mask.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/masks/dla_mask.py` & `picca-8.1.0/py/picca/delta_extraction/masks/dla_mask.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/masks/lines_mask.py` & `picca-8.1.0/py/picca/delta_extraction/masks/lines_mask.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/quasar_catalogue.py` & `picca-8.1.0/py/picca/delta_extraction/quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py` & `picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py` & `picca-8.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/rejection_log.py` & `picca-8.1.0/py/picca/delta_extraction/rejection_log.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py` & `picca-8.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py` & `picca-8.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/survey.py` & `picca-8.1.0/py/picca/delta_extraction/survey.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/utils.py` & `picca-8.1.0/py/picca/delta_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/delta_extraction/utils_pk1d.py` & `picca-8.1.0/py/picca/delta_extraction/utils_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/io.py` & `picca-8.1.0/py/picca/io.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/pk1d/compute_pk1d.py` & `picca-8.1.0/py/picca/pk1d/compute_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/pk1d/postproc_pk1d.py` & `picca-8.1.0/py/picca/pk1d/postproc_pk1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -652,15 +652,14 @@
             min_array,
             max_array,
             median_array,
             snrfit_array,
         )
 
     for ikbin, kbin in enumerate(kbin_edges[:-1]):  # Main loop 2) k bins
-
         if apply_z_weights:  # special chunk selection in that case
             delta_z = zbin_centers[1:] - zbin_centers[:-1]
             if not np.allclose(delta_z, delta_z[0], atol=1.0e-3):
                 raise ValueError(
                     "z bins should have equal widths with apply_z_weights."
                 )
             delta_z = delta_z[0]
@@ -700,16 +699,44 @@
         index_zbin_array[ikbin] = izbin
 
         # Counts the number of chunks in each (z,k) bin
         num_chunks = np.ma.count(p1d_table["k"][select])
 
         n_array[ikbin] = num_chunks
 
-        for icol, col in enumerate(p1d_table_cols):
+        if weight_method == "fit_snr":
+            snr_bin_edges = np.arange(
+                MEANPK_FITRANGE_SNR[0], MEANPK_FITRANGE_SNR[1] + 1, 1
+            )
+            snr_bins = (snr_bin_edges[:-1] + snr_bin_edges[1:]) / 2
+
+            p1d_values = p1d_table["Pk"][select]
+            data_snr = p1d_table["forest_snr"][select]
+
+            data_snr = data_snr[(~np.isnan(p1d_values)) & (~np.isnan(data_snr))]
+            p1d_values = p1d_values[(~np.isnan(p1d_values)) & (~np.isnan(data_snr))]
+
+            standard_dev, _, _ = binned_statistic(
+                data_snr, p1d_values, statistic="std", bins=snr_bin_edges
+            )
+            standard_dev_full = np.copy(standard_dev)
+            standard_dev = standard_dev[~np.isnan(standard_dev)]
+            snr_bins = snr_bins[~np.isnan(standard_dev)]
+            coef, *_ = curve_fit(
+                fitfunc_variance_pk1d,
+                snr_bins,
+                standard_dev**2,
+                bounds=(0, np.inf),
+            )
+            data_snr[data_snr > MEANPK_FITRANGE_SNR[1]] = MEANPK_FITRANGE_SNR[1]
+            data_snr[data_snr < 1.01] = 1.01
+            variance_estimated = fitfunc_variance_pk1d(data_snr, *coef)
+            weights = 1.0 / variance_estimated
 
+        for icol, col in enumerate(p1d_table_cols):
             if num_chunks == 0:
                 userprint(
                     "Warning: 0 chunks found in bin "
                     + str(zbin_edges[izbin])
                     + "<z<"
                     + str(zbin_edges[izbin + 1])
                     + ", "
@@ -722,58 +749,54 @@
             if weight_method == "fit_snr":
                 snr_bin_edges = np.arange(
                     MEANPK_FITRANGE_SNR[0], MEANPK_FITRANGE_SNR[1] + 1, 1
                 )
                 snr_bins = (snr_bin_edges[:-1] + snr_bin_edges[1:]) / 2
 
                 data_values = p1d_table[col][select]
-                data_snr = p1d_table["forest_snr"][select]
-                p1d_values = p1d_table["Pk"][select]
-                mask = np.isnan(data_values) | np.isnan(data_snr)
-                if len(mask[mask]) != 0:
-                    data_snr = data_snr[~mask]
-                    data_values = data_values[~mask]
-                    p1d_values = p1d_values[~mask]
+                data_values = data_values[
+                    (~np.isnan(p1d_values)) & (~np.isnan(data_snr))
+                ]
                 # Fit function to observed dispersion in P1D:
-                standard_dev, _, _ = binned_statistic(
-                    data_snr, p1d_values, statistic="std", bins=snr_bin_edges
+                standard_dev_col, _, _ = binned_statistic(
+                    data_snr, data_values, statistic="std", bins=snr_bin_edges
                 )
-                standard_dev_full = np.copy(standard_dev)
-                mask = np.isnan(standard_dev)
-                if len(mask[mask]) != 0:
-                    standard_dev = standard_dev[~mask]
-                    snr_bins = snr_bins[~mask]
+                standard_dev_col = standard_dev_col[~np.isnan(standard_dev)]
+
                 # the *_ is to ignore the rest of the return arguments
-                coef, *_ = curve_fit(
+
+                coef_col, *_ = curve_fit(
                     fitfunc_variance_pk1d,
                     snr_bins,
-                    standard_dev**2,
+                    standard_dev_col**2,
                     bounds=(0, np.inf),
                 )
 
                 # Model variance from fit function
                 data_snr[data_snr > MEANPK_FITRANGE_SNR[1]] = MEANPK_FITRANGE_SNR[1]
                 data_snr[data_snr < 1.01] = 1.01
-                variance_estimated = fitfunc_variance_pk1d(data_snr, *coef)
-                weights = 1.0 / variance_estimated
+                variance_estimated_col = fitfunc_variance_pk1d(data_snr, *coef_col)
+                weights_col = 1.0 / variance_estimated_col
                 if apply_z_weights:
                     weights *= redshift_weights
                 mean = np.average(data_values, weights=weights)
                 if apply_z_weights:
                     # Analytic expression for the re-weighted average:
-                    error = np.sqrt(np.sum(weights * redshift_weights)) / np.sum(
-                        weights
+                    error = np.sqrt(np.sum(weights_col * redshift_weights)) / np.sum(
+                        weights_col
                     )
                 else:
-                    error = np.sqrt(1.0 / np.sum(weights))
+                    error = np.sqrt(1.0 / np.sum(weights_col))
                 if col == "Pk":
-                    if len(mask[mask]) != 0:
-                        standard_dev = np.concatenate(
-                            [standard_dev, np.full(len(mask[mask]), np.nan)]
-                        )
+                    standard_dev = np.concatenate(
+                        [
+                            standard_dev,
+                            np.full(len(standard_dev[np.isnan(standard_dev)]), np.nan),
+                        ]
+                    )
                     snrfit_array[ikbin, 0:4] = [
                         zbin_centers[izbin],
                         (kbin + kbin_edges[ikbin + 1]) / 2.0,
                         coef[0],
                         coef[1],
                     ]
                     snrfit_array[ikbin, 4:] = standard_dev_full  # also save nan values
@@ -988,21 +1011,21 @@
                 # index of the (ikbin,ikbin2) coefficient on the bottom of the matrix
                 index_2 = (nbins_k * ikbin2) + ikbin
                 covariance_array[index_2] = covariance_array[index]
                 n_array[index_2] = n_array[index]
 
                 zbin_array[index_2] = zbin_centers[izbin]
                 index_zbin_array[index_2] = izbin
-                k1_array[index_2] = kbin_centers[ikbin]
-                k2_array[index_2] = kbin_centers[ikbin2]
+                k1_array[index_2] = kbin_centers[ikbin2]
+                k2_array[index_2] = kbin_centers[ikbin]
 
     # For fit_snr method, due to the SNR fitting scheme used for weighting,
     # the diagonal of the weigthed sample covariance matrix is not equal
     # to the error in mean P1D. This is tested on Ohio mocks.
-    # We choose to renormalize the covariance matrix.
+    # We choose to renormalize the whole covariance matrix.
     if weight_method == "fit_snr":
         # Third loop 1) k bins
         for ikbin in range(nbins_k):
             std_ikbin = mean_p1d_table["errorPk"][(nbins_k * izbin) + ikbin]
             # Third loop 2) k bins
             for ikbin2 in range(ikbin, nbins_k):
                 std_ikbin2 = mean_p1d_table["errorPk"][(nbins_k * izbin) + ikbin2]
```

### Comparing `picca-8.0.0/py/picca/pk1d/prep_pk1d.py` & `picca-8.1.0/py/picca/pk1d/prep_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/pk1d/utils.py` & `picca-8.1.0/py/picca/pk1d/utils.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/prep_del.py` & `picca-8.1.0/py/picca/prep_del.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/raw_io.py` & `picca-8.1.0/py/picca/raw_io.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/abstract_test.py` & `picca-8.1.0/py/picca/tests/delta_extraction/abstract_test.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/config_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/config_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/correction_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/correction_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/data_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/data_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/mask_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/mask_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/scripts_tests.py` & `picca-8.1.0/py/picca/tests/delta_extraction/scripts_tests.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/delta_extraction/test_utils.py` & `picca-8.1.0/py/picca/tests/delta_extraction/test_utils.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/test_2_pk1d.py` & `picca-8.1.0/py/picca/tests/test_2_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/test_3_cor.py` & `picca-8.1.0/py/picca/tests/test_3_cor.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/tests/test_helpers.py` & `picca-8.1.0/py/picca/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/utils.py` & `picca-8.1.0/py/picca/utils.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/wedgize.py` & `picca-8.1.0/py/picca/wedgize.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca/xcf.py` & `picca-8.1.0/py/picca/xcf.py`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/py/picca.egg-info/PKG-INFO` & `picca-8.1.0/py/picca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 8.0.0
+Version: 8.1.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-8.0.0/py/picca.egg-info/SOURCES.txt` & `picca-8.1.0/py/picca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picca-8.0.0/setup.py` & `picca-8.1.0/setup.py`

 * *Files identical despite different names*

