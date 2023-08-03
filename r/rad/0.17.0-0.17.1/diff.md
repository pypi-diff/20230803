# Comparing `tmp/rad-0.17.0.tar.gz` & `tmp/rad-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.17.0.tar", last modified: Thu Jul 27 20:01:18 2023, max compression
+gzip compressed data, was "rad-0.17.1.tar", last modified: Thu Aug  3 19:31:57 2023, max compression
```

## Comparing `rad-0.17.0.tar` & `rad-0.17.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.949386 rad-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 20:01:09.000000 rad-0.17.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 20:01:09.000000 rad-0.17.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 20:01:09.000000 rad-0.17.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 20:01:09.000000 rad-0.17.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-27 20:01:09.000000 rad-0.17.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-27 20:01:09.000000 rad-0.17.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-27 20:01:09.000000 rad-0.17.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-27 20:01:09.000000 rad-0.17.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-27 20:01:09.000000 rad-0.17.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 20:01:09.000000 rad-0.17.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-27 20:01:09.000000 rad-0.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-27 20:01:18.945386 rad-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 20:01:09.000000 rad-0.17.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-27 20:01:09.000000 rad-0.17.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 20:01:09.000000 rad-0.17.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 20:01:09.000000 rad-0.17.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-07-27 20:01:09.000000 rad-0.17.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-27 20:01:09.000000 rad-0.17.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 20:01:09.000000 rad-0.17.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-27 20:01:09.000000 rad-0.17.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 20:01:09.000000 rad-0.17.0/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 20:01:09.000000 rad-0.17.0/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 20:01:09.000000 rad-0.17.0/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 20:01:09.000000 rad-0.17.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-07-27 20:01:09.000000 rad-0.17.0/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-07-27 20:01:09.000000 rad-0.17.0/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:01:18.949386 rad-0.17.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.933386 rad-0.17.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.941386 rad-0.17.0/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/variance-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-27 20:01:09.000000 rad-0.17.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.937386 rad-0.17.0/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 20:01:18.000000 rad-0.17.0/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:18.945386 rad-0.17.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:09.000000 rad-0.17.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 20:01:09.000000 rad-0.17.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-27 20:01:09.000000 rad-0.17.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 20:01:09.000000 rad-0.17.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.333656 rad-0.17.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 19:31:45.000000 rad-0.17.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-03 19:31:45.000000 rad-0.17.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-03 19:31:45.000000 rad-0.17.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-03 19:31:45.000000 rad-0.17.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-03 19:31:45.000000 rad-0.17.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 19:31:45.000000 rad-0.17.1/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 19:31:45.000000 rad-0.17.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-03 19:31:45.000000 rad-0.17.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-03 19:31:45.000000 rad-0.17.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-03 19:31:45.000000 rad-0.17.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-03 19:31:45.000000 rad-0.17.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-08-03 19:31:45.000000 rad-0.17.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-03 19:31:45.000000 rad-0.17.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 19:31:45.000000 rad-0.17.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-03 19:31:45.000000 rad-0.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:45.000000 rad-0.17.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-03 19:31:57.333656 rad-0.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-03 19:31:45.000000 rad-0.17.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 19:31:45.000000 rad-0.17.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 19:31:45.000000 rad-0.17.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-08-03 19:31:45.000000 rad-0.17.1/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.317656 rad-0.17.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-03 19:31:45.000000 rad-0.17.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 19:31:45.000000 rad-0.17.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-03 19:31:45.000000 rad-0.17.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 19:31:45.000000 rad-0.17.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-08-03 19:31:45.000000 rad-0.17.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-03 19:31:45.000000 rad-0.17.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 19:31:45.000000 rad-0.17.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-03 19:31:45.000000 rad-0.17.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-03 19:31:45.000000 rad-0.17.1/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 19:31:45.000000 rad-0.17.1/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 19:31:45.000000 rad-0.17.1/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-03 19:31:45.000000 rad-0.17.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-08-03 19:31:45.000000 rad-0.17.1/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-08-03 19:31:45.000000 rad-0.17.1/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:31:57.333656 rad-0.17.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.317656 rad-0.17.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.321656 rad-0.17.1/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.325656 rad-0.17.1/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.325656 rad-0.17.1/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.329656 rad-0.17.1/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.329656 rad-0.17.1/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.333656 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/variance-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 19:31:45.000000 rad-0.17.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.325656 rad-0.17.1/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 19:31:57.000000 rad-0.17.1/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:57.333656 rad-0.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:31:45.000000 rad-0.17.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-03 19:31:45.000000 rad-0.17.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-03 19:31:45.000000 rad-0.17.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 19:31:45.000000 rad-0.17.1/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-08-03 19:31:45.000000 rad-0.17.1/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-03 19:31:45.000000 rad-0.17.1/tox.ini
```

### Comparing `rad-0.17.0/.github/pull_request_template.md` & `rad-0.17.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.github/workflows/changelog.yml` & `rad-0.17.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.github/workflows/ci.yml` & `rad-0.17.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.github/workflows/publish-to-pypi.yml` & `rad-0.17.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.github/workflows/release.yml` & `rad-0.17.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.gitignore` & `rad-0.17.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/.pre-commit-config.yaml` & `rad-0.17.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,21 +30,21 @@
   hooks:
     - id: codespell
       args: ["--write-changes"]
       additional_dependencies:
         - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: 'v3.9.0'
