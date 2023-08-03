# Comparing `tmp/pyrfu-2.4.5.tar.gz` & `tmp/pyrfu-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfu-2.4.5.tar", last modified: Tue Aug  1 09:02:49 2023, max compression
+gzip compressed data, was "pyrfu-2.4.6.tar", last modified: Thu Aug  3 20:53:13 2023, max compression
```

## Comparing `pyrfu-2.4.5.tar` & `pyrfu-2.4.6.tar`

### file list

```diff
@@ -1,288 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.175972 pyrfu-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 09:02:28.000000 pyrfu-2.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 09:02:28.000000 pyrfu-2.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-01 09:02:49.175972 pyrfu-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-08-01 09:02:28.000000 pyrfu-2.4.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.075971 pyrfu-2.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/disp_surf_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/one_fluid_dispersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.083971 pyrfu-2.4.5/pyrfu/lp/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/photo_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/thermal_current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.123971 pyrfu-2.4.5/pyrfu/mms/
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/ancillary.json
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/calculate_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/copy_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/copy_files_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/correct_edp_probe_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_get_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_get_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/def2psd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dft_time_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/download_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dpf2psd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dsl2gse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dsl2gsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_ang_ang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_skymap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_omni.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad_combine_sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad_spinavg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_proton_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_skymap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_skymap_combine_sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_spec_combine_sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_spin_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/estimate_phase_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_active_eyes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_bad_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_correct_energies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_energy_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_flat_field_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_omni.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pad_spinavg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pitch_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_remove_bad_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_remove_sun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_sector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_spin_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_split_integral_ch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/fft_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/fk_power_spectrum_4sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_eis_allt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_feeps_alleyes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_feeps_omni.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_hpca_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_pitch_angle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_calc_anodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_energies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_spin_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/lh_wave_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/list_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/list_files_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/load_ancillary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/load_brst_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_kappa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_rq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_vdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/mms_keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/probe_align_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd2def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd2dpf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd_rebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/read_feeps_sector_masks_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_edist_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_idist_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_imoms_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/rotate_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/scpot2ne.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/spectr_to_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.131971 pyrfu-2.4.5/pyrfu/mms/sun/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_elim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_omni.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_to_e64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/whistler_b2e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.135971 pyrfu-2.4.5/pyrfu/models/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/igrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    26798 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/igrf13coeffs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/magnetopause_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.143972 pyrfu-2.4.5/pyrfu/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/add_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/annotate_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/colorbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.143972 pyrfu-2.4.5/pyrfu/plot/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    43962 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/make_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/mms_pl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/pl_scatter_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/pl_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_ang_ang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_clines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_magnetosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_reduced_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_sitl_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_spectr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_surf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/span_tint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.171972 pyrfu-2.4.5/pyrfu/pyrf/
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/autocorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/average_vdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/avg_4sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_grad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_j.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_v.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_ag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_agyro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_dng.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_dt.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_sqrtq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cart2sph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cart2sph_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cdfepoch2datetime64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/compress_cwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/convert_fac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/corr_deriv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cotrans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/date_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime2iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642ttns.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642unix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dec_par_perp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dist_append.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dynamic_press.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/e_vxb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/eb_nrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ebsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/edb.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/end.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/extend_tint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/filt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/find_closest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/get_omni_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/gse2gsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/histogram2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/increments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/int_sph_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iplasma_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso2unix.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012timevec.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/l_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/lowpass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/magnetosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/match_phibe_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/match_phibe_v.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean_bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/medfilt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/median_bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/movmean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mva.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mva_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/new_xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pid_4sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/plasma_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/plasma_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/poynting_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pres_anis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/psd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pvi_4sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/read_cdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/remove_repeated_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_models_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/sph2cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/st_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/struct_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/t_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/time_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/timevec2iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/transformation_indices.json
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_append.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_skymap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_tensor_xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_vec_xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ttns2datetime64.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/unix2datetime64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/vht.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wave_fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wavepolarize_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/waverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.171972 pyrfu-2.4.5/pyrfu/solo/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/db_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/read_lfr_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/read_tnr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.175972 pyrfu-2.4.5/pyrfu/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/test_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/test_pyrf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:02:49.175972 pyrfu-2.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.465364 pyrfu-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 20:52:52.000000 pyrfu-2.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 20:52:52.000000 pyrfu-2.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-08-03 20:53:13.465364 pyrfu-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-08-03 20:52:52.000000 pyrfu-2.4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.409364 pyrfu-2.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-03 20:52:52.000000 pyrfu-2.4.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.409364 pyrfu-2.4.6/pyrfu/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.413364 pyrfu-2.4.6/pyrfu/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/dispersion/disp_surf_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/dispersion/one_fluid_dispersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.413364 pyrfu-2.4.6/pyrfu/lp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/lp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/lp/photo_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/lp/thermal_current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.429364 pyrfu-2.4.6/pyrfu/mms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/ancillary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/calculate_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/copy_files_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/correct_edp_probe_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/db_get_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/db_get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/def2psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/dft_time_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/download_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/dpf2psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/dsl2gse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/dsl2gsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_ang_ang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_pad_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_pad_spinavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_proton_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_skymap_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_spec_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/eis_spin_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/estimate_phase_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_active_eyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_bad_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_correct_energies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_energy_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_flat_field_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_pad_spinavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_pitch_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_remove_bad_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_remove_sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_sector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_spin_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/feeps_split_integral_ch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/fft_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/fk_power_spectrum_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_eis_allt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_feeps_alleyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_feeps_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_hpca_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_pitch_angle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/hpca_calc_anodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/hpca_energies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/hpca_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/hpca_spin_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/lh_wave_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/list_files_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/load_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/load_brst_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/make_model_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/make_model_rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/make_model_vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/mms_keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/probe_align_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/psd2def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/psd2dpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/psd_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/psd_rebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/read_feeps_sector_masks_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/remove_edist_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/remove_idist_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/remove_imoms_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/rotate_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/scpot2ne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/spectr_to_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.437364 pyrfu-2.4.6/pyrfu/mms/sun/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/vdf_elim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/vdf_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/vdf_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/vdf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/vdf_to_e64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/mms/whistler_b2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.437364 pyrfu-2.4.6/pyrfu/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/models/igrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26798 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/models/igrf13coeffs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/models/magnetopause_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.441364 pyrfu-2.4.6/pyrfu/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/add_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/annotate_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/colorbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.441364 pyrfu-2.4.6/pyrfu/plot/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    43962 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/make_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/mms_pl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/pl_scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/pl_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_ang_ang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_clines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_magnetosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_reduced_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_sitl_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_spectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/plot_surf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/span_tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/plot/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.465364 pyrfu-2.4.6/pyrfu/pyrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/average_vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/avg_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/c_4_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/c_4_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/c_4_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/c_4_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_ag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_agyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_dng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/calc_sqrtq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/cart2sph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/cart2sph_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/cdfepoch2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/compress_cwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/convert_fac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/corr_deriv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/cotrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/date_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/datetime2iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/datetime642iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/datetime642ttns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/datetime642unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/dec_par_perp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/dist_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/dynamic_press.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/e_vxb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/eb_nrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35991 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ebsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/edb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/extend_tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/find_closest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/get_omni_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/gse2gsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/histogram2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/increments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/int_sph_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/iplasma_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/iso86012datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/iso86012datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/iso86012timevec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/iso86012unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/l_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/lowpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/magnetosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/match_phibe_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/match_phibe_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/mean_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/medfilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/median_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/movmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/mva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/mva_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/new_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/optimize_nbins_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/optimize_nbins_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/pid_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/plasma_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/plasma_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/poynting_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/pres_anis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/pvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/pvi_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/read_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/remove_repeated_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/shock_models_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/shock_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/shock_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/sph2cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/st_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/struct_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/t_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/time_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/timevec2iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/transformation_indices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_tensor_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ts_vec_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/ttns2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/unix2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/vht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/wave_fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/wavepolarize_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/pyrf/waverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.465364 pyrfu-2.4.6/pyrfu/solo/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/solo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/solo/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/solo/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/solo/read_lfr_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/solo/read_tnr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.465364 pyrfu-2.4.6/pyrfu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/tests/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68831 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/tests/test_pyrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 20:52:52.000000 pyrfu-2.4.6/pyrfu/tests/test_solo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:53:13.413364 pyrfu-2.4.6/pyrfu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-08-03 20:53:13.000000 pyrfu-2.4.6/pyrfu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-08-03 20:53:13.000000 pyrfu-2.4.6/pyrfu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:53:13.000000 pyrfu-2.4.6/pyrfu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-03 20:53:13.000000 pyrfu-2.4.6/pyrfu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 20:53:13.000000 pyrfu-2.4.6/pyrfu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:53:13.465364 pyrfu-2.4.6/setup.cfg
```

### Comparing `pyrfu-2.4.5/LICENSE.txt` & `pyrfu-2.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/PKG-INFO` & `pyrfu-2.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -29,25 +29,27 @@
 Project-URL: documentation, https://pyrfu.readthedocs.io/en/latest/
 Project-URL: source, https://github.com/louis-richard/irfu-python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: MS-DOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
@@ -81,14 +83,20 @@
 
 .. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
 .. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
+.. |CodeQL| image:: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml/badge.svg
+.. _CodeQL: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml
+
+.. |CodeCov| image:: https://codecov.io/gh/louis-richard/irfu-python/coverage.svg?branch=main
+.. _CodeCov: https://codecov.io/gh/louis-richard/irfu-python/branch/main
+
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
 .. |Commits| image:: https://img.shields.io/github/last-commit/louis-richard/irfu-python?logo=github&color=9cf
 .. _Commits: https://github.com/louis-richard/irfu-python/commits/master
 
 .. |Readthedocs| image:: https://img.shields.io/readthedocs/pyrfu?logo=read-the-docs&color=blueviolet
@@ -97,84 +105,73 @@
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
 |License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
-|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|PyLintB|_ |CodeQL|_ |CodeCov|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
-The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
-Magnetospheric MultiScale (MMS) mission.
+The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
-.. end-marker-intro-do-not-remove
-
-Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
-
-
 Quickstart
 ==========
 
-Installing pyrfu with pip (`more details here`_):
-
-.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
+Installing pyrfu with pip (`more details here <https://pyrfu.readthedocs.io/en/latest/installation.html>`_):
 
 .. code-block:: console
 
     $ python -m pip install pyrfu
     # or
     $ python -m pip install --user pyrfu
 
-Import `pyrfu.mms`_ package with routines specific to work with the
+Import `pyrfu.mms <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html>`_ package with routines specific to work with the
 Magnetospheric Multiscale mission (MMS)
 
-.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
-
 .. code:: python
 
     from pyrfu import mms
 
 Setup path to MMS data
 
 .. code:: python
 
     mms.db_init("/Volumes/mms")
 
+
 Load magnetic field and ion bulk velocity data
 
 .. code:: python
 
     tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
     b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
     v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-Import `pyrfu.pyrf`_ package with generic routines
 
-.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
+Import `pyrfu.pyrf <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html>`_ package with generic routines
 
 .. code:: python
 
     from pyrfu import pyrf
 
 Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
     v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
-Import `pyrfu.plot`_ package with plotting routines
-
-.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
+Import `pyrfu.plot <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html>`_ package with plotting routines
 
 .. code:: python
 
     from pyrfu import plot
 
+
 Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
     import matplotlib.pyplot as plt
 
     f, axs = plt.subplots(2, sharex="all")
@@ -182,24 +179,33 @@
     axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
     axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
 
     plot.plot_line(axs[1], v_gsm_i)
     axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
     axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
+.. end-marker-intro-do-not-remove
+
+Documentation
+=============
+Full documentation can be found on `pyrfu.readthedocs.io <https://pyrfu.readthedocs.io/en/latest/index.html>`_
+
+Examples
+========
+A list of examples is available `here <https://pyrfu.readthedocs.io/en/latest/examples/index.html>`_
 
 Credits
--------
+=======
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
----------------
+===============
 Please use the following to acknowledge use of pyrfu in your publications:
 Data analysis was performed using the pyrfu analysis package available at https://github.com/louis-richard/irfu-python
 
 Additional Information
-----------------------
+======================
 MMS Science Data Center: https://lasp.colorado.edu/mms/sdc/public/
 
 MMS Datasets: https://lasp.colorado.edu/mms/sdc/public/datasets/
 
 MMS - Goddard Space Flight Center: http://mms.gsfc.nasa.gov/
```

### Comparing `pyrfu-2.4.5/README.rst` & `pyrfu-2.4.6/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 
 .. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
 .. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
+.. |CodeQL| image:: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml/badge.svg
+.. _CodeQL: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml
+
+.. |CodeCov| image:: https://codecov.io/gh/louis-richard/irfu-python/coverage.svg?branch=main
+.. _CodeCov: https://codecov.io/gh/louis-richard/irfu-python/branch/main
+
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
 .. |Commits| image:: https://img.shields.io/github/last-commit/louis-richard/irfu-python?logo=github&color=9cf
 .. _Commits: https://github.com/louis-richard/irfu-python/commits/master
 
 .. |Readthedocs| image:: https://img.shields.io/readthedocs/pyrfu?logo=read-the-docs&color=blueviolet
@@ -44,84 +50,73 @@
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
 |License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
-|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|PyLintB|_ |CodeQL|_ |CodeCov|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
-The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
-Magnetospheric MultiScale (MMS) mission.
+The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
-.. end-marker-intro-do-not-remove
-
-Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
-
-
 Quickstart
 ==========
 
-Installing pyrfu with pip (`more details here`_):
-
-.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
+Installing pyrfu with pip (`more details here <https://pyrfu.readthedocs.io/en/latest/installation.html>`_):
 
 .. code-block:: console
 
     $ python -m pip install pyrfu
     # or
     $ python -m pip install --user pyrfu
 
-Import `pyrfu.mms`_ package with routines specific to work with the
+Import `pyrfu.mms <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html>`_ package with routines specific to work with the
 Magnetospheric Multiscale mission (MMS)
 
-.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
-
 .. code:: python
 
     from pyrfu import mms
 
 Setup path to MMS data
 
 .. code:: python
 
     mms.db_init("/Volumes/mms")
 
+
 Load magnetic field and ion bulk velocity data
 
 .. code:: python
 
     tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
     b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
     v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-Import `pyrfu.pyrf`_ package with generic routines
 
-.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
+Import `pyrfu.pyrf <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html>`_ package with generic routines
 
 .. code:: python
 
     from pyrfu import pyrf
 
 Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
     v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
-Import `pyrfu.plot`_ package with plotting routines
-
-.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
+Import `pyrfu.plot <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html>`_ package with plotting routines
 
 .. code:: python
 
     from pyrfu import plot
 
+
 Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
     import matplotlib.pyplot as plt
 
     f, axs = plt.subplots(2, sharex="all")
@@ -129,24 +124,33 @@
     axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
     axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
 
     plot.plot_line(axs[1], v_gsm_i)
     axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
     axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
+.. end-marker-intro-do-not-remove
+
+Documentation
+=============
+Full documentation can be found on `pyrfu.readthedocs.io <https://pyrfu.readthedocs.io/en/latest/index.html>`_
+
+Examples
+========
+A list of examples is available `here <https://pyrfu.readthedocs.io/en/latest/examples/index.html>`_
 
 Credits