+  rev: 'v3.10.1'
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.0.280'
+  rev: 'v0.0.281'
   hooks:
     - id: ruff
       args: ["--fix"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
```

### Comparing `rad-0.17.0/CHANGES.rst` & `rad-0.17.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-0.18.0 (unreleased)
+0.17.2 (unreleased)
 -------------------
 
 -
 
+0.17.1 (2023-08-03)
+-------------------
+
+- Added "archive_catalog" field to ref_file. [#303]
+
+- Added a prefix "s_" to the archive destination in "cal_step". [#303]
+
+- Require all the new ``cal_step`` steps to be present in the ``cal_step`` schema. [#301]
+
+- Add missing unit enforcements to various schemas. [#300]
+
 0.17.0 (2023-07-27)
 -------------------
 
 - Fix invalid uri fragment in rad_schema. [#286]
 
 - Update the steps listed in ``cal_step`` to reflect the currently implemented steps.
   The new additions are ``outlier_detection``, ``refpix``, ``sky_match``, and ``tweak_reg``. [#282]
 
 - Update the steps listed in ``cal_step`` with the ``resample`` step. [#295]
 
 - Fix the URIs for ``inverselinearity`` and add consistency checks for names/uris. [#296]
 
+- Add ``archive_meta`` keyword for the MAST archive to encode information specific
+  to the archive's needs. [#279]
+
 0.16.0 (2023-06-26)
 -------------------
 
 - Fix minor discrepancies found when looking over the schemas. [#267]
 
 - Bugfix for ``inverse_linearity-1.0.0``'s ``reftype`` so that it is CRDS
   compatible. [#272]
```

### Comparing `rad-0.17.0/CODE_OF_CONDUCT.md` & `rad-0.17.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/LICENSE` & `rad-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/PKG-INFO` & `rad-0.17.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.17.0
+Version: 0.17.1
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.17.0/README.md` & `rad-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/Makefile` & `rad-0.17.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/_static/custom.css` & `rad-0.17.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/_static/stsci_logo.png` & `rad-0.17.1/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/conf.py` & `rad-0.17.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/index.rst` & `rad-0.17.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/make.bat` & `rad-0.17.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/docs/schemas.rst` & `rad-0.17.1/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/pyproject.toml` & `rad-0.17.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/scripts/insert_next_release.py` & `rad-0.17.1/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/scripts/set_release_date.py` & `rad-0.17.1/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/integration.py` & `rad-0.17.1/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.17.1/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/cal_step-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/cal_step-1.0.0.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,111 +8,111 @@
 properties:
   assign_wcs:
     title: Assign World Coordinate System
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.assign_wcs, GuideWindow.assign_wcs]
+      destination: [ScienceRefData.s_assign_wcs, GuideWindow.s_assign_wcs]
   flat_field:
     title: Flat Field Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.flat_field, GuideWindow.flat_field]
+      destination: [ScienceRefData.s_flat_field, GuideWindow.s_flat_field]
   dark:
     title: Dark Subtraction
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.dark, GuideWindow.dark]
+      destination: [ScienceRefData.s_dark, GuideWindow.s_dark]
   dq_init:
     title: Data Quality Mask Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.dq_init, GuideWindow.dq_init]
+      destination: [ScienceRefData.s_dq_init, GuideWindow.s_dq_init]
   jump:
     title: Jump Detection Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.jump, GuideWindow.jump]
+      destination: [ScienceRefData.s_jump, GuideWindow.s_jump]
   linearity:
     title: Linearity Correction
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.linearity, GuideWindow.linearity]
+      destination: [ScienceRefData.s_linearity, GuideWindow.s_linearity]
   photom:
     title: Photometry Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.photom, GuideWindow.photom]
+      destination: [ScienceRefData.s_photom, GuideWindow.s_photom]
   source_detection:
     title: Source Detection Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.source_detection, GuideWindow.source_detection]
+      destination: [ScienceRefData.s_source_detection, GuideWindow.s_source_detection]
   ramp_fit:
     title: Ramp Fitting
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.ramp_fit, GuideWindow.ramp_fit]
+      destination: [ScienceRefData.s_ramp_fit, GuideWindow.s_ramp_fit]
   refpix:
     title: Reference Pixel Correction
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.refpix, GuideWindow.refpix]
+      destination: [ScienceRefData.s_refpix, GuideWindow.s_refpix]
   saturation:
     title: Saturation Checking
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.saturation, GuideWindow.saturation]
+      destination: [ScienceRefData.s_saturation, GuideWindow.s_saturation]
   outlier_detection:
     title: outlier_detection
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.outlier_detection, GuideWindow.outlier_detection]
+      destination: [ScienceRefData.s_outlier_detection, GuideWindow.s_outlier_detection]
   tweakreg:
     title: Tweakreg step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.tweakreg, GuideWindow.tweak_reg]
+      destination: [ScienceRefData.s_tweakreg, GuideWindow.s_tweakreg]
   skymatch:
     title: Sky Match step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.skymatch, GuideWindow.skymatch]
+      destination: [ScienceRefData.s_skymatch, GuideWindow.s_skymatch]
   resample:
     title: Resample Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.resample, GuideWindow.skymatch]
+      destination: [ScienceRefData.s_resample, GuideWindow.s_resample]
 propertyOrder: [assign_wcs, flat_field, dark, dq_init, jump, linearity, photom, source_detection, outlier_detection, ramp_fit, refpix, saturation, skymatch, tweakreg, resample]
 flowStyle: block
-required: [assign_wcs, flat_field, dark, dq_init, jump, linearity, photom, source_detection, ramp_fit, saturation]
+required: [assign_wcs, flat_field, dark, dq_init, jump, linearity, outlier_detection, photom, source_detection, ramp_fit, refpix, resample, saturation, skymatch, tweakreg]
 additionalProperties: true
 ...
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/guidewindow-1.0.0
 
 title: Guide window information
 
 datamodel_name: GuidewindowModel
 
+archive_meta: None
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/photometry-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/pixelarea-1.0.0
+
+title: Pixel area reference schema
+
+datamodel_name: PixelareaRefModel
 
-title: Photometry information
 type: object
 properties:
-  conversion_megajanskys:
-    title: Flux density (MJy/steradian) producing 1 cps
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.conversion_megajanskys]
-  conversion_microjanskys:
-    title: Flux density (uJy/arcsec2) producing 1 cps
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.conversion_microjanskys]
-  pixelarea_steradians:
-    title: Nominal pixel area in steradians
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.pixelarea_steradians]
-  pixelarea_arcsecsq:
-    title: Nominal pixel area in arcsec^2
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.pixelarea_arcsecsq]
-  conversion_megajanskys_uncertainty:
-    title: Uncertainty in flux density conversion to MJy/steradians
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.conversion_megajanskys_uncertainty]
-  conversion_microjanskys_uncertainty:
-    title: Uncertainty in flux density conversion to uJy/steradians
-    anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      - type: "null"
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.conversion_microjanskys_uncertainty]
-propertyOrder: [conversion_microjanskys, conversion_megajanskys,
-                pixelarea_steradians, pixelarea_arcsecsq,
-                conversion_megajanskys_uncertainty, conversion_microjanskys_uncertainty]
+  meta:
+    allOf:
+      - $ref: ref_common-1.0.0
+      - type: object
+        properties:
+          reftype:
+            type: string
+            enum: [AREA]
+          photometry:
+            type: object
+            properties:
+              pixelarea_steradians:
+                title: Nominal pixel area in steradians
+                anyOf:
+                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                    properties:
+                      datatype:
+                        enum: ["float64"]
+                      unit:
+                        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                        enum: ["sr"]
+                  - type: "null"
+              pixelarea_arcsecsq:
+                title: Nominal pixel area in arcsec^2
+                anyOf:
+                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                    properties:
+                      datatype:
+                        enum: ["float64"]
+                      unit:
+                        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                        enum: ["arcsec**2"]
+                  - type: "null"
+            required: [pixelarea_steradians, pixelarea_arcsecsq]
+        required: [photometry]
+      - $ref: ref_optical_element-1.0.0
+  data:
+    title: Pixel area array
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: float32
+    ndim: 2
+required: [meta, data]
 flowStyle: block