--------
+=======
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
----------------
+===============
 Please use the following to acknowledge use of pyrfu in your publications:
 Data analysis was performed using the pyrfu analysis package available at https://github.com/louis-richard/irfu-python
 
 Additional Information
-----------------------
+======================
 MMS Science Data Center: https://lasp.colorado.edu/mms/sdc/public/
 
 MMS Datasets: https://lasp.colorado.edu/mms/sdc/public/datasets/
 
 MMS - Goddard Space Flight Center: http://mms.gsfc.nasa.gov/
```

### Comparing `pyrfu-2.4.5/docs/conf.py` & `pyrfu-2.4.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyproject.toml` & `pyrfu-2.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,38 @@
     "setuptools>=42",
     "wheel==0.38.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfu"
-version = "2.4.5"
+version = "2.4.6"
 description = "Python Space Physics (RymdFysik) Utilities"
 readme = "README.rst"
 authors = [{ name = "Louis RICHARD", email = "louir@irfu.se" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Other Environment",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
+    "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft",
     "Operating System :: Microsoft :: MS-DOS",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
     "cdflib>=1.0.4",
     "geopack>=1.0.9",
     "matplotlib>=3.5.2",
@@ -106,22 +108,23 @@
     ancillary.json,
     config.json,
     feeps_bad_data.json,
     igrf13coeffs.csv,
     mms_keys.json,
     transformation_indices.json,
     test_pyrf.py,
-    test_dispersion.py
+    test_dispersion.py,
+    test_solo.py
 """
 ignored-modules = "scipy,cdflib"
 
 [tool.bumpver]
 current_version = "2.4.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
-tag             = true
+tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "pyrfu/__init__.py" = ["{version}", "Copyright 2020-YYYY"]
```

### Comparing `pyrfu-2.4.5/pyrfu/dispersion/disp_surf_calc.py` & `pyrfu-2.4.6/pyrfu/dispersion/disp_surf_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/dispersion/one_fluid_dispersion.py` & `pyrfu-2.4.6/pyrfu/dispersion/one_fluid_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/lp/__init__.py` & `pyrfu-2.4.6/pyrfu/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/lp/photo_current.py` & `pyrfu-2.4.6/pyrfu/lp/photo_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/lp/thermal_current.py` & `pyrfu-2.4.6/pyrfu/lp/thermal_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/__init__.py` & `pyrfu-2.4.6/pyrfu/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/ancillary.json` & `pyrfu-2.4.6/pyrfu/mms/ancillary.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/calculate_epsilon.py` & `pyrfu-2.4.6/pyrfu/mms/calculate_epsilon.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/copy_files.py` & `pyrfu-2.4.6/pyrfu/mms/copy_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/copy_files_ancillary.py` & `pyrfu-2.4.6/pyrfu/mms/copy_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/correct_edp_probe_timing.py` & `pyrfu-2.4.6/pyrfu/mms/correct_edp_probe_timing.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/db_get_ts.py` & `pyrfu-2.4.6/pyrfu/mms/db_get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/db_get_variable.py` & `pyrfu-2.4.6/pyrfu/mms/db_get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/db_init.py` & `pyrfu-2.4.6/pyrfu/mms/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/def2psd.py` & `pyrfu-2.4.6/pyrfu/mms/def2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/dft_time_shift.py` & `pyrfu-2.4.6/pyrfu/mms/dft_time_shift.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/download_ancillary.py` & `pyrfu-2.4.6/pyrfu/mms/download_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/download_data.py` & `pyrfu-2.4.6/pyrfu/mms/download_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/dpf2psd.py` & `pyrfu-2.4.6/pyrfu/mms/dpf2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/dsl2gse.py` & `pyrfu-2.4.6/pyrfu/mms/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/dsl2gsm.py` & `pyrfu-2.4.6/pyrfu/mms/dsl2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_ang_ang.py` & `pyrfu-2.4.6/pyrfu/mms/eis_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_pad.py` & `pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_skymap.py` & `pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_spec.py` & `pyrfu-2.4.6/pyrfu/mms/eis_combine_proton_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_moments.py` & `pyrfu-2.4.6/pyrfu/mms/eis_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_omni.py` & `pyrfu-2.4.6/pyrfu/mms/eis_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_pad.py` & `pyrfu-2.4.6/pyrfu/mms/eis_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_pad_combine_sc.py` & `pyrfu-2.4.6/pyrfu/mms/eis_pad_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_pad_spinavg.py` & `pyrfu-2.4.6/pyrfu/mms/eis_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_proton_correction.py` & `pyrfu-2.4.6/pyrfu/mms/eis_proton_correction.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_skymap.py` & `pyrfu-2.4.6/pyrfu/mms/eis_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_skymap_combine_sc.py` & `pyrfu-2.4.6/pyrfu/mms/eis_skymap_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_spec_combine_sc.py` & `pyrfu-2.4.6/pyrfu/mms/eis_spec_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/eis_spin_avg.py` & `pyrfu-2.4.6/pyrfu/mms/eis_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/estimate_phase_speed.py` & `pyrfu-2.4.6/pyrfu/mms/estimate_phase_speed.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_active_eyes.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_active_eyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_bad_data.json` & `pyrfu-2.4.6/pyrfu/mms/feeps_bad_data.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_correct_energies.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_correct_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_energy_table.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_energy_table.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_flat_field_corrections.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_flat_field_corrections.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_omni.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_pad.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_pad_spinavg.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_pitch_angles.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_pitch_angles.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_remove_bad_data.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_remove_bad_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_remove_sun.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_remove_sun.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_sector_spec.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_sector_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_spin_avg.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/feeps_split_integral_ch.py` & `pyrfu-2.4.6/pyrfu/mms/feeps_split_integral_ch.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/fft_bandpass.py` & `pyrfu-2.4.6/pyrfu/mms/fft_bandpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/fk_power_spectrum_4sc.py` & `pyrfu-2.4.6/pyrfu/mms/fk_power_spectrum_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_data.py` & `pyrfu-2.4.6/pyrfu/mms/get_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_dist.py` & `pyrfu-2.4.6/pyrfu/mms/get_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_eis_allt.py` & `pyrfu-2.4.6/pyrfu/mms/get_eis_allt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_feeps_alleyes.py` & `pyrfu-2.4.6/pyrfu/mms/get_feeps_alleyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_feeps_omni.py` & `pyrfu-2.4.6/pyrfu/mms/get_feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_hpca_dist.py` & `pyrfu-2.4.6/pyrfu/mms/get_hpca_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_pitch_angle_dist.py` & `pyrfu-2.4.6/pyrfu/mms/get_pitch_angle_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_ts.py` & `pyrfu-2.4.6/pyrfu/mms/get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/get_variable.py` & `pyrfu-2.4.6/pyrfu/mms/get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/hpca_calc_anodes.py` & `pyrfu-2.4.6/pyrfu/mms/hpca_calc_anodes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/hpca_energies.py` & `pyrfu-2.4.6/pyrfu/mms/hpca_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/hpca_pad.py` & `pyrfu-2.4.6/pyrfu/mms/hpca_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/hpca_spin_sum.py` & `pyrfu-2.4.6/pyrfu/mms/hpca_spin_sum.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/lh_wave_analysis.py` & `pyrfu-2.4.6/pyrfu/mms/lh_wave_analysis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/list_files.py` & `pyrfu-2.4.6/pyrfu/mms/list_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/list_files_ancillary.py` & `pyrfu-2.4.6/pyrfu/mms/list_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/load_ancillary.py` & `pyrfu-2.4.6/pyrfu/mms/load_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/load_brst_segments.py` & `pyrfu-2.4.6/pyrfu/mms/load_brst_segments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/make_model_kappa.py` & `pyrfu-2.4.6/pyrfu/mms/make_model_kappa.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/make_model_rq.py` & `pyrfu-2.4.6/pyrfu/mms/make_model_rq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/make_model_vdf.py` & `pyrfu-2.4.6/pyrfu/mms/make_model_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/mms_keys.json` & `pyrfu-2.4.6/pyrfu/mms/mms_keys.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/probe_align_times.py` & `pyrfu-2.4.6/pyrfu/mms/probe_align_times.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/psd2def.py` & `pyrfu-2.4.6/pyrfu/mms/psd2def.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/psd2dpf.py` & `pyrfu-2.4.6/pyrfu/mms/psd2dpf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/psd_moments.py` & `pyrfu-2.4.6/pyrfu/mms/psd_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/psd_rebin.py` & `pyrfu-2.4.6/pyrfu/mms/psd_rebin.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/read_feeps_sector_masks_csv.py` & `pyrfu-2.4.6/pyrfu/mms/read_feeps_sector_masks_csv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/reduce.py` & `pyrfu-2.4.6/pyrfu/mms/reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/remove_edist_background.py` & `pyrfu-2.4.6/pyrfu/mms/remove_edist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/remove_idist_background.py` & `pyrfu-2.4.6/pyrfu/mms/remove_idist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/remove_imoms_background.py` & `pyrfu-2.4.6/pyrfu/mms/remove_imoms_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/rotate_tensor.py` & `pyrfu-2.4.6/pyrfu/mms/rotate_tensor.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/scpot2ne.py` & `pyrfu-2.4.6/pyrfu/mms/scpot2ne.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/spectr_to_dataset.py` & `pyrfu-2.4.6/pyrfu/mms/spectr_to_dataset.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/tokenize.py` & `pyrfu-2.4.6/pyrfu/mms/tokenize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/vdf_elim.py` & `pyrfu-2.4.6/pyrfu/mms/vdf_elim.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/vdf_omni.py` & `pyrfu-2.4.6/pyrfu/mms/vdf_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/vdf_projection.py` & `pyrfu-2.4.6/pyrfu/mms/vdf_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/vdf_reduce.py` & `pyrfu-2.4.6/pyrfu/mms/vdf_reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/vdf_to_e64.py` & `pyrfu-2.4.6/pyrfu/mms/vdf_to_e64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/mms/whistler_b2e.py` & `pyrfu-2.4.6/pyrfu/mms/whistler_b2e.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/models/igrf.py` & `pyrfu-2.4.6/pyrfu/models/igrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/models/igrf13coeffs.csv` & `pyrfu-2.4.6/pyrfu/models/igrf13coeffs.csv`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/models/magnetopause_normal.py` & `pyrfu-2.4.6/pyrfu/models/magnetopause_normal.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/__init__.py` & `pyrfu-2.4.6/pyrfu/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/add_position.py` & `pyrfu-2.4.6/pyrfu/plot/add_position.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/annotate_heatmap.py` & `pyrfu-2.4.6/pyrfu/plot/annotate_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/colorbar.py` & `pyrfu-2.4.6/pyrfu/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg` & `pyrfu-2.4.6/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/make_labels.py` & `pyrfu-2.4.6/pyrfu/plot/make_labels.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/mms_pl_config.py` & `pyrfu-2.4.6/pyrfu/plot/mms_pl_config.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/pl_scatter_matrix.py` & `pyrfu-2.4.6/pyrfu/plot/pl_scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/pl_tx.py` & `pyrfu-2.4.6/pyrfu/plot/pl_tx.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_ang_ang.py` & `pyrfu-2.4.6/pyrfu/plot/plot_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_clines.py` & `pyrfu-2.4.6/pyrfu/plot/plot_clines.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_heatmap.py` & `pyrfu-2.4.6/pyrfu/plot/plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_line.py` & `pyrfu-2.4.6/pyrfu/plot/plot_line.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_magnetosphere.py` & `pyrfu-2.4.6/pyrfu/plot/plot_magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_projection.py` & `pyrfu-2.4.6/pyrfu/plot/plot_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_reduced_2d.py` & `pyrfu-2.4.6/pyrfu/plot/plot_reduced_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_sitl_overview.py` & `pyrfu-2.4.6/pyrfu/plot/plot_sitl_overview.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_spectr.py` & `pyrfu-2.4.6/pyrfu/plot/plot_spectr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/plot_surf.py` & `pyrfu-2.4.6/pyrfu/plot/plot_surf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/span_tint.py` & `pyrfu-2.4.6/pyrfu/plot/span_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/plot/zoom.py` & `pyrfu-2.4.6/pyrfu/plot/zoom.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/__init__.py` & `pyrfu-2.4.6/pyrfu/pyrf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 from .gse2gsm import gse2gsm
 from .histogram import histogram
 from .histogram2d import histogram2d
 from .increments import increments
 from .int_sph_dist import int_sph_dist
 from .integrate import integrate
 from .iplasma_calc import iplasma_calc
-from .iso2unix import iso2unix
 from .iso86012datetime import iso86012datetime
 from .iso86012datetime64 import iso86012datetime64
 from .iso86012timevec import iso86012timevec
+from .iso86012unix import iso86012unix
 from .l_shell import l_shell
 from .lowpass import lowpass
 from .magnetosphere import magnetosphere
 from .match_phibe_dir import match_phibe_dir
 from .match_phibe_v import match_phibe_v
 from .mean import mean
 from .mean_bins import mean_bins
@@ -159,15 +159,15 @@
     "gse2gsm",
     "histogram",
     "histogram2d",
     "increments",
     "int_sph_dist",
     "integrate",
     "iplasma_calc",
-    "iso2unix",
+    "iso86012unix",
     "iso86012datetime",
     "iso86012datetime64",
     "iso86012timevec",
     "l_shell",
     "lowpass",
     "magnetosphere",
     "match_phibe_dir",
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/autocorr.py` & `pyrfu-2.4.6/pyrfu/pyrf/autocorr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/average_vdf.py` & `pyrfu-2.4.6/pyrfu/pyrf/average_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/avg_4sc.py` & `pyrfu-2.4.6/pyrfu/pyrf/avg_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/c_4_grad.py` & `pyrfu-2.4.6/pyrfu/pyrf/c_4_grad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/c_4_j.py` & `pyrfu-2.4.6/pyrfu/pyrf/c_4_j.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/c_4_k.py` & `pyrfu-2.4.6/pyrfu/pyrf/c_4_k.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/c_4_v.py` & `pyrfu-2.4.6/pyrfu/pyrf/c_4_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_ag.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_ag.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_agyro.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_agyro.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_dng.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_dng.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_dt.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_dt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_fs.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_fs.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/calc_sqrtq.py` & `pyrfu-2.4.6/pyrfu/pyrf/calc_sqrtq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/cart2sph.py` & `pyrfu-2.4.6/pyrfu/pyrf/cart2sph.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/cart2sph_ts.py` & `pyrfu-2.4.6/pyrfu/pyrf/cart2sph_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/cdfepoch2datetime64.py` & `pyrfu-2.4.6/pyrfu/pyrf/cdfepoch2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/compress_cwt.py` & `pyrfu-2.4.6/pyrfu/pyrf/compress_cwt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party import
 import numba
 import numpy as np
+import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-@numba.jit(nopython=True, parallel=True)
+@numba.jit(cache=True, fastmath=True, nopython=True, parallel=True)
 def _compress_cwt_1d(cwt, nc: int = 100):
     nf = cwt.shape[1]
     idxs = np.arange(
         start=int(nc / 2),
         stop=len(cwt) - int(nc / 2),
         step=nc,
         dtype=np.int64,
@@ -33,15 +34,15 @@
 
 
 def compress_cwt(cwt, nc: int = 100):
     r"""Compress the wavelet transform averaging of nc time steps.
 
     Parameters
     ----------
-    cwt : xarray.DataArray
+    cwt : xarray.Dataset
         Wavelet transform to compress.
     nc : int, Optional
         Number of time steps for averaging. Default is 100.
 
     Returns
     -------
     cwt_t : xarray.DataArray
@@ -51,14 +52,16 @@
     cwt_y : ndarray
         Compressed wavelet transform of the second component of the field.
     cwt_z : ndarray
         Compressed wavelet transform of the third component of the field.
 
     """
 
+    assert isinstance(cwt, xr.Dataset), "cwt must be an xarray.Dataset"
+
     indices = np.arange(
         int(nc / 2),
         len(cwt.time.data) - int(nc / 2),
         step=nc,
         dtype=np.int64,
     )
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/convert_fac.py` & `pyrfu-2.4.6/pyrfu/pyrf/convert_fac.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,52 +77,60 @@
     assert isinstance(b_bgd, xr.DataArray), "b_xyz must be a xarray.DataArray"
 
     assert r_xyz is None or isinstance(
         r_xyz,
         (xr.DataArray, list, np.ndarray),
     )
 
-    if r_xyz is None:
-        r_xyz = np.array([1, 0, 0])
-
     if len(inp) != len(b_bgd):
         b_bgd = resample(b_bgd, inp, f_s=calc_fs(inp))
 
     time, inp_data = [inp.time.data, inp.data]
 
-    # Normalize background magnetic field
-    b_hat = b_bgd / np.linalg.norm(b_bgd, axis=1, keepdims=True)
+    if r_xyz is None:
+        r_xyz = np.array([1, 0, 0])
 
     if isinstance(r_xyz, xr.DataArray):
         r_xyz = resample(r_xyz, b_bgd, f_s=calc_fs(b_bgd))
 
-    elif len(r_xyz) == 3:
+    elif isinstance(r_xyz, (list, np.ndarray)) and len(r_xyz) == 3:
         r_xyz = np.tile(r_xyz, (len(b_bgd), 1))
 
-    # Perpendicular
-    r_perp_y = np.cross(b_hat, r_xyz, axis=1)
-    r_perp_y /= np.linalg.norm(r_perp_y, axis=1, keepdims=True)
-    r_perp_x = np.cross(r_perp_y, b_bgd, axis=1)
-    r_perp_x /= np.linalg.norm(r_perp_x, axis=1, keepdims=True)
+    if b_bgd.ndim == 2 and b_bgd.shape[1] == 3:
+        # Normalize background magnetic field
+        b_hat = b_bgd / np.linalg.norm(b_bgd, axis=1, keepdims=True)
+
+        # Perpendicular
+        r_perp_y = np.cross(b_hat, r_xyz, axis=1)
+        r_perp_y /= np.linalg.norm(r_perp_y, axis=1, keepdims=True)
+        r_perp_x = np.cross(r_perp_y, b_bgd, axis=1)
+        r_perp_x /= np.linalg.norm(r_perp_x, axis=1, keepdims=True)
+        r_para = b_hat
+    elif b_bgd.ndim == 3 and b_bgd.shape[1] == 3 and b_bgd.shape[2] == 3:
+        r_perp_x = ts_vec_xyz(b_bgd.time.data, b_bgd.data[:, 0])
+        r_perp_y = ts_vec_xyz(b_bgd.time.data, b_bgd.data[:, 1])
+        r_para = ts_vec_xyz(b_bgd.time.data, b_bgd.data[:, 2])
+    else:
+        raise TypeError("b_bgd must be a vector or a tensor time series")
 
     if inp_data.ndim == 2 and inp_data.shape[1] == 3:
-        out_data = np.zeros(inp.shape)
+        out_data = np.zeros(inp.shape, dtype=inp_data.dtype)
 
         out_data[:, 0] = np.sum(r_perp_x * inp_data, axis=1)
         out_data[:, 1] = np.sum(r_perp_y * inp_data, axis=1)
-        out_data[:, 2] = np.sum(b_hat * inp_data, axis=1)
+        out_data[:, 2] = np.sum(r_para * inp_data, axis=1)
 
         # To xarray
         out = ts_vec_xyz(time, out_data, attrs=inp.attrs)
 
     elif inp_data.ndim == 1:
         out_data = np.zeros([inp_data.shape[0], 2])
 
         out_data[:, 0] = inp * np.sum(r_perp_x * r_xyz, axis=1)
-        out_data[:, 1] = inp * np.sum(b_hat * r_xyz, axis=1)
+        out_data[:, 1] = inp * np.sum(r_para * r_xyz, axis=1)
 
         out = xr.DataArray(
             out_data, coords=[time, ["perp", "para"]], dims=["time", "comp"]
         )
     else:
         raise TypeError("inp must be a vector or scalar")
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/corr_deriv.py` & `pyrfu-2.4.6/pyrfu/pyrf/corr_deriv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/cotrans.py` & `pyrfu-2.4.6/pyrfu/pyrf/cotrans.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 # Local imports
 from ..models import igrf
+from .ts_tensor_xyz import ts_tensor_xyz
 from .ts_vec_xyz import ts_vec_xyz
+from .unix2datetime64 import unix2datetime64
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
@@ -45,17 +47,16 @@
     dipole_direction_geo_ = np.stack(
         [
             cos_phi * np.cos(np.deg2rad(lambda_)),
             cos_phi * np.sin(np.deg2rad(lambda_)),
             np.sin(np.deg2rad(phi)),
         ],
     ).T
-
     dipole_direction_gse_ = cotrans(
-        np.hstack([time[:, None], dipole_direction_geo_]),
+        ts_vec_xyz(unix2datetime64(time), dipole_direction_geo_),
         "geo>gse",
     )
 
     return dipole_direction_gse_
 
 
 def _transformation_matrix(t, tind, hapgood, *args):
@@ -63,14 +64,16 @@
 
     transf_mat_out = np.zeros((len(t), 3, 3))
     transf_mat_out[:, 0, 0] = np.ones(len(t))
     transf_mat_out[:, 1, 1] = np.ones(len(t))
     transf_mat_out[:, 2, 2] = np.ones(len(t))
 
     for j, t_num in enumerate(tind[::-1]):
+        assert abs(t_num) in list(range(1, 6)), "t_num must be +/- 1, 2, 3, 4, 5"
+
         if t_num in [-1, 1]:
             if hapgood:
                 theta = 100.461 + 36000.770 * t_zero + 15.04107 * ut
 
             else:
                 # Source: United States Naval Observatory, Astronomical
                 # Applications Dept. http: // aa.usno.navy.mil / faq / docs
@@ -112,42 +115,39 @@
 
             transf_mat = np.matmul(_triang(l_sun, 2), _triang(eps, 0))
             if t_num == -2:
                 transf_mat = np.transpose(transf_mat, [0, 2, 1])
 
         elif t_num in [-3, 3]:
             dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
-            y_e = dipole_direction_gse_[:, 2]  # 1st col is time
-            z_e = dipole_direction_gse_[:, 3]
+            y_e = dipole_direction_gse_[:, 1]  # 1st col is time
+            z_e = dipole_direction_gse_[:, 2]
             psi = np.rad2deg(np.arctan(y_e / z_e))
 
             transf_mat = _triang(-psi * np.sign(t_num), 0)  # inverse if -3
 
         elif t_num in [-4, 4]:
             dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
 
             mu = np.arctan(
-                dipole_direction_gse_[:, 1]
-                / np.sqrt(np.sum(dipole_direction_gse_[:, 2:] ** 2, axis=1)),
+                dipole_direction_gse_[:, 0]
+                / np.sqrt(np.sum(dipole_direction_gse_[:, 1:] ** 2, axis=1)),
             )
             mu = np.rad2deg(mu)
 
             transf_mat = _triang(-mu * np.sign(t_num), 1)
 
-        elif t_num in [-5, 5]:
+        else:
             lambda_, phi = igrf(t, "dipole")
 
             transf_mat = np.matmul(_triang(phi - 90, 1), _triang(lambda_, 2))
             if t_num == -5:
                 transf_mat = np.transpose(transf_mat, [0, 2, 1])
 
-        else:
-            raise ValueError
-
-        if j == len(tind):
+        if j == 0:
             transf_mat_out = transf_mat
         else:
             transf_mat_out = np.matmul(transf_mat, transf_mat_out)
 
     return transf_mat_out
 
 
@@ -201,61 +201,54 @@
     References
     ----------
     .. [1]  Hapgood 1997 (corrected version of Hapgood 1992) Planet.Space Sci..Vol.
             40, No. 5. pp. 71l - 717, 1992
 
     """
 
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+    assert inp.ndim < 3, "inp must be scalar or vector"
+
     if ">" in flag:
         ref_syst_in, ref_syst_out = flag.split(">")
     else:
         ref_syst_in, ref_syst_out = [None, flag.lower()]
 
-    if isinstance(inp, xr.DataArray):
-        if "COORDINATE_SYSTEM" in inp.attrs:
-            ref_syst_internal = inp.attrs["COORDINATE_SYSTEM"].lower()
-            ref_syst_internal = ref_syst_internal.split(">")[0]
-        else:
-            ref_syst_internal = None
-
-        if ref_syst_in is not None and ref_syst_internal is not None:
-            message = "input ref. frame in variable and input flag differs"
-            assert ref_syst_internal == ref_syst_in, message
-        elif ref_syst_in is None and ref_syst_internal is not None:
-            ref_syst_in = ref_syst_internal.lower()
-        elif ref_syst_in is None and ref_syst_internal is None:
-            raise ValueError("input reference frame undefined")
+    if "COORDINATE_SYSTEM" in inp.attrs:
+        ref_syst_internal = inp.attrs["COORDINATE_SYSTEM"].lower()
+        ref_syst_internal = ref_syst_internal.split(">")[0]
+    else:
+        ref_syst_internal = None
 
+    if ref_syst_in is not None and ref_syst_internal is not None:
+        message = "input ref. frame in variable and input flag differs"
+        assert ref_syst_internal == ref_syst_in, message
+        flag = f"{ref_syst_in}>{ref_syst_out}"
+    elif ref_syst_in is None and ref_syst_internal is not None:
+        ref_syst_in = ref_syst_internal.lower()
         flag = f"{ref_syst_in}>{ref_syst_out}"
+    elif flag.lower() == "dipoledirectiongse":
+        flag = flag.lower()
+    elif ref_syst_in is None and ref_syst_internal is None:
+        raise ValueError(f"Transformation {flag} is unknown!")
 
     if ref_syst_in == ref_syst_out:
         return inp
 
     # J2000 reference time
     j2000 = 946727930.8160001
     # j2000 = Time("J2000", format="jyear_str").unix
 
-    if isinstance(inp, xr.DataArray):
-        time = inp.time.data
-        t = time.astype(int) * 1e-9
-
-        #  Terrestial Time (seconds since J2000)
-        tts = t - j2000
-        inp_ts = inp
-        inp = inp.data
-
-    elif isinstance(inp, np.ndarray):
-        time = (inp[:, 0] * 1e9).astype("datetime64[ns]")
-        t = inp[:, 0]
-        #  Terrestial Time (seconds since J2000)
-        tts = t - j2000
-        inp_ts = None
-        inp = inp[:, 1:]
-    else:
-        raise TypeError("invalid input")
+    time = inp.time.data
+    t = (time.astype(np.int64) * 1e-9).astype(np.float64)
+
+    #  Terrestial Time (seconds since J2000)
+    tts = t - j2000
+    inp_ts = inp
+    inp = inp.data
 
     if hapgood:
         day_start_epoch = time.astype("datetime64[D]")
         day_start_epoch = day_start_epoch.astype("datetime64[ns]")
         day_start_epoch = day_start_epoch.astype(np.int64) / 1e9
         mjd_ref_epoch = np.datetime64("2000-01-01T12:00:00", "ns")
         mjd_ref_epoch = mjd_ref_epoch.astype(np.int64) / 1e9
@@ -298,33 +291,22 @@
         file_name = "transformation_indices.json"
 
         with open(os.sep.join([root_path, file_name]), "r", encoding="utf-8") as file:
             transformation_dict = json.load(file)
 
         tind = transformation_dict[flag]
 
-    elif flag == "dipoledirectiongse":
-        out_data = _dipole_direction_gse(t)
-        return ts_vec_xyz(inp.time.data, out_data)
+        transf_mat = _transformation_matrix(t, tind, hapgood, *args_trans_mat)
 
-    else:
-        raise ValueError(f"Transformation {flag} is unknown!")
+        if inp.ndim == 1:
+            out = ts_tensor_xyz(inp_ts.time.data, transf_mat)
 
-    transf_mat = _transformation_matrix(t, tind, hapgood, *args_trans_mat)
-
-    if inp.ndim == 2:
-        out = np.einsum("kji,ki->kj", transf_mat, inp)
-    elif inp.ndim == 1:
-        out = transf_mat
-    else:
-        raise ValueError
-
-    if inp_ts is not None:
-        out_data = out
-        out = inp_ts.copy()
-        out.data = out_data
-        out.attrs["COORDINATE_SYSTEM"] = ref_syst_out.upper()
+        else:
+            out_data = np.einsum("kji,ki->kj", transf_mat, inp)
+            out = inp_ts.copy()
+            out.data = out_data
+            out.attrs["COORDINATE_SYSTEM"] = ref_syst_out.upper()
 
     else:
-        out = np.hstack([t[:, None], out])
+        out = _dipole_direction_gse(t)
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/cross.py` & `pyrfu-2.4.6/pyrfu/pyrf/cross.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/date_str.py` & `pyrfu-2.4.6/pyrfu/pyrf/date_str.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/datetime2iso8601.py` & `pyrfu-2.4.6/pyrfu/pyrf/datetime2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/datetime642iso8601.py` & `pyrfu-2.4.6/pyrfu/pyrf/iso86012unix.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,27 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def datetime642iso8601(time):
-    r"""Convert datetime64 in ns units to ISO 8601 time format .
+def iso86012unix(time):
+    r"""Converts time in iso format to unix
 
     Parameters
     ----------
-    time : ndarray
-        Time in datetime64 in ns units.
+    time : str or array_like of str
+        Time.
 
     Returns
     -------
-    time_iso8601 : ndarray
-        Time in ISO 8601 format.
-
-    See Also
-    --------
-    pyrfu.pyrf.datetime642iso8601
+    out : float or list of float
+        Time in unix format.
 
     """
 
-    # Convert to required precision
-    time_datetime64 = time.astype("<M8[ns]")
+    assert isinstance(time, (str, list, np.ndarray)), "time must be a str or array_like"
 
-    # Convert to string
-    time_iso8601 = time_datetime64.astype(str)
-    time_iso8601 = np.atleast_1d(np.squeeze(np.stack([time_iso8601])))
+    out = np.atleast_1d(time).astype("datetime64[ns]")
 
-    return time_iso8601
+    return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/datetime642ttns.py` & `pyrfu-2.4.6/pyrfu/pyrf/datetime642ttns.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/datetime642unix.py` & `pyrfu-2.4.6/pyrfu/pyrf/datetime642iso8601.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+# 3rd party imports
+import numpy as np
+
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def datetime642unix(time):
-    r"""Converts datetime64 in ns units to unix time.
+def datetime642iso8601(time):
+    r"""Convert datetime64 in ns units to ISO 8601 time format .
 
     Parameters
     ----------
     time : ndarray
-        Time in datetime64 format.
+        Time in datetime64 in ns units.
 
     Returns
     -------
-    time_unix : ndarray
-        Time in unix format.
+    time_iso8601 : ndarray
+        Time in ISO 8601 format.
 
     See Also
     --------
-    pyrfu.pyrf.unix2datetime64
+    pyrfu.pyrf.datetime642iso8601
 
     """
 
-    # Make sure that time is in ns format
-    time_ns = time.astype("<M8[ns]")
-
-    # Convert to unix
-    time_unix = time_ns.astype("int64") / 1e9
+    if isinstance(time, np.datetime64):
+        time = np.array([time])
+        time_datetime64 = time.astype("datetime64[ns]")
+    elif isinstance(time, (list, np.ndarray)) and isinstance(time[0], np.datetime64):
+        time_datetime64 = time.astype("datetime64[ns]")
+    else:
+        raise TypeError("time must be numpy.datetime64 or array_like")
+
+    # Convert to string
+    time_iso8601 = time_datetime64.astype(str)
+    time_iso8601 = np.atleast_1d(np.squeeze(np.stack([time_iso8601])))
 
-    return time_unix
+    return time_iso8601
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/dist_append.py` & `pyrfu-2.4.6/pyrfu/pyrf/dist_append.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
 from .ts_skymap import ts_skymap
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
@@ -32,29 +33,35 @@
 
     Notes
     -----
     The time series have to be in the correct time order.
 
     """
 
+    # Check input type
+    assert isinstance(inp1, xr.Dataset), "inp1 must be a xarray.Dataset"
+
     if inp0 is None:
         return inp1
 
+    assert isinstance(inp0, xr.Dataset), "inp0 must be a xarray.Dataset"
+
     # Global attributes
     glob_attrs = inp0.attrs
 
     # Stack coordinates
     # time
     time = np.hstack([inp0.time.data, inp1.time.data])
 
     # Azimuthal angle
-    if inp0.phi.ndim == 2:
-        phi = np.vstack([inp0.phi.data, inp1.phi.data])
-    else:
-        phi = inp0.phi.data
+    # if inp0.phi.ndim == 2:
+    #    phi = np.vstack([inp0.phi.data, inp1.phi.data])
+    # else:
+    #    phi = inp0.phi.data
+    phi = np.vstack([inp0.phi.data, inp1.phi.data])
 
     # Elevation angle
     theta = inp0.theta.data
 
     # Coordinates attributes
     coords_attrs = {k: inp0[k].attrs for k in ["time", "energy", "phi", "theta"]}
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/dot.py` & `pyrfu-2.4.6/pyrfu/pyrf/dot.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/dynamic_press.py` & `pyrfu-2.4.6/pyrfu/pyrf/dynamic_press.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def dynamic_press(n_s, v_xyz, specie: str = "i"):
+def dynamic_press(n_s, v_xyz, specie: str = "ions"):
     r"""Computes dynamic pressure.
 
     Parameters
     ----------
     n_s : xarray.DataArray
         Time series of the number density of the specie.
     v_xyz : xarray.DataArray
         Time series of the bulk velocity of the specie.
-    specie : {"i", "e"}, Optional
-        Specie. default "i".
+    specie : {"ions", "electrons"}, Optional
+        Specie. Default "ions".
 
     Returns
     -------
     p_dyn : xarray.DataArray
         Time series of the dynamic pressure of the specie.
 
     Examples
@@ -40,31 +41,39 @@
 
     Spacecraft index
 
     >>> mms_id = 1
 
     Load ion bulk velocity and remove spintone
 
-    >>> v_xyz_i = mms.get_data("Vi_gse_fpi_fast_l2", tint, mms_id)
-    >>> st_xyz_i = mms.get_data("STi_gse_fpi_fast_l2", tint, mms_id)
+    >>> v_xyz_i = mms.get_data("vi_gse_fpi_fast_l2", tint, mms_id)
+    >>> st_xyz_i = mms.get_data("sti_gse_fpi_fast_l2", tint, mms_id)
     >>> v_xyz_i = v_xyz_i - st_xyz_i
 
     Ion number density
 
-    >>> n_i = mms.get_data("Ni_fpi_fast_l2", tint, mms_id)
+    >>> n_i = mms.get_data("ni_fpi_fast_l2", tint, mms_id)
 
     Compute dynamic pressure
 
-    >>> p = pyrf.dynamic_press(n_i, v_xyz_i, specie="i")
+    >>> p = pyrf.dynamic_press(n_i, v_xyz_i, specie="ions")
 
     """
 
-    if specie == "i":
+    # Check input
+    assert isinstance(n_s, xr.DataArray), "n_s must be a xarray.DataArray"
+    assert isinstance(v_xyz, xr.DataArray), "v_xyz must be a xarray.DataArray"
+    assert isinstance(specie, str), "specie must be a str"
+    assert specie.lower() in ["ions", "electrons"], "specie must be ions or electrons"
+
+    # Check n_s and v_xyz shapes
+    assert n_s.ndim == 1, "n_s must be a scalar"
+    assert v_xyz.ndim == 2 and v_xyz.shape[1] == 3, "v_xyz must be a vector"
+
+    if specie.lower() == "ions":
         mass = constants.proton_mass
-    elif specie == "e":
-        mass = constants.electron_mass
     else:
-        raise ValueError("Unknown specie")
+        mass = constants.electron_mass
 
-    p_dyn = n_s * mass * np.linalg.norm(v_xyz, axis=0) ** 2
+    p_dyn = n_s * mass * np.linalg.norm(v_xyz, axis=1) ** 2
 
     return p_dyn
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/e_vxb.py` & `pyrfu-2.4.6/pyrfu/pyrf/e_vxb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
 from .resample import resample
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
@@ -46,44 +47,41 @@
 
     Spacecraft index
 
     >>> mms_id = 1
 
     Load magnetic field and electric field
 
-    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_fast_l2", tint, mms_id)
+    >>> b_xyz = mms.get_data("b_gse_fgm_srvy_l2", tint, mms_id)
+    >>> e_xyz = mms.get_data("e_gse_edp_fast_l2", tint, mms_id)
 
     Compute ExB drift velocity
 
     >>> v_xyz_exb = pyrf.e_vxb(e_xyz, b_xyz,"ExB")
 
     """
 
-    input_v_cons = v_xyz.size == 3
-    estimate_exb = flag.lower() == "exb"
+    assert isinstance(flag, str) and flag.lower() in ["exb", "vxb"], "Invalid flag"
+    assert isinstance(b_xyz, xr.DataArray), "b_xyz must be a xarray.DataArray"
 
-    if estimate_exb:
+    if isinstance(v_xyz, (list, np.ndarray)) and v_xyz.ndim == 1 and len(v_xyz) == 3:
+        v_xyz = ts_vec_xyz(b_xyz.time.data, np.tile(v_xyz, (len(b_xyz), 1)))
+    elif isinstance(v_xyz, xr.DataArray):
         b_xyz = resample(b_xyz, v_xyz)
+    else:
+        raise TypeError("v_xyz must be xarray.DataArray or array_like constant vector")
 
+    if flag.lower() == "exb":
         res = 1e3 * np.cross(v_xyz.data, b_xyz.data, axis=1)
         res /= np.linalg.norm(b_xyz.data, axis=1)[:, None] ** 2
 
         attrs = {"UNITS": "km/s", "FIELDNAM": "Velocity", "LABLAXIS": "V"}
 
     else:
-        if input_v_cons:
-            res = np.cross(np.tile(v_xyz, (len(b_xyz), 1)), b_xyz.data)
-            res *= (-1) * 1e-3
-
-        else:
-            b_xyz = resample(b_xyz, v_xyz)
-
-            res = np.cross(v_xyz.data, b_xyz.data)
-            res *= (-1) * 1e-3
+        res = -1e-3 * np.cross(v_xyz.data, b_xyz.data)
 
         attrs = {
             "UNITS": "mV/s",
             "FIELDNAM": "Electric field",
             "LABLAXIS": "E",
         }
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ebsp.py` & `pyrfu-2.4.6/pyrfu/pyrf/ebsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import numpy as np
 import xarray as xr
 from scipy import fft
 
 from .calc_fs import calc_fs
 from .cart2sph import cart2sph
 from .convert_fac import convert_fac
-from .datetime642iso8601 import datetime642iso8601
-from .iso2unix import iso2unix
 from .resample import resample
 
 # Local imports
 from .ts_time import ts_time
 from .ts_vec_xyz import ts_vec_xyz
 from .unix2datetime64 import unix2datetime64
 
@@ -64,26 +62,26 @@
             logging.info("Interpolating b to e")
         elif fs_e == fs_b and len(e_xyz) == len(db_xyz):
             fs_ = fs_e
         else:
             fs_ = 2 * fs_e
             start_time = np.max(
                 [
-                    e_xyz.time.data[0].astype(int) / 1e9,
-                    db_xyz.time.data[0].astype(int) / 1e9,
+                    e_xyz.time.data[0].astype(np.float64) / 1e9,
+                    db_xyz.time.data[0].astype(np.float64) / 1e9,
                 ]
             )
             end_time = np.min(
                 [
-                    e_xyz.time.data[-1].astype(int) / 1e9,
-                    db_xyz.time.data[-1].astype(int) / 1e9,
+                    e_xyz.time.data[-1].astype(np.float64) / 1e9,
+                    db_xyz.time.data[-1].astype(np.float64) / 1e9,
                 ]
             )
 
-            nt = int((end_time - start_time) * fs_)
+            nt = np.floor((end_time - start_time) * fs_).astype(np.int64)
 
             t = np.linspace(start_time, end_time, nt)
 
             t = ts_time(t)
 
             e_xyz = resample(e_xyz, t)
             b_bgd = resample(b_bgd, t)
@@ -93,80 +91,61 @@
             logging.info("Interpolating b and e to 2x e sampling")
 
     return e_xyz, db_xyz, b_xyz, b_bgd, fs_
 
 
 def _b_elevation(b_x, b_y, b_z, angle_b_elevation_max):
     # Remove the last sample if the total number of samples is odd
-    b_x = b_x[: int(2 * (len(b_x) // 2)), :]
-    b_y = b_y[: int(2 * (len(b_y) // 2)), :]
-    b_z = b_z[: int(2 * (len(b_z) // 2)), :]
+    b_x = b_x[: int(2 * (len(b_x) // 2))]
+    b_y = b_y[: int(2 * (len(b_y) // 2))]
+    b_z = b_z[: int(2 * (len(b_z) // 2))]
 
     angle_b_elevation = np.arctan(b_z / np.sqrt(b_x**2 + b_y**2))
     angle_b_elevation = np.rad2deg(angle_b_elevation)
     idx_b_par_spin_plane = np.abs(angle_b_elevation) < angle_b_elevation_max
 
     return angle_b_elevation, idx_b_par_spin_plane
 
 
 def _freq_int(freq_int, delta_b):
-    start_time = delta_b.time.data[0].astype(int) / 1e9
-    end_time = delta_b.time.data[-1].astype(int) / 1e9
+    start_time = delta_b.time.data[0].astype(np.float64) / 1e9
+    end_time = delta_b.time.data[-1].astype(np.float64) / 1e9
 
-    pc12_range, pc35_range, other_range = [False, False, False]
+    pc12_range, other_range = [False, False]
 
     if isinstance(freq_int, str):
-        if freq_int.lower() == "pc12":
-            pc12_range = True
-
-            freq_int = [0.1, 5]
-
-            delta_t = 1  # local
-
-            tint = np.round([start_time, end_time])
-            tint = list(datetime642iso8601(unix2datetime64(tint)))
-
-        elif freq_int.lower() == "pc35":
-            pc35_range = True
-
+        if freq_int.lower() == "pc35":
             freq_int = [0.002, 0.1]
 
             delta_t = 60  # local
-
-            tint = 60 * np.array([np.round(start_time / 60), np.round(end_time / 60)])
-            tint = datetime642iso8601(unix2datetime64(tint))
-
         else:
-            raise ValueError("Invalid format of interval")
+            pc12_range = True
 
-        fs_out = 1 / delta_t
+            freq_int = [0.1, 5.0]
 
-        nt = np.round((iso2unix(tint[1]) - iso2unix(tint[0])) / delta_t)
-        nt = nt.astype(int)  # local
+            delta_t = 1  # local
 
-        out_time = np.linspace(iso2unix(tint[0]), iso2unix(tint[1]), nt)
-        out_time += delta_t / 2
-        out_time = out_time[:-1]
+        fs_out = 1 / delta_t
     else:
         if freq_int[1] >= freq_int[0]:
             other_range = True
 
             fs_out = freq_int[1] / 5
 
             delta_t = 1 / fs_out  # local
-
-            nt = np.round((end_time - start_time) / delta_t).astype(int)
-
-            out_time = np.linspace(start_time, end_time, nt)
-            out_time += delta_t / 2
-            out_time = out_time[:-1]
         else:
             raise ValueError("FREQ_INT must be [f_min f_max], f_min<f_max")
 
-    any_range = [pc12_range, pc35_range, other_range]
+    nt = np.floor((end_time - start_time) / delta_t).astype(np.int64)
+
+    out_time = np.linspace(start_time, end_time, nt, dtype=np.float64)
+    out_time += delta_t / 2.0
+    out_time = out_time[:-1]
+
+    any_range = [pc12_range, other_range]
 
     return any_range, freq_int, fs_out, out_time
 
 
 @numba.jit(cache=True, nogil=True, parallel=True, nopython=True, fastmath=True)
 def _average_data(data=None, x=None, y=None, av_window=None):
     # average data with time x to time y using window
@@ -296,21 +275,21 @@
             * k : xarray.DataArray
                 k-vector (theta, phi FAC) [angles in degrees].
 
     Other Parameters
     ----------------
     polarization : bool
         Computes polarization parameters. Default False.
-    noresamp : bool
+    no_resample : bool
         No resampling, E and delta_b are given at the same time line.
         Default False.
     fac : bool
         Uses FAC coordinate system (defined by b0 and optionally xyz),
         otherwise no coordinate system transformation is performed. Default
-        False.
+        True.
     de_dot_b0 : bool
         Computes dEz from delta_b dot B = 0, uses full_b. Default False.
     full_b_db : bool
         delta_b contains DC field. Default False.
     nav : int
         Number of wave periods to average Default 8.
     fac_matrix : numpy.ndarray
@@ -358,15 +337,22 @@
     >>>                          freq_int=[10, 4000], **options)
 
     """
 
     assert isinstance(db_xyz, xr.DataArray), "delta_b must be a DataArray"
     assert isinstance(b_xyz, xr.DataArray), "full_b must be a DataArray"
     assert isinstance(b_bgd, xr.DataArray), "b0 must be a DataArray"
-    assert isinstance(xyz, xr.DataArray), "xyz must be a DataArray"
+
+    message = "freq_int must be a string or array_like"
+    assert isinstance(freq_int, (list, np.ndarray, str)), message
+
+    if isinstance(freq_int, (list, np.ndarray)):
+        assert len(freq_int) == 2, "freq_int list must contain two elements"
+    else:
+        assert freq_int in ["pc12", "pc35"], "string freq_int must be pc12 or pc35"
 
     # Compute magnetic field fluctuations sampling frequency
     fs_b = calc_fs(db_xyz)
 
     # Below which we cannot apply E*B=0
     angle_b_elevation_max = 15.0
 
@@ -390,51 +376,47 @@
         "b0": b_bgd,
         "r": xyz,
     }
 
     want_polarization = kwargs.get("polarization", False)
 
     flag_no_resample = kwargs.get("no_resample", False)
-    flag_want_fac = kwargs.get("fac", False)
+    flag_want_fac = kwargs.get("fac", True)
     flag_de_dot_b0 = kwargs.get("de_dot_b0", False)
     flag_full_b_db = kwargs.get("full_b_db", False)
 
     m_width_coeff = kwargs.get("m_width_coeff", 1.0)
 
     # Number of wave periods to average
     n_wave_period_to_average = kwargs.get("nav", 8)
 
     # matrix for rotation to FAC
     fac_matrix = kwargs.get("fac_matrix", None)
 
     if flag_want_fac and fac_matrix is None:
-        if b_bgd is None:
-            raise ValueError("ebsp(): at least b0 should be given for option FAC")
-
         if xyz is None:
             logging.info(
                 "convert_fac : assuming s/c position [1 0 0] for estimating FAC"
             )
             xyz = [1, 0, 0]
             xyz = ts_vec_xyz(db_xyz.time.data, np.tile(xyz, (len(db_xyz), 1)))
+        else:
+            assert isinstance(xyz, xr.DataArray), "xyz must be a DataArray"
 
         xyz = resample(xyz, db_xyz, **{"f_s": fs_b})
 
     b_bgd = resample(b_bgd, db_xyz, **{"f_s": fs_b})
 
     if flag_full_b_db:
         b_xyz = db_xyz
         res["full_b"] = b_xyz
         db_xyz = db_xyz - b_bgd
 
-    if flag_de_dot_b0 and b_xyz is None:
-        raise ValueError("full_b must be given for option de_dot_b0=0")
-
     any_range, freq_int, out_sampling, out_time = _freq_int(freq_int, db_xyz)
-    pc12_range, pc35_range, other_range = any_range
+    pc12_range, other_range = any_range
 
     if want_ee:
         # Check the sampling rate
         temp_ = _checksampling(e_xyz, db_xyz, b_xyz, b_bgd, flag_no_resample)
         e_xyz, db_xyz, b_xyz, b_bgd, in_sampling = temp_
 
     else:
@@ -442,33 +424,31 @@
 
         e_xyz = None
 
     if in_sampling / 2 < freq_int[1]:
         raise ValueError("F_MAX must be lower than the Nyquist frequency")
 
     if want_ee and e_xyz.shape[1] < 3 and not flag_de_dot_b0:
-        raise ValueError(
+        raise TypeError(
             "E must have all 3 components or flag de_dot_db=0 must be given"
         )
 
     if len(db_xyz) % 2:
         db_xyz = db_xyz[:-1, :]
         b_bgd = b_bgd[:-1, :]
 
         if fac_matrix is None:
             xyz = xyz[:-1, :]
         else:
-            fac_matrix["t"] = fac_matrix["t"][:-1, :]
-
-            fac_matrix["rotMatrix"] = fac_matrix["rotMatrix"][:-1, :, :]
+            fac_matrix = fac_matrix[:-1, ...]
 
         if want_ee:
             e_xyz = e_xyz[:-1, :]
 
-    in_time = db_xyz.time.data.astype("int64") / 1e9
+    in_time = db_xyz.time.data.astype(np.float64) / 1e9
 
     b_x, b_y, b_z = [None, None, None]
 
     idx_b_par_spin_plane = None
 
     if flag_de_dot_b0:
         b_x, b_y, b_z = [b_xyz[:, i].data for i in range(3)]
@@ -483,42 +463,39 @@
     # Otherwise we compute Ez within the main loop and do the transformation
     # to FAC there.
 
     time_b0 = 0
     if flag_want_fac:
         res["flagFac"] = True
 
-        time_b0 = b_bgd.time.data.astype("int64") / 1e9
+        time_b0 = b_bgd.time.data.astype(np.float64) / 1e9
 
         if want_ee and not flag_de_dot_b0:
             eisr2 = e_xyz[:, :2]
             idx_nan_e = np.isnan(e_xyz.data)
             idx_nan_eisr2 = np.isnan(eisr2.data)
 
-            if e_xyz.shape[1] < 3:
-                raise TypeError("E must be a 3D vector to be rotated to FAC")
-
             if fac_matrix is None:
                 e_xyz = convert_fac(e_xyz, b_bgd, xyz)
             else:
                 e_xyz = convert_fac(e_xyz, fac_matrix)
 
         else:
-            idx_nan_e = None
+            idx_nan_e = np.full((len(in_time), 3), False)
             eisr2 = None
-            idx_nan_eisr2 = None
+            idx_nan_eisr2 = np.full((len(in_time), 2), False)
 
         if fac_matrix is None:
             db_xyz = convert_fac(db_xyz, b_bgd, xyz)
         else:
             db_xyz = convert_fac(db_xyz, fac_matrix)
     else:
-        idx_nan_e = None
+        idx_nan_e = np.full((len(in_time), 3), False)
         eisr2 = None
-        idx_nan_eisr2 = None
+        idx_nan_eisr2 = np.full((len(in_time), 2), False)
 
     # Find the frequencies for an FFT of all data and set important parameters
     nd2 = len(in_time) / 2
 
     freq = in_sampling * np.arange(nd2) / nd2 * 0.5
 
     # The frequencies corresponding to FFT
@@ -652,23 +629,25 @@
                     -(we_re[:, 0] * b_x + we_re[:, 1] * b_y) / b_z
                     - 1j * (we_im[:, 0] * b_x + we_im[:, 1] * b_y) / b_z
                 )
                 we_z[idx_b_par_spin_plane] = np.nan
 
                 if flag_want_fac:
                     if fac_matrix is None:
-                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
+                        tmp = np.vstack([np.transpose(we[:, :2]), np.transpose(we_z)])
+                        arg_ = ts_vec_xyz(time_b0, np.transpose(tmp))
                         we = convert_fac(arg_, b_bgd, xyz)
                     else:
-                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
+                        tmp = np.vstack([np.transpose(we[:, :2]), np.transpose(we_z)])
+                        arg_ = ts_vec_xyz(time_b0, np.transpose(tmp))
                         we = convert_fac(arg_, fac_matrix)
-
-                    we = we[:, 1:]
                 else:
-                    we = np.hstack([we[:, :2], we_z])
+                    we = np.transpose(
+                        np.vstack([np.transpose(we[:, :2]), np.transpose(we_z)])
+                    )
 
             power_e = 2 * np.pi * (we * np.conj(we)) / new_freq_mat
             power_e = np.vstack([power_e.T, np.sum(power_e, axis=1)]).T
 
             power_ex_plot[:, ind_a] = power_e[:, 0]
             power_ey_plot[:, ind_a] = power_e[:, 1]
             power_ez_plot[:, ind_a] = power_e[:, 2]
@@ -751,15 +730,16 @@
             censure_idx = np.hstack(
                 [
                     np.arange(np.min([censure[ind_a], len(out_time)])),
                     np.arange(
                         np.max([0, len(out_time) - censure[ind_a] - 1]), len(out_time)
                     ),
                 ]
-            ).astype(int)
+            )
+            censure_idx = censure_idx.astype(np.int64)
 
             s_mat_avg[censure_idx, ...] = np.nan
 
             # compute singular value decomposition
             # real matrix which is superposition of real part of spectral
             # matrix over imaginary part
             a_mat, u_mat = [np.zeros((6, 3, n_data_out)) for _ in range(2)]
@@ -856,15 +836,15 @@
         censure_idx = np.hstack(
             [
                 np.arange(np.min([censure[ind_a], len(in_time)])),
                 np.arange(np.max([1, len(in_time) - censure[ind_a]]), len(in_time)),
             ]
         )
 
-        censure_idx = censure_idx.astype(int)
+        censure_idx = censure_idx.astype(np.int64)
 
         power_bx_plot[censure_idx, ind_a] = np.nan
         power_by_plot[censure_idx, ind_a] = np.nan
         power_bz_plot[censure_idx, ind_a] = np.nan
         power_2b_plot[censure_idx, ind_a] = np.nan
 
         if want_ee:
@@ -884,18 +864,16 @@
     idx_nan_b = np.sum(idx_nan_b, axis=1) > 0
     idx_nan_eisr2 = np.sum(idx_nan_eisr2, axis=1) > 0
 
     n_power_b = len(power_2b_plot)
 
     if pc12_range or other_range:
         censure3 = np.floor(1.8 * a_)
-    elif pc35_range:
-        censure3 = np.floor(0.4 * a_)
     else:
-        raise ValueError("Invalid range")
+        censure3 = np.floor(0.4 * a_)
 
     # Censure magnetic fied
     power_bx_plot = _censure_plot(power_bx_plot, idx_nan_b, censure3, n_power_b, a_)
     power_by_plot = _censure_plot(power_by_plot, idx_nan_b, censure3, n_power_b, a_)
     power_bz_plot = _censure_plot(power_bz_plot, idx_nan_b, censure3, n_power_b, a_)
     power_2b_plot = _censure_plot(power_2b_plot, idx_nan_b, censure3, n_power_b, a_)
 
@@ -961,25 +939,25 @@
             power_ex_plot, power_ey_plot, power_ez_plot, power_2e_plot
         )
 
         poynting_xyz = np.tile(s_plot_x, (3, 1, 1))
         poynting_xyz = np.transpose(poynting_xyz, [1, 2, 0])
         poynting_xyz[:, :, 1] = s_plot_y
         poynting_xyz[:, :, 2] = s_plot_z
-        poynting_xyz = poynting_xyz.astype(float)
+        poynting_xyz = poynting_xyz.astype(np.float64)
 
         poynting_r_th_ph = np.tile(s_r, (3, 1, 1))
         poynting_r_th_ph = np.transpose(poynting_r_th_ph, [1, 2, 0])
         poynting_r_th_ph[..., 1] = np.pi / 2 - s_elevation
         poynting_r_th_ph[..., 2] = s_azimuth
         poynting_r_th_ph[..., 1:] = poynting_r_th_ph[..., 1:] * 180 / np.pi
-        poynting_r_th_ph = poynting_r_th_ph.astype(float)
+        poynting_r_th_ph = poynting_r_th_ph.astype(np.float64)
 
         # Output
-        res["ee_ss"] = power_2e_isr2_plot.astype(float)
+        res["ee_ss"] = power_2e_isr2_plot.astype(np.float64)
 
         res["ee_xxyyzzss"] = xr.DataArray(
             ee_xxyyzzss[:, ::-1, ...],
             coords=[res["t"], res["f"], ["xx", "yy", "zz", "ss"]],
             dims=["time", "frequency", "comp"],
         )
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/edb.py` & `pyrfu-2.4.6/pyrfu/pyrf/edb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
 from .resample import resample
 from .ts_scalar import ts_scalar
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
@@ -75,14 +76,18 @@
 
     Compute Ez
 
     >>> e_z, alpha = pyrf.edb(e_xyz, b_xyz)
 
     """
 
+    assert isinstance(e_xyz, xr.DataArray), "e_xyz must be a xarray.DataArray"
+    assert isinstance(b_bgd, xr.DataArray), "b_bgd must be a xarray.DataArray"
+    assert isinstance(angle_lim, (int, float)), "angle_lime must be int or float"
+
     flag_method, default_value = _check_method(flag_method)
 
     # Make sure that background magnetic field sampling matches the
     # electric field sampling
     b_bgd = resample(b_bgd, e_xyz)
 
     b_data = b_bgd.data
@@ -114,17 +119,17 @@
         )
         b_angle = np.rad2deg(b_angle)
         ind = np.abs(b_angle) < angle_lim
 
         if True in ind:
             e_data[ind, 2] = np.sum(e_data[ind, :2] * b_data[ind, :2], axis=1)
             e_data[ind, 2] *= b_data[ind, 2]
-            e_data[ind, 2] /= np.linalg.norm(b_data[:, :2], axis=1) ** 2
+            e_data[ind, 2] /= np.linalg.norm(b_data[ind, :2], axis=1) ** 2
 
     b_angle = ts_scalar(e_xyz.time.data, b_angle, {"UNITS": "degrees"})
     e_data = ts_vec_xyz(
         e_xyz.time.data,
         e_data,
-        {"UNITS": e_xyz.attrs["UNITS"]},
+        e_xyz.attrs,
     )
 
     return e_data, b_angle
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/end.py` & `pyrfu-2.4.6/pyrfu/pyrf/start.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party import
 import numpy as np
+import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def end(inp):
-    """Gives the last time of the time series in unix format.
+def start(inp):
+    r"""Gives the first time of the time series.
 
     Parameters
     ----------
     inp : xarray.DataArray
-        Time series of the input variable.
+        Time series.
 
     Returns
     -------
     out : float
-        Value of the last time in unix format.
+        Value of the first time in the desired format.
 
     """
 
-    out = inp.time.data[-1].astype(np.int64) / 1e9
+    # Check input type
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+
+    # Make sure this is a time series
+    assert list(inp.dims)[0] == "time", "inp must be a time series"
+
+    out = inp.time.data[0].astype(np.int64) * 1e-9
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/estimate.py` & `pyrfu-2.4.6/pyrfu/pyrf/estimate.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
 
 def _estimate_capa_sphe(radius):
     return 4 * np.pi * constants.epsilon_0 * radius
 
 
 def _estimate_capa_wire(radius, length):
-    if not radius or radius == 0 or not length:
-        out = None
-    elif length and radius and length >= 10 * radius:
+    if length and radius != 0 and length >= 10 * radius:
         l_ = np.log(length / radius)
         out = length / l_ * (1 + 1 / l_ * (1 - np.log(2)))
         out *= 2 * np.pi * constants.epsilon_0
     else:
         raise ValueError(
             "capacitance_wire requires length at least 10 times the radius!",
         )
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/extend_tint.py` & `pyrfu-2.4.6/pyrfu/pyrf/extend_tint.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,24 @@
     Load spacecraft position
 
     >>> tints_long = pyrf.extend_tint(tint, [-100, 100])
 
     """
 
     # Set default extension
-    if tint is None:
-        tint = [-60.0, 60.0]
+    if ext is None:
+        ext = [-60.0, 60.0]
 
     # Make sure tint and ext are 2 elements array_like
     message = "must be array_like with 2 elements"
     assert isinstance(tint, (np.ndarray, list)) and len(tint) == 2, f"tint {message}"
     assert isinstance(ext, (np.ndarray, list)) and len(ext) == 2, f"ext {message}"
 
     # Convert extension to timedelta64[ns]
-    ext = np.array(ext) * 1e9
-    ext = ext.astype("timedelta64[ns]")
+    ext = (np.array(ext) * 1e9).astype("timedelta64[ns]")
 
     # Original time interval to datetime64[ns]
     if isinstance(tint[0], np.datetime64):
         tint_ori = tint
     elif isinstance(tint[0], str):
         tint_ori = iso86012datetime64(np.array(tint))
     else:
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/filt.py` & `pyrfu-2.4.6/pyrfu/pyrf/filt.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,27 +36,26 @@
                 0.5,
                 60,
             )
 
         num1, den1 = signal.ellip(order, 0.5, 60, f_min, btype="highpass")
     else:
         if order == -1:
-            order, f_max = signal.ellipord(
+            order1, f_max = signal.ellipord(
                 f_max,
                 np.min([f_max * 1.3, 0.9999]),
                 0.5,
                 60,
             )
+            order2, f_min = signal.ellipord(f_min, f_min * 0.75, 0.5, 60)
+        else:
+            order1, order2 = [order, order]
 
-        num1, den1 = signal.ellip(order, 0.5, 60, f_max)
-
-        if order == -1:
-            order, f_min = signal.ellipord(f_min, f_min * 0.75, 0.5, 60)
-
-        num2, den2 = signal.ellip(order, 0.5, 60, f_min)
+        num1, den1 = signal.ellip(order1, 0.5, 60, f_max)
+        num2, den2 = signal.ellip(order2, 0.5, 60, f_min)
 
     return num1, den1, num2, den2
 
 
 def filt(inp, f_min: float = 0.0, f_max: float = 1.0, order: int = -1):
     r"""Filters input quantity.
 
@@ -100,19 +99,25 @@
     Bandpass filter E waveform
 
     >>> e_xyzfac_hf = pyrf.filt(e_xyzfac, 4, 0, 3)
     >>> e_xyzfac_lf = pyrf.filt(e_xyzfac, 0, 4, 3)
 
     """
 
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+
     f_samp = 1 / (np.median(np.diff(inp.time)).astype(np.int64) * 1e-9)
 
     # Data of the input
     inp_data = inp.data
 
+    assert isinstance(f_min, (int, float)), "f_min must be int or float"
+    assert isinstance(f_max, (int, float)), "f_max must be int or float"
+    assert isinstance(order, (int, float)), "order must be int or float"
+
     f_min, f_max = [f_min / (f_samp / 2), f_max / (f_samp / 2)]
 
     f_max = np.min([f_max, 1.0])
 
     # Parameters of the elliptic filter. fact defines the width between
     # stopband and passband
     # r_pass, r_stop, fact = [0.5, 60, 1.1]
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/find_closest.py` & `pyrfu-2.4.6/pyrfu/pyrf/find_closest.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/get_omni_data.py` & `pyrfu-2.4.6/pyrfu/pyrf/get_omni_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     Returns
     -------
     data : xarray.Dataset
         OMNI data.
 
     """
 
-    tint = iso86012datetime64(np.array(tint)).astype("<M8[s]")
+    tint = iso86012datetime64(np.array(tint)).astype("datetime64[s]")
 
     url_ = _omni_url(tint, database)
 
     vars_ = ""
     for variable in variables:
         vars_ = f"{vars_}&vars={var_omni_2[variable]:d}"
 
@@ -172,12 +172,12 @@
     lines = out[idx_start:idx_end].split("\\n")[:-1]
     lines = [list(filter(lambda x: x != "", l_.split(" "))) for l_ in lines]
     lines = [[f"{l_[0]}-{l_[1]}/{l_[2]}", *l_[3:]] for l_ in lines[1:]]
     data = pd.DataFrame(lines, columns=["time", *variables])
     data["time"] = pd.to_datetime(data["time"], format="%Y-%j/%H")
 
     data = data.set_index("time").astype(np.float64)
-    fmt_ = f"<M8[{database[5].lower()}]"
-    data = data.loc[data.index.isin(tint.astype(fmt_).astype("<M8[ns]"))]
+    fmt_ = f"datetime64[{database[5].lower()}]"
+    data = data.loc[data.index.isin(tint.astype(fmt_).astype("datetime64[ns]"))]
     data = data.to_xarray()
 
     return data
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/gradient.py` & `pyrfu-2.4.6/pyrfu/pyrf/gradient.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/gse2gsm.py` & `pyrfu-2.4.6/pyrfu/pyrf/t_eval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Local imports
-from .cotrans import cotrans
+# Built-in imports
+import bisect
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def gse2gsm(inp, flag: str = "gse>gsm"):
-    r"""Converts GSE to GSM.
+def t_eval(inp, times):
+    r"""Evaluates the input time series at the target time.
 
     Parameters
     ----------
-    inp : xarray.DataArray or ndarray
-        Time series of the input in GSE (GSM) coordinates.
-        If ndarray first column is time in unix format.
-    flag : {"gse>gsm", "gsm>gse"}, Optional
-        Flag for conversion direction. Default is "gse>gsm"
+    inp : xarray.DataArray
+        Time series if the input to evaluate.
+    times : ndarray
+        Times at which the input will be evaluated.
 
     Returns
     -------
-    out : xarray.DataArray or ndarray
-        Time series of the input in GSM (GSE) coordinates.
-        If ndarray first column is time in unix format.
-
-    See also
-    --------
-    pyrfu.pyrf.geocentric_coordinate_transformation
+    out : xarray.DataArray
+        Time series of the input at times t.
 
     """
 
-    assert flag in ["gse>gsm", "gsm>gse"], "invalid flag"
+    idx = np.zeros(len(times))
+
+    for i, time in enumerate(times):
+        idx[i] = bisect.bisect_left(inp.time.data, time)
+
+    idx = idx.astype(np.int64)
 
-    out = cotrans(inp, flag)
+    if inp.ndim == 2:
+        out = xr.DataArray(
+            inp.data[idx, :],
+            coords=[times, inp.comp],
+            dims=["time", "comp"],
+        )
+    else:
+        out = xr.DataArray(inp.data[idx], coords=[times], dims=["time"])
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/histogram.py` & `pyrfu-2.4.6/pyrfu/pyrf/histogram.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Built-in imports
-from typing import Union
-
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def histogram(
-    inp,
-    bins: Union[str, int, np.ndarray, list] = 100,
-    y_range: tuple = None,
-    weights=None,
-    density: bool = True,
-):
+def histogram(inp, bins=100, y_range=None, weights=None, density=True):
     r"""Computes 1D histogram of the inp with bins bins
 
     Parameters
     ----------
     inp : xarray.DataArray
         Time series of the input scalar variable.
     bins : str or int or array_like, Optional
         Number of bins. Default is ``bins=100``.
     y_range : (float, float), Optional
         The lower and upper range of the bins.  If not provided, range
-        is simply ``(a.min(), a.max())``.  Values outside the range are
+        is simply ``(inp.min(), inp.max())``.  Values outside the range are
         ignored. The first element of the range must be less than or
         equal to the second. `range` affects the automatic bin
         computation as well. While bin width is computed to be optimal
         based on the actual data within `range`, the bin count will fill
         the entire range including portions containing no data.
     weights : array_like, Optional
-        An array of weights, of the same shape as `a`.  Each value in
-        `a` only contributes its associated weight towards the bin count
+        An array of weights, of the same shape as `inp`.  Each value in
+        `inp` only contributes its associated weight towards the bin count
         (instead of 1). If `density` is True, the weights are
         normalized, so that the integral of the density over the range
         remains 1.
     density : bool, Optional
         If ``False``, the result will contain the number of samples in each
         bin. If ``True``, the result is the value of the probability *density*
         function at the bin, normalized such that the *integral* over the
@@ -56,14 +47,18 @@
     Returns
     -------
     out : xarray.DataArray
         1D distribution of the input time series.
 
     """
 
+    # Check input
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+    assert inp.ndim == 1, "inp must be a scalar time series"
+
     hist, bins = np.histogram(
         inp.data,
         bins=bins,
         range=y_range,
         weights=weights,
         density=density,
     )
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/histogram2d.py` & `pyrfu-2.4.6/pyrfu/pyrf/histogram2d.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Built-in imports
-from typing import Union
-
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 # Local imports
 from .resample import resample
 
@@ -15,22 +12,15 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def histogram2d(
-    inp1,
-    inp2,
-    bins: Union[str, int, tuple] = 100,
-    y_range: tuple = None,
-    weights=None,
-    density: bool = True,
-):
+def histogram2d(inp1, inp2, bins=100, y_range=None, weights=None, density=True):
     r"""Computes 2d histogram of inp2 vs inp1 with nbins number of bins.
 
     Parameters
     ----------
     inp1 : xarray.DataArray
         Time series of the x coordinates of the points to be histogrammed.
     inp2 : xarray.DataArray
@@ -95,16 +85,16 @@
         inp2 = resample(inp2, inp1)
 
     h2d, x_edges, y_edges = np.histogram2d(
         inp1.data,
         inp2.data,
         bins=bins,
         range=y_range,
-        weights=weights,
         density=density,
+        weights=weights,
     )
 
     x_bins = x_edges[:-1] + np.median(np.diff(x_edges)) / 2
     y_bins = y_edges[:-1] + np.median(np.diff(y_edges)) / 2
 
     out = xr.DataArray(
         h2d,
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/increments.py` & `pyrfu-2.4.6/pyrfu/pyrf/pvi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
-from scipy.stats import kurtosis
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def increments(inp, scale: int = 10):
-    r"""Returns the increments of a time series.
+def pvi(inp, scale: int = 10):
+    r"""Returns the PVI of a time series.
 
-    .. math:: y = |x_i - x_{i+s}|
+    .. math::
+
+        y = \frac{|x_i - x_{i+s}|^2}{<|x_i - x_{i+s}|^2>}
 
     where :math:`s` is the scale.
 
     Parameters
     ----------
     inp : xarray.DataArray
         Input time series.
     scale : int, Optional
-        Scale at which to compute the increments. Default is 10.
+        Scale at which to compute the PVI. Default is 10.
 
     Returns
     -------
-    kurt : ndarray
-        kurtosis of the increments, one per product, using the Fisher's
-        definition (0 value for a normal distribution).
-    result : xarray.DataArray
-        An xarray containing the time series increments, one per
-        product in the original time series.
+    values : xarray.DataArray
+        An xarray containing the pvi of the original time series.
 
     """
 
-    if inp.data.ndim == 1:
+    if len(inp.data.shape) == 1:
         data = inp.data[:, np.newaxis]
     else:
         data = inp.data
 
-    delta_inp = data[scale:, :] - data[:-scale, :]
-
-    result = np.array(delta_inp)
-
-    cols = [inp.coords[dim].data for dim in inp.dims]
-
-    if inp.data.ndim == 1:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[cols[0][0 : len(delta_inp)]],
-            dims=inp.dims,
-            attrs=inp.attrs,
-        )
-    else:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[cols[0][0 : len(delta_inp)], *cols[1:]],
-            dims=inp.dims,
-            attrs=inp.attrs,
-        )
+    delta_inp = np.abs((data[scale:, :] - data[:-scale, :]))
+    delta_inp2 = np.sum(delta_inp**2, axis=1)
+    sigma = np.mean(delta_inp2)
+    result = np.array(delta_inp2 / sigma)
+
+    time = inp.coords[inp.dims[0]].data
+
+    result = xr.DataArray(
+        result,
+        coords=[time[0 : len(delta_inp)]],
+        dims=[inp.dims[0]],
+        attrs=inp.attrs,
+    )
 
-    kurt = kurtosis(result, axis=0, fisher=False)
+    result.attrs["units"] = "dimensionless"
 
-    return kurt, result
+    return result
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/int_sph_dist.py` & `pyrfu-2.4.6/pyrfu/pyrf/int_sph_dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,19 @@
     n_az_g = len(phi)
     d_phi_g = 2 * np.pi / n_az_g
     phi_grid = np.linspace(0, 2 * np.pi - d_phi_g, n_az_g) + d_phi_g / 2
     phi_grid = kwargs.get("phi_grid", phi_grid)
 
     # Overwrite projection dimension if azimuthal angle of projection
     # plane is not provided. Set the azimuthal angle grid width.
-    if phi_grid is None or projection_dim == "1d":
-        projection_dim = "1d"
-        d_phi_grid = 1.0
-    elif phi_grid is not None and projection_dim.lower() in ["2d", "3d"]:
+    if phi_grid is not None and projection_dim.lower() in ["2d", "3d"]:
         d_phi_grid = np.median(np.diff(phi_grid))
     else:
-        raise RuntimeError(
-            "1d projection with phi_grid provided doesn't make sense!!",
-        )
+        projection_dim = "1d"
+        d_phi_grid = 1.0
 
     # Make sure the transformation matrix is orthonormal.
     x_phat = xyz[:, 0] / np.linalg.norm(xyz[:, 0])  # re-normalize
     y_phat = xyz[:, 1] / np.linalg.norm(xyz[:, 1])  # re-normalize
 
     z_phat = np.cross(x_phat, y_phat)
     z_phat /= np.linalg.norm(z_phat)
@@ -131,44 +127,17 @@
         )
     else:
         n_mc_mat = np.zeros_like(vdf)
         n_mc_mat[vdf != 0] = n_mc
 
     n_mc_mat = n_mc_mat.astype(int)
 
-    if projection_base == "pol":
-        # Area or line element (primed)
-        d_a_grid = speed_grid ** (int(projection_dim[0]) - 1) * d_phi_grid * d_v_grid
-        d_a_grid = d_a_grid.astype(np.float64)
-
-        if projection_dim == "1d":
-            f_g = mc_pol_1d(
-                vdf,
-                speed,
-                phi,
-                theta,
-                d_v,
-                d_v_m,
-                d_phi,
-                d_theta,
-                speed_grid_edges,
-                d_a_grid,
-                v_lim,
-                a_lim,
-                n_mc_mat,
-                r_mat,
-            )
-        else:
-            raise NotImplementedError(
-                "2d projection on polar grid is not ready yet!!",
-            )
-
-    elif projection_base == "cart" and projection_dim == "2d":
+    if projection_base == "cart" and projection_dim == "2d":
         d_a_grid = d_v_grid**2
-        f_g = mc_cart_2d(
+        f_g = _mc_cart_2d(
             vdf,
             speed,
             phi,
             theta,
             d_v,
             d_v_m,
             d_phi,
@@ -178,15 +147,15 @@
             v_lim,
             a_lim,
             n_mc_mat,
             r_mat,
         )
     elif projection_base == "cart" and projection_dim == "3d":
         d_a_grid = d_v_grid**3
-        f_g = mc_cart_3d(
+        f_g = _mc_cart_3d(
             vdf,
             speed,
             phi,
             theta,
             d_v,
             d_v_m,
             d_phi,
@@ -195,19 +164,41 @@
             d_a_grid,
             v_lim,
             a_lim,
             n_mc_mat,
             r_mat,
         )
     else:
-        raise ValueError("Invalid base!!")
+        # Area or line element (primed)
+        d_a_grid = speed_grid ** (int(projection_dim[0]) - 1) * d_phi_grid * d_v_grid
+        d_a_grid = d_a_grid.astype(np.float64)
 
-    if projection_dim == "1d":
-        pst = {"f": f_g, "vx": speed_grid, "vx_edges": speed_grid_edges}
-    elif projection_dim == "2d" and projection_base == "cart":
+        if projection_dim == "1d":
+            f_g = _mc_pol_1d(
+                vdf,
+                speed,
+                phi,
+                theta,
+                d_v,
+                d_v_m,
+                d_phi,
+                d_theta,
+                speed_grid_edges,
+                d_a_grid,
+                v_lim,
+                a_lim,
+                n_mc_mat,
+                r_mat,
+            )
+        else:
+            raise NotImplementedError(
+                "2d projection on polar grid is not ready yet!!",
+            )
+
+    if projection_dim == "2d" and projection_base == "cart":
         pst = {
             "f": f_g,
             "vx": speed_grid,
             "vy": speed_grid,
             "vx_edges": speed_grid_edges,
             "vy_edges": speed_grid_edges,
         }
@@ -218,23 +209,21 @@
             "vy": speed_grid,
             "vz": speed_grid,
             "vx_edges": speed_grid_edges,
             "vy_edges": speed_grid_edges,
             "vz_edges": speed_grid_edges,
         }
     else:
-        raise NotImplementedError(
-            "2d projection on polar grid is not ready yet!!",
-        )
+        pst = {"f": f_g, "vx": speed_grid, "vx_edges": speed_grid_edges}
 
     return pst
 
 
 @numba.jit(cache=True, nogil=True, parallel=True, nopython=True)
-def mc_pol_1d(
+def _mc_pol_1d(
     vdf,
     v,
     phi,
     theta,
     d_v,
     d_v_m,
     d_phi,
@@ -337,15 +326,15 @@
                     if use_point * (i_vxg < n_vg):
                         f_g[i_vxg] += f_ijk * c_ijk / d_a
 
     return f_g
 
 
 @numba.jit(cache=True, nogil=True, parallel=True, nopython=True)
-def mc_cart_3d(
+def _mc_cart_3d(
     vdf,
     v,
     phi,
     theta,
     d_v,
     d_v_m,
     d_phi,
@@ -450,15 +439,15 @@
                     if use_point:
                         f_g[i_vxg, i_vyg, i_vzg] += f_ijk * c_ijk / d_a_grid
 
     return f_g
 
 
 @numba.jit(cache=True, nogil=True, parallel=True, nopython=True)
-def mc_cart_2d(
+def _mc_cart_2d(
     vdf,
     v,
     phi,
     theta,
     d_v,
     d_v_m,
     d_phi,
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/integrate.py` & `pyrfu-2.4.6/pyrfu/pyrf/integrate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/iplasma_calc.py` & `pyrfu-2.4.6/pyrfu/pyrf/iplasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/iso2unix.py` & `pyrfu-2.4.6/pyrfu/pyrf/unix2datetime64.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,33 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def iso2unix(time):
-    r"""Converts time in iso format to unix
+def unix2datetime64(time):
+    r"""Converts unix time to datetime64 in ns units.
 
     Parameters
     ----------
-    time : str or list of str
-        Time.
+    time : ndarray
+        Time in unix format.
 
     Returns
     -------
-    out : float or list of float
-        Time in unix format.
+    time_datetime64 : ndarray
+        Time in datetime64 format.
+
+    See Also
+    --------
+    pyrfu.pyrf.datetime642unix
 
     """
 
-    # Convert iso time to unix
-    out = np.array(time).astype("datetime64[ns]")
+    # Make sure that time is in ns format
+    time_unix = (time * 1e9).astype(np.int64)
+
+    # Convert to unix
+    time_datetime64 = time_unix.astype("datetime64[ns]")
 
-    return out
+    return time_datetime64
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime.py` & `pyrfu-2.4.6/pyrfu/pyrf/iso86012datetime.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime64.py` & `pyrfu-2.4.6/pyrfu/pyrf/iso86012datetime64.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
     See Also
     --------
     pyrfu.pyrf.datetime642iso8601
 
     """
 
-    time_datetime64 = time.astype("<M8[ns]")
+    time_datetime64 = time.astype("datetime64[ns]")
 
     return time_datetime64
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/iso86012timevec.py` & `pyrfu-2.4.6/pyrfu/pyrf/iso86012timevec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/l_shell.py` & `pyrfu-2.4.6/pyrfu/pyrf/l_shell.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/lowpass.py` & `pyrfu-2.4.6/pyrfu/pyrf/lowpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/magnetosphere.py` & `pyrfu-2.4.6/pyrfu/pyrf/magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/match_phibe_dir.py` & `pyrfu-2.4.6/pyrfu/pyrf/match_phibe_dir.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/match_phibe_v.py` & `pyrfu-2.4.6/pyrfu/pyrf/match_phibe_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/mean.py` & `pyrfu-2.4.6/pyrfu/pyrf/mean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/mean_bins.py` & `pyrfu-2.4.6/pyrfu/pyrf/mean_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/mean_field.py` & `pyrfu-2.4.6/pyrfu/pyrf/mean_field.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/medfilt.py` & `pyrfu-2.4.6/pyrfu/pyrf/medfilt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/median_bins.py` & `pyrfu-2.4.6/pyrfu/pyrf/median_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/movmean.py` & `pyrfu-2.4.6/pyrfu/pyrf/movmean.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Load ion pressure tensor
 
     >>> p_xyz_i = mms.get_data("Pi_gse_fpi_brst_l2", tint, mms_id)
 
     Running average the pressure tensor over 10s
 
     >>> fs = pyrf.calc_fs(p_xyz_i)
-    >>>> p_xyz_i = pyrf.movmean(p_xyz_i, int(10 * fs))
+    >>> p_xyz_i = pyrf.movmean(p_xyz_i, int(10 * fs))
 
     """
 
     if isinstance(n_pts, float):
         n_pts = np.floor(n_pts).astype(np.int64)
 
     if n_pts % 2:
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/mva.py` & `pyrfu-2.4.6/pyrfu/pyrf/mva.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/mva_gui.py` & `pyrfu-2.4.6/pyrfu/pyrf/mva_gui.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/new_xyz.py` & `pyrfu-2.4.6/pyrfu/pyrf/new_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/norm.py` & `pyrfu-2.4.6/pyrfu/pyrf/norm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/normalize.py` & `pyrfu-2.4.6/pyrfu/pyrf/normalize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_1d.py` & `pyrfu-2.4.6/pyrfu/pyrf/optimize_nbins_1d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_2d.py` & `pyrfu-2.4.6/pyrfu/pyrf/optimize_nbins_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/pid_4sc.py` & `pyrfu-2.4.6/pyrfu/pyrf/pid_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/plasma_beta.py` & `pyrfu-2.4.6/pyrfu/pyrf/plasma_beta.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/plasma_calc.py` & `pyrfu-2.4.6/pyrfu/pyrf/plasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/poynting_flux.py` & `pyrfu-2.4.6/pyrfu/pyrf/poynting_flux.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/pres_anis.py` & `pyrfu-2.4.6/pyrfu/pyrf/pres_anis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/psd.py` & `pyrfu-2.4.6/pyrfu/pyrf/psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/pvi.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_scalar.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,52 +9,41 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def pvi(inp, scale: int = 10):
-    r"""Returns the PVI of a time series.
-
-    .. math::
-
-        y = \frac{|x_i - x_{i+s}|^2}{<|x_i - x_{i+s}|^2>}
-
-    where :math:`s` is the scale.
+def ts_scalar(time, data, attrs: dict = None):
+    r"""Create a time series containing a 0th order tensor
 
     Parameters
     ----------
-    inp : xarray.DataArray
-        Input time series.
-    scale : int, Optional
-        Scale at which to compute the PVI. Default is 10.
+    time : numpy.ndarray
+        Array of times.
+    data : numpy.ndarray
+        Data corresponding to the time list.
+    attrs : dict, Optional
+        Attributes of the data list.
 
     Returns
     -------
-    values : xarray.DataArray
-        An xarray containing the pvi of the original time series.
+    out : xarray.DataArray
+        0th order tensor time series.
 
     """
 
-    if len(inp.data.shape) == 1:
-        data = inp.data[:, np.newaxis]
-    else:
-        data = inp.data
-
-    delta_inp = np.abs((data[scale:, :] - data[:-scale, :]))
-    delta_inp2 = np.sum(delta_inp**2, axis=1)
-    sigma = np.mean(delta_inp2)
-    result = np.array(delta_inp2 / sigma)
-
-    time = inp.coords[inp.dims[0]].data
-
-    result = xr.DataArray(
-        result,
-        coords=[time[0 : len(delta_inp)]],
-        dims=[inp.dims[0]],
-        attrs=inp.attrs,
-    )
+    # Check input type
+    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
+    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
+
+    # Check input shape must be (n, )
+    assert data.ndim == 1, "Input must be a scalar"
+    assert len(time) == len(data), "Time and data must have the same length"
+
+    if attrs is None or not isinstance(attrs, dict):
+        attrs = {}
 
-    result.attrs["units"] = "dimensionless"
+    out = xr.DataArray(data, coords=[time[:]], dims="time", attrs=attrs)
+    out.attrs["TENSOR_ORDER"] = 0
 
-    return result
+    return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/pvi_4sc.py` & `pyrfu-2.4.6/pyrfu/pyrf/pvi_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/read_cdf.py` & `pyrfu-2.4.6/pyrfu/pyrf/read_cdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/remove_repeated_points.py` & `pyrfu-2.4.6/pyrfu/pyrf/remove_repeated_points.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/resample.py` & `pyrfu-2.4.6/pyrfu/pyrf/resample.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/shock_models_parameters.json` & `pyrfu-2.4.6/pyrfu/pyrf/shock_models_parameters.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/shock_normal.py` & `pyrfu-2.4.6/pyrfu/pyrf/shock_normal.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/shock_parameters.py` & `pyrfu-2.4.6/pyrfu/pyrf/shock_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,20 @@
     """
 
     id_b = list(filter(lambda x: x[0].lower() == "b", spec))
     regions = [id_[1:] for id_ in id_b if len(id_) > 1]
     regions = regions if len(regions) > 1 else [""]
 
     spec["ref_sys"] = spec.get("ref_sys", "sc")
+    assert spec["ref_sys"].lower() in ["sc", "nif"], "Invalid reference frame"
 
     if spec["ref_sys"].lower() == "nif":
         if "nvec" not in spec:
-            logging.warning("Setting shock speed, nvec to None")
-            spec["nvec"] = None
+            logging.warning("Setting shock speed, nvec to [1, 0, 0]")
+            spec["nvec"] = np.array([1, 0, 0])
 
         if "v_sh" not in spec:
             logging.warning("Setting shock speed, Vsh, to 0.")
             spec["v_sh"] = 0.0
 
     dspec = {}
 
@@ -127,17 +128,17 @@
                 spec["ref_sys"],
                 spec["v_sh"],
                 spec["nvec"],
             )
 
     # Sonic Mach number
     if (
-        f"t_i{regions[0]}" in spec
+        f"v{regions[0]}" in spec
+        and f"t_i{regions[0]}" in spec
         and f"t_e{regions[0]}" in spec
-        and f"v{regions[0]}" in spec
     ):
         for region in regions:
             dspec[f"m_s{region}"] = _sonic_mach(
                 spec[f"v{region}"],
                 spec[f"t_i{region}"],
                 spec[f"t_e{region}"],
                 spec["ref_sys"],
@@ -146,15 +147,14 @@
             )
 
     if (
         f"n{regions[0]}" in spec
         and f"v{regions[0]}" in spec
         and f"t_i{regions[0]}" in spec
         and f"t_e{regions[0]}" in spec
-        and f"v{regions[0]}" in spec
     ):
         for region in regions:
             dspec[f"m_f{region}"] = _fast_mach(
                 spec[f"b{region}"],
                 spec[f"n{region}"],
                 spec[f"v{region}"],
                 spec[f"t_i{region}"],
@@ -271,51 +271,45 @@
     return v_htf
 
 
 def _alfv_mach(b, n, v, ref_sys, v_sh, nvec):
     v_si = 1e3 * v
     v_sh_si = 1e3 * v_sh
 
-    if ref_sys.lower() == "sc":
-        m_a = np.linalg.norm(v_si) / _v_alfv(b, n)
-    elif ref_sys.lower() == "nif" and nvec is not None:
+    if ref_sys.lower() == "nif" and nvec is not None:
         m_a = np.abs(np.sum(v_si * nvec) - v_sh_si) / _v_alfv(b, n)
     else:
-        raise ValueError("Invalid reference frame")
+        m_a = np.linalg.norm(v_si) / _v_alfv(b, n)
 
     return m_a
 
 
 def _sonic_mach(v, t_i, t_e, ref_sys, v_sh, nvec):
     v_si = 1e3 * v
     v_sh_si = 1e3 * v_sh
 
-    if ref_sys.lower() == "sc":
-        m_s = np.linalg.norm(v_si) / _v_sound(t_i, t_e)
-    elif ref_sys.lower() == "nif" and nvec is not None:
+    if ref_sys.lower() == "nif" and nvec is not None:
         m_s = np.abs(np.sum(v_si * nvec) - v_sh_si) / _v_sound(t_i, t_e)
     else:
-        raise ValueError("Invalid reference frame")
+        m_s = np.linalg.norm(v_si) / _v_sound(t_i, t_e)
 
     return m_s
 
 
 def _fast_mach(b, n, v, t_i, t_e, ref_sys, v_sh, nvec):
     v_si = 1e3 * v
     v_sh_si = 1e3 * v_sh
 
-    if ref_sys.lower() == "sc":
-        m_f = np.linalg.norm(v_si) / _v_fast(b, n, v, t_i, t_e)
-    elif ref_sys.lower() == "nif" and nvec is not None:
+    if ref_sys.lower() == "nif" and nvec is not None:
         theta_bn = np.rad2deg(np.arccos(np.sum(b * nvec) / np.linalg.norm(b)))
         m_f = np.abs(np.sum(v_si * nvec) - v_sh_si) / _v_fast(
             b, n, v, t_i, t_e, theta_bn
         )
     else:
-        raise ValueError("Invalid reference frame")
+        m_f = np.linalg.norm(v_si) / _v_fast(b, n, v, t_i, t_e)
 
     return m_f
 
 
 def _beta(b, n, t_s):
     b_si = 1e-9 * np.linalg.norm(b)
     n_si = 1e6 * n
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/sph2cart.py` & `pyrfu-2.4.6/pyrfu/pyrf/sph2cart.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/st_diff.py` & `pyrfu-2.4.6/pyrfu/pyrf/st_diff.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/struct_func.py` & `pyrfu-2.4.6/pyrfu/pyrf/struct_func.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/time_clip.py` & `pyrfu-2.4.6/pyrfu/pyrf/time_clip.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/timevec2iso8601.py` & `pyrfu-2.4.6/pyrfu/pyrf/timevec2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/trace.py` & `pyrfu-2.4.6/pyrfu/pyrf/trace.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/transformation_indices.json` & `pyrfu-2.4.6/pyrfu/pyrf/transformation_indices.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_append.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_scalar.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_tensor_xyz.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,47 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def ts_scalar(time, data, attrs: dict = None):
-    r"""Create a time series containing a 0th order tensor
+def ts_tensor_xyz(time, data, attrs: dict = None):
+    r"""Create a time series containing a 2nd order tensor.
 
     Parameters
     ----------
-    time : numpy.ndarray
+    time : ndarray
         Array of times.
-    data : numpy.ndarray
+    data : ndarray
         Data corresponding to the time list.
     attrs : dict, Optional
         Attributes of the data list.
 
     Returns
     -------
     out : xarray.DataArray
-        0th order tensor time series.
+        2nd order tensor time series.
 
     """
 
     # Check input type
     assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
     assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
 
-    # Check input shape must be (n, )
-    assert data.ndim == 1, "Input must be a scalar"
+    # Check input shape must be (n, 3, 3)
+    assert data.ndim == 3 and data.shape[1:] == (3, 3)
     assert len(time) == len(data), "Time and data must have the same length"
 
     if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
-    out = xr.DataArray(data, coords=[time[:]], dims="time", attrs=attrs)
-    out.attrs["TENSOR_ORDER"] = 0
+    out = xr.DataArray(
+        data,
+        coords=[time[:], ["x", "y", "z"], ["x", "y", "z"]],
+        dims=["time", "comp_h", "comp_v"],
+        attrs=attrs,
+    )
+
+    out.attrs["TENSOR_ORDER"] = 2
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_skymap.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_tensor_xyz.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_vec_xyz.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def ts_tensor_xyz(time, data, attrs: dict = None):
-    r"""Create a time series containing a 2nd order tensor.
+def ts_vec_xyz(time, data, attrs: dict = None):
+    r"""Create a time series containing a 1st order tensor.
 
     Parameters
     ----------
     time : ndarray
         Array of times.
     data : ndarray
         Data corresponding to the time list.
     attrs : dict, Optional
         Attributes of the data list.
 
     Returns
     -------
     out : xarray.DataArray
-        2nd order tensor time series.
+        1st order tensor time series.
 
     """
 
     # Check input type
     assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
     assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
 
-    # Check input shape must be (n, 3, 3)
-    assert data.ndim == 3 and data.shape[1:] == (3, 3)
+    # Check input shape must be (n, 3)
+    assert data.ndim == 2 and data.shape[1] == 3
     assert len(time) == len(data), "Time and data must have the same length"
 
     if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
     out = xr.DataArray(
         data,
-        coords=[time[:], ["x", "y", "z"], ["x", "y", "z"]],
-        dims=["time", "comp_h", "comp_v"],
+        coords=[time[:], ["x", "y", "z"]],
+        dims=["time", "comp"],
         attrs=attrs,
     )
 
-    out.attrs["TENSOR_ORDER"] = 2
+    out.attrs["TENSOR_ORDER"] = 1
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_time.py` & `pyrfu-2.4.6/pyrfu/pyrf/ts_time.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ts_vec_xyz.py` & `pyrfu-2.4.6/pyrfu/pyrf/increments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
+from scipy.stats import kurtosis
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def ts_vec_xyz(time, data, attrs: dict = None):
-    r"""Create a time series containing a 1st order tensor.
+def increments(inp, scale: int = 10):
+    r"""Returns the increments of a time series.
+
+    .. math:: y = |x_i - x_{i+s}|
+
+    where :math:`s` is the scale.
 
     Parameters
     ----------
-    time : ndarray
-        Array of times.
-    data : ndarray
-        Data corresponding to the time list.
-    attrs : dict, Optional
-        Attributes of the data list.
+    inp : xarray.DataArray
+        Input time series.
+    scale : int, Optional
+        Scale at which to compute the increments. Default is 10.
 
     Returns
     -------
-    out : xarray.DataArray
-        1st order tensor time series.
+    kurt : ndarray
+        kurtosis of the increments, one per product, using the Fisher's
+        definition (0 value for a normal distribution).
+    result : xarray.DataArray
+        An xarray containing the time series increments, one per
+        product in the original time series.
 
     """
 
-    # Check input type
-    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
-    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
-
-    # Check input shape must be (n, 3)
-    assert data.ndim == 2 and data.shape[1] == 3
-    assert len(time) == len(data), "Time and data must have the same length"
-
-    if attrs is None or not isinstance(attrs, dict):
-        attrs = {}
-
-    out = xr.DataArray(
-        data,
-        coords=[time[:], ["x", "y", "z"]],
-        dims=["time", "comp"],
-        attrs=attrs,
-    )
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+    assert inp.ndim < 4, "inp must ber a scalar, vector or tensor"
 
-    out.attrs["TENSOR_ORDER"] = 1
+    if inp.ndim == 1:
+        data = inp.data[:, np.newaxis]
+    else:
+        data = inp.data
+
+    # Compute the increments
+    delta_inp = data[scale:, ...] - data[:-scale, ...]
+
+    # Compute kurtosis of the increments
+    kurt = kurtosis(delta_inp, axis=0, fisher=False)
+
+    times, *comp = [inp.coords[dim].data for dim in inp.dims]
+
+    result = xr.DataArray(
+        np.squeeze(delta_inp),
+        coords=[times[0 : len(delta_inp)], *comp],
+        dims=inp.dims,
+        attrs=inp.attrs,
+    )
 
-    return out
+    return kurt, result
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/ttns2datetime64.py` & `pyrfu-2.4.6/pyrfu/pyrf/ttns2datetime64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
+import numpy as np
 from cdflib import cdfepoch
 
 # Local imports
 from .timevec2iso8601 import timevec2iso8601
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
@@ -27,17 +28,20 @@
     Returns
     -------
     time_datetime64 : ndarray
         Time in datetime64 format in ns units.
 
     """
 
+    message = "time must be float, int, or array_like"
+    assert isinstance(time, (float, int, list, np.ndarray)), message
+
     #
     time_tt2000 = cdfepoch.breakdown_tt2000(time)
 
     # Convert to ISO 8601 string 'YYYY-MM-DDThh:mm:ss.mmmuuunnn'
     time_iso8601 = timevec2iso8601(time_tt2000)
 
     #
-    time_datetime64 = time_iso8601.astype("<M8[ns]")
+    time_datetime64 = time_iso8601.astype("datetime64[ns]")
 
     return time_datetime64
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/vht.py` & `pyrfu-2.4.6/pyrfu/pyrf/vht.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/wave_fft.py` & `pyrfu-2.4.6/pyrfu/pyrf/wave_fft.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/wavelet.py` & `pyrfu-2.4.6/pyrfu/pyrf/wavelet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import logging
-
 # Built-in imports
+import logging
 import os
 
 # 3rd party imports
 import numba
 import numpy as np
 import xarray as xr
 from scipy import fft
@@ -90,19 +89,21 @@
     n_freqs = kwargs.get("nf", 200)
     wavelet_width = kwargs.get("wavelet_width", 5.36)
     cut_edge = kwargs.get("cut_edge", True)
     return_power = kwargs.get("return_power", True)
 
     if kwargs.get("linear"):
         linear_df = True
-        if isinstance(kwargs["linear"], (int, float)):
-            delta_f = kwargs["linear"]
-        else:
+        if isinstance(kwargs["linear"], bool) and kwargs["linear"]:
             delta_f = 100
             logging.warning("Unknown input for linear delta_f set to 100")
+        elif isinstance(kwargs["linear"], (int, float)):
+            delta_f = kwargs["linear"]
+        else:
+            raise TypeError("linear keyword argument must be bool, float or int")
     else:
         delta_f = 100
         linear_df = False
 
     scale_min, scale_max = [0.01, 2]
 
     f_min, f_max = kwargs.get(
@@ -196,16 +197,14 @@
 
     if len(inp.shape) == 1:
         out = xr.DataArray(
             np.fliplr(power2),
             coords=[time, np.flip(new_freq)],
             dims=["time", "frequency"],
         )
-    elif len(inp.shape) == 2:
+    else:
         out = xr.Dataset(
             out_dict,
             coords={"time": time, "frequency": np.flip(new_freq)},
         )
-    else:
-        raise TypeError("Invalid shape")
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/wavepolarize_means.py` & `pyrfu-2.4.6/pyrfu/pyrf/wavepolarize_means.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/pyrf/waverage.py` & `pyrfu-2.4.6/pyrfu/pyrf/waverage.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/solo/db_init.py` & `pyrfu-2.4.6/pyrfu/solo/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu/solo/read_lfr_density.py` & `pyrfu-2.4.6/pyrfu/solo/read_lfr_density.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,21 @@
     -------
     files : list
         List of files corresponding to the parameters in the selected time
         interval
 
     """
 
+    # Check input types
+    assert isinstance(tint, (list, np.ndarray)), "tint must be array_like"
+    assert len(tint) == 2, "tint must contain two elements"
+    assert isinstance(tint[0], str), "tint[0] must be a string"
+    assert isinstance(tint[1], str), "tint[1] must be a string"
+    assert isinstance(tree, bool), "tree must be a boolean"
+
     # Check path
     if not data_path:
         # pkg_path = os.path.dirname(os.path.abspath(__file__))
         pkg_path = os.path.dirname(os.path.abspath(__file__))
 
         # Read the current version of the MMS configuration file
         with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
```

### Comparing `pyrfu-2.4.5/pyrfu/solo/read_tnr.py` & `pyrfu-2.4.6/pyrfu/solo/read_tnr.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,20 @@
     # directory and file name search patterns:
     # - assume directories are of the form: [data_path]/L2/thr/year/month/
     # - assume file names are of the form:
     #   solo_L2_rpw-tnr-surv-cdag_YYYYMMDD_version.cdf
 
     file_name = r"solo_L2_rpw-tnr-surv.*_([0-9]{8})_V[0-9]{2}.cdf"
 
+    # Check tint
+    assert isinstance(tint, (list, np.ndarray)), "tint must be array_like"
+    assert len(tint) == 2, "tint must contain two elements"
+    assert isinstance(tint[0], str), "tint[0] must be a string"
+    assert isinstance(tint[1], str), "tint[1] must be a string"
+
     d_start = parser.parse(parser.parse(tint[0]).strftime("%Y-%m-%d"))
     until_ = parser.parse(tint[1]) - datetime.timedelta(seconds=1)
     days = rrule(DAILY, dtstart=d_start, until=until_)
 
     for date in days:
         if tree:
             local_dir = os.sep.join(
@@ -152,17 +158,18 @@
     Notes
     -----
     The script check if there are data from the two channel and put them
     together.
 
     """
 
-    files = _list_files_tnr_l2(tint, data_path, tree)
+    # Check input types
+    assert isinstance(sensor, int), "sensor must integer"
 
-    assert files, "No files found. Make sure that the data_path is correct"
+    files = _list_files_tnr_l2(tint, data_path, tree)
 
     # Initialize spectrum output to None
     out = None
 
     for file in files:
         # Notify user
         logging.info("Loading %s...", os.path.split(file)[-1])
@@ -271,10 +278,10 @@
             xr.DataArray(
                 vp,
                 coords=[np.stack(time), freq_tnr],
                 dims=["time", "frequency"],
             ),
         )
 
-    out = out[np.argsort(out.time.data)]
+        out = out[np.argsort(out.time.data)]
 
     return out
```

### Comparing `pyrfu-2.4.5/pyrfu/tests/test_dispersion.py` & `pyrfu-2.4.6/pyrfu/tests/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.5/pyrfu.egg-info/PKG-INFO` & `pyrfu-2.4.6/pyrfu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -29,25 +29,27 @@
 Project-URL: documentation, https://pyrfu.readthedocs.io/en/latest/
 Project-URL: source, https://github.com/louis-richard/irfu-python
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: MS-DOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
@@ -81,14 +83,20 @@
 
 .. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
 .. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
+.. |CodeQL| image:: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml/badge.svg
+.. _CodeQL: https://github.com/louis-richard/irfu-python/actions/workflows/codeql.yml
+
+.. |CodeCov| image:: https://codecov.io/gh/louis-richard/irfu-python/coverage.svg?branch=main
+.. _CodeCov: https://codecov.io/gh/louis-richard/irfu-python/branch/main
+
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
 .. |Commits| image:: https://img.shields.io/github/last-commit/louis-richard/irfu-python?logo=github&color=9cf
 .. _Commits: https://github.com/louis-richard/irfu-python/commits/master
 
 .. |Readthedocs| image:: https://img.shields.io/readthedocs/pyrfu?logo=read-the-docs&color=blueviolet
@@ -97,84 +105,73 @@
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
 |License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
-|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|PyLintB|_ |CodeQL|_ |CodeCov|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
-The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
-Magnetospheric MultiScale (MMS) mission.
+The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
-.. end-marker-intro-do-not-remove
-
-Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
-
-
 Quickstart
 ==========
 
-Installing pyrfu with pip (`more details here`_):
-
-.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
+Installing pyrfu with pip (`more details here <https://pyrfu.readthedocs.io/en/latest/installation.html>`_):
 
 .. code-block:: console
 
     $ python -m pip install pyrfu
     # or
     $ python -m pip install --user pyrfu
 
-Import `pyrfu.mms`_ package with routines specific to work with the
+Import `pyrfu.mms <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html>`_ package with routines specific to work with the
 Magnetospheric Multiscale mission (MMS)
 
-.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
-
 .. code:: python
 
     from pyrfu import mms
 
 Setup path to MMS data
 
 .. code:: python
 
     mms.db_init("/Volumes/mms")
 
+
 Load magnetic field and ion bulk velocity data
 
 .. code:: python
 
     tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
     b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
     v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-Import `pyrfu.pyrf`_ package with generic routines
 
-.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
+Import `pyrfu.pyrf <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html>`_ package with generic routines
 
 .. code:: python
 
     from pyrfu import pyrf
 
 Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
     v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
-Import `pyrfu.plot`_ package with plotting routines
-
-.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
+Import `pyrfu.plot <https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html>`_ package with plotting routines
 
 .. code:: python
 
     from pyrfu import plot
 
+
 Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
     import matplotlib.pyplot as plt
 
     f, axs = plt.subplots(2, sharex="all")
@@ -182,24 +179,33 @@
     axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
     axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
 
     plot.plot_line(axs[1], v_gsm_i)
     axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
     axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
+.. end-marker-intro-do-not-remove
+
+Documentation
+=============
+Full documentation can be found on `pyrfu.readthedocs.io <https://pyrfu.readthedocs.io/en/latest/index.html>`_
+
+Examples
+========
+A list of examples is available `here <https://pyrfu.readthedocs.io/en/latest/examples/index.html>`_
 
 Credits
--------
+=======
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
----------------
+===============
 Please use the following to acknowledge use of pyrfu in your publications:
 Data analysis was performed using the pyrfu analysis package available at https://github.com/louis-richard/irfu-python
 
 Additional Information
-----------------------
+======================
 MMS Science Data Center: https://lasp.colorado.edu/mms/sdc/public/
 
 MMS Datasets: https://lasp.colorado.edu/mms/sdc/public/datasets/
 
 MMS - Goddard Space Flight Center: http://mms.gsfc.nasa.gov/
```

### Comparing `pyrfu-2.4.5/pyrfu.egg-info/SOURCES.txt` & `pyrfu-2.4.6/pyrfu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -199,18 +199,18 @@
 pyrfu/pyrf/gse2gsm.py
 pyrfu/pyrf/histogram.py
 pyrfu/pyrf/histogram2d.py
 pyrfu/pyrf/increments.py
 pyrfu/pyrf/int_sph_dist.py
 pyrfu/pyrf/integrate.py
 pyrfu/pyrf/iplasma_calc.py
-pyrfu/pyrf/iso2unix.py
 pyrfu/pyrf/iso86012datetime.py
 pyrfu/pyrf/iso86012datetime64.py
 pyrfu/pyrf/iso86012timevec.py
+pyrfu/pyrf/iso86012unix.py
 pyrfu/pyrf/l_shell.py
 pyrfu/pyrf/lowpass.py
 pyrfu/pyrf/magnetosphere.py
 pyrfu/pyrf/match_phibe_dir.py
 pyrfu/pyrf/match_phibe_v.py
 pyrfu/pyrf/mean.py
 pyrfu/pyrf/mean_bins.py
@@ -265,8 +265,9 @@
 pyrfu/solo/__init__.py
 pyrfu/solo/config.json
 pyrfu/solo/db_init.py
 pyrfu/solo/read_lfr_density.py
 pyrfu/solo/read_tnr.py
 pyrfu/tests/__init__.py
 pyrfu/tests/test_dispersion.py
-pyrfu/tests/test_pyrf.py
+pyrfu/tests/test_pyrf.py
+pyrfu/tests/test_solo.py
```