-required: [conversion_microjanskys, conversion_megajanskys,
-           pixelarea_steradians, pixelarea_arcsecsq,
-           conversion_megajanskys_uncertainty, conversion_microjanskys_uncertainty]
+propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,20 @@
   - type: object
     properties:
       datamodel_name:
         description: |-
           The name of the datamodel that this schema describes.
         type: string
 
+      archive_meta:
+        description: |-
+          Metadata to aide the archive in determining how to handle
+          a given file.
+        type: string
+
       sdf:
         description: |-
           Documents source of this attribute's value when level 1
           files are created.
         type: object
         properties:
           special_processing:
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/pixelarea-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
 
-title: Pixel area reference schema
+title: Super-bias reference schema
 
-datamodel_name: PixelareaRefModel
+datamodel_name: SuperbiasRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [AREA]
-          photometry:
-            type: object
-            properties:
-              pixelarea_steradians:
-                title: Nominal pixel area in steradians
-                anyOf:
-                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-                  - type: "null"
-              pixelarea_arcsecsq:
-                title: Nominal pixel area in arcsec^2
-                anyOf:
-                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-                  - type: "null"
-            required: [pixelarea_steradians, pixelarea_arcsecsq]
-        required: [photometry]
-      - $ref: ref_optical_element-1.0.0
+            enum: [BIAS]
   data:
-    title: Pixel area array
+    title: 2-D super-bias array
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: float32
     ndim: 2
-required: [meta, data]
+  dq:
+    title: 2-D data quality array for all planes
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+  err:
+    title: 2-D Error array
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: float32
+    ndim: 2
+required: [meta, data, dq, err]
 flowStyle: block
-propertyOrder: [meta, data]
+propertyOrder: [meta, data, dq, err]
 ...
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/wfi_science_raw-1.0.0
 
-title: Super-bias reference schema
+title: |
+  The schema for Level 1 WFI science data (both imaging and spectrographic).
 
-datamodel_name: SuperbiasRefModel
+datamodel_name: ScienceRawModel
+
+archive_meta: None
 
 type: object
 properties:
   meta:
-    allOf:
-      - $ref: ref_common-1.0.0
-      - type: object
-        properties:
-          reftype:
-            type: string
-            enum: [BIAS]
+    $ref: common-1.0.0
   data:
-    title: 2-D super-bias array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
-  dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  err:
-    title: 2-D Error array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
-required: [meta, data, dq, err]
+    title: Science data, including the border reference pixels.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: uint16
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+  amp33:
+    title: Amp 33 reference pixel data.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: uint16
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+propertyOrder: [meta, data, amp33]
 flowStyle: block
-propertyOrder: [meta, data, dq, err]
+required: [meta, data, amp33]
 ...
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/variance-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/variance-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_image-1.0.0
 
 title: |
   The schema for WFI Level 2 images.
 
 datamodel_name: ImageModel
+archive_meta: None
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
```

### Comparing `rad-0.17.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.17.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_mosaic-1.0.0
 
 title: |
   The schema for WFI Level 3 mosaics.
 
 datamodel_name: MosaicModel
 
+archive_meta: None
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.17.0/src/rad.egg-info/PKG-INFO` & `rad-0.17.1/src/rad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.17.0
+Version: 0.17.1
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.17.0/src/rad.egg-info/SOURCES.txt` & `rad-0.17.1/src/rad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/tests/test_integration.py` & `rad-0.17.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/tests/test_manifest.py` & `rad-0.17.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/tests/test_schemas.py` & `rad-0.17.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rad-0.17.0/tox.ini` & `rad-0.17.1/tox.ini`

 * *Files identical despite different names*

