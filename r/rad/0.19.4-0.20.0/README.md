# Comparing `tmp/rad-0.19.4.tar.gz` & `tmp/rad-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.19.4.tar", last modified: Wed May  8 20:40:30 2024, max compression
+gzip compressed data, was "rad-0.20.0.tar", last modified: Wed May 15 15:55:30 2024, max compression
```

## Comparing `rad-0.19.4.tar` & `rad-0.20.0.tar`

### file list

```diff
@@ -1,148 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.926424 rad-0.19.4/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:40:20.000000 rad-0.19.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.902424 rad-0.19.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 20:40:20.000000 rad-0.19.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:40:20.000000 rad-0.19.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.902424 rad-0.19.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-08 20:40:20.000000 rad-0.19.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 20:40:20.000000 rad-0.19.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 20:40:20.000000 rad-0.19.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-08 20:40:20.000000 rad-0.19.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-08 20:40:20.000000 rad-0.19.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 20:40:20.000000 rad-0.19.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 20:40:20.000000 rad-0.19.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-08 20:40:30.926424 rad-0.19.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-08 20:40:20.000000 rad-0.19.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 20:40:20.000000 rad-0.19.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.898424 rad-0.19.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 20:40:20.000000 rad-0.19.4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-08 20:40:20.000000 rad-0.19.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 20:40:20.000000 rad-0.19.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-08 20:40:20.000000 rad-0.19.4/docs/creating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 20:40:20.000000 rad-0.19.4/docs/ground_tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-08 20:40:20.000000 rad-0.19.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-08 20:40:20.000000 rad-0.19.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 20:40:20.000000 rad-0.19.4/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 20:40:20.000000 rad-0.19.4/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-08 20:40:20.000000 rad-0.19.4/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-08 20:40:20.000000 rad-0.19.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-08 20:40:20.000000 rad-0.19.4/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-05-08 20:40:20.000000 rad-0.19.4/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:40:30.926424 rad-0.19.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.898424 rad-0.19.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/src/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.910424 rad-0.19.4/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.910424 rad-0.19.4/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.918424 rad-0.19.4/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/base_exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/fps-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ground_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tvac-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 20:40:20.000000 rad-0.19.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-08 20:40:20.000000 rad-0.19.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.716598 rad-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 15:55:19.000000 rad-0.20.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.688598 rad-0.20.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-15 15:55:19.000000 rad-0.20.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-15 15:55:19.000000 rad-0.20.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.688598 rad-0.20.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 15:55:19.000000 rad-0.20.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-15 15:55:19.000000 rad-0.20.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 15:55:19.000000 rad-0.20.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 15:55:19.000000 rad-0.20.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 15:55:19.000000 rad-0.20.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 15:55:19.000000 rad-0.20.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-15 15:55:19.000000 rad-0.20.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 15:55:19.000000 rad-0.20.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-05-15 15:55:19.000000 rad-0.20.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-15 15:55:19.000000 rad-0.20.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-15 15:55:19.000000 rad-0.20.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-15 15:55:19.000000 rad-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:19.000000 rad-0.20.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-15 15:55:30.716598 rad-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-15 15:55:19.000000 rad-0.20.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.692598 rad-0.20.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-15 15:55:19.000000 rad-0.20.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.692598 rad-0.20.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 15:55:19.000000 rad-0.20.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-05-15 15:55:19.000000 rad-0.20.0/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.684598 rad-0.20.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.692598 rad-0.20.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 15:55:19.000000 rad-0.20.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 15:55:19.000000 rad-0.20.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 15:55:19.000000 rad-0.20.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 15:55:19.000000 rad-0.20.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-15 15:55:19.000000 rad-0.20.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 15:55:19.000000 rad-0.20.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-15 15:55:19.000000 rad-0.20.0/docs/creating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 15:55:19.000000 rad-0.20.0/docs/ground_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-15 15:55:19.000000 rad-0.20.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-15 15:55:19.000000 rad-0.20.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 15:55:19.000000 rad-0.20.0/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 15:55:19.000000 rad-0.20.0/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 15:55:19.000000 rad-0.20.0/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-15 15:55:19.000000 rad-0.20.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.692598 rad-0.20.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-15 15:55:19.000000 rad-0.20.0/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-05-15 15:55:19.000000 rad-0.20.0/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:55:30.716598 rad-0.20.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.684598 rad-0.20.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.692598 rad-0.20.0/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.696598 rad-0.20.0/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.696598 rad-0.20.0/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22827 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.704598 rad-0.20.0/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.704598 rad-0.20.0/src/rad/resources/schemas/fps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/ref_file-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/statistics-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.704598 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/fps-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.708598 rad-0.20.0/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.708598 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/target-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.712598 rad-0.20.0/src/rad/resources/schemas/tvac/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/ref_file-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/statistics-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.712598 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/tvac-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 15:55:19.000000 rad-0.20.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.716598 rad-0.20.0/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 15:55:30.000000 rad-0.20.0/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:30.716598 rad-0.20.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:19.000000 rad-0.20.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 15:55:19.000000 rad-0.20.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 15:55:19.000000 rad-0.20.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-15 15:55:19.000000 rad-0.20.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-15 15:55:19.000000 rad-0.20.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 15:55:19.000000 rad-0.20.0/tox.ini
```

### Comparing `rad-0.19.4/.github/pull_request_template.md` & `rad-0.20.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/.github/workflows/changelog.yml` & `rad-0.20.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/.github/workflows/ci_cron.yml` & `rad-0.20.0/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/.github/workflows/release.yml` & `rad-0.20.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/.gitignore` & `rad-0.20.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/.pre-commit-config.yaml` & `rad-0.20.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/CHANGES.rst` & `rad-0.20.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-0.20.0 (unreleased)
+0.20.1 (unreleased)
 -------------------
 
-- 
+-
+
+0.20.0 (2024-05-15)
+-------------------
+
+- This PR removes reference file and guidewindow db tables from cal_step schemas. [#420]
+
+- Separated TVAC and FPS schemas into their own suite of files. [#414]
+
+- Fixed the TVAC & FPS archive catalog destinations. [#424]
+
+- Added statistics schemas to both FPS and TVAC. [#423]
+
+- Removed filepath_level_pnt5 from TVAC/FPS database. [#422]
+
+- Removed the db entries for filename_l1a and filename_pnt5 in TVAC and FPS schemas. [#421]
+
 
 0.19.4 (2024-05-08)
 -------------------
 
 - Updated RTD with documentation for new data products. [#419]
 
+
 0.19.3 (2024-04-25)
 -------------------
 
 - Duplicated the keywords from groundtest to tvac_groundtest. [#409]
 
 
 0.19.2 (2024-04-17)
```

### Comparing `rad-0.19.4/CODE_OF_CONDUCT.md` & `rad-0.20.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/LICENSE` & `rad-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/PKG-INFO` & `rad-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.4
+Version: 0.20.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.4/README.md` & `rad-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/Makefile` & `rad-0.20.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/_static/custom.css` & `rad-0.20.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/_static/stsci_logo.png` & `rad-0.20.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/conf.py` & `rad-0.20.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/creating.rst` & `rad-0.20.0/docs/creating.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/ground_tests.rst` & `rad-0.20.0/docs/ground_tests.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/index.rst` & `rad-0.20.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/make.bat` & `rad-0.20.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/reference_files.rst` & `rad-0.20.0/docs/reference_files.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/docs/schemas.rst` & `rad-0.20.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/pyproject.toml` & `rad-0.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/scripts/insert_next_release.py` & `rad-0.20.0/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/scripts/set_release_date.py` & `rad-0.20.0/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/integration.py` & `rad-0.20.0/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.20.0/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -151,45 +151,14 @@
   description: |-
     Mosaic associations metadata keywords
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/mosaic_wcsinfo-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/mosaic_wcsinfo-1.0.0
   title: Mosaic WCS parameters
   description: |-
     Mosaic WCS parameters
-# Ground Modules
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/base_exposure-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/base_exposure-1.0.0
-  title: Exposure information
-  description: |-
-    Ground test exposure information
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/base_guidestar-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/base_guidestar-1.0.0
-  title: Guidestar information
-  description: |-
-    Guidestar information
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/groundtest-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/groundtest-1.0.0
-  title: Ground Test Information
-  description: |-
-    Ground test description.
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac_groundtest-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac_groundtest-1.0.0
-  title: TVAC Ground Test Information
-  description: |-
-    TVAC ground test description.
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps-1.0.0
-  title: FPS schema
-  description: |-
-    FPS test data
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac-1.0.0
-  title: TVAC schema
-  description: |-
-    TVAC test data
 # Reference Modules
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/dark-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
   title: Dark reference schema
   description: |-
     Dark reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/distortion-1.0.0
@@ -330,14 +299,178 @@
   description: |-
     SDF software version number
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tagged_scalars/telescope-1.0.0
   title: Telescope used to acquire the data
   description: |-
     Telescope used to acquire the data
+# FPS Schemas
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps-1.0.0
+  title: FPS schema
+  description: |-
+    FPS test data
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/cal_step-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/cal_step-1.0.0
+  title: FPS Level 2 Calibration Step status information
+  description: |-
+    FPS Level 2 Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/exposure-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/exposure-1.0.0
+  title: FPS Exposure information
+  description: |-
+    FPS Exposure information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/groundtest-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/groundtest-1.0.0
+  title: FPS Ground Test Information
+  description: |-
+    FPS Ground test description.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/guidestar-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/guidestar-1.0.0
+  title: FPS Guidestar information
+  description: |-
+    FPS Guidestar information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/statistics-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/statistics-1.0.0
+  title: FPS Summary Statistics
+  description: |-
+    FPS Summary Statistics
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/ref_file-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/ref_file-1.0.0
+  title: FPS Calibration reference file names.
+  description: |-
+    FPS Calibration reference file names.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/wfi_mode-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/wfi_mode-1.0.0
+  title: FPS Roman WFI Instrument Mode
+  description: |-
+    FPS Roman WFI Instrument
+# FPS Tagged Scalars
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/calibration_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/calibration_software_version-1.0.0
+  title: FPS Calibration software version
+  description: |-
+    FPS Calibration software version number
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/filename-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/filename-1.0.0
+  title: FPS Name of the file
+  description: |-
+    FPS Name of the file
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/file_date-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/file_date-1.0.0
+  title: FPS Date this file was created (UTC)
+  description: |-
+    FPS Date this file was created (UTC)
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/model_type-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/model_type-1.0.0
+  title: FPS Type of data model
+  description: |-
+    FPS Type of data model
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/origin-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/origin-1.0.0
+  title: FPS Organization responsible for creating file
+  description: |-
+    FPS Organization responsible for creating file
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/prd_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/prd_software_version-1.0.0
+  title: FPS S&OC PRD version number used in data processing
+  description: |-
+    FPS S&OC PRD version number used in data processing
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/sdf_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/sdf_software_version-1.0.0
+  title: FPS SDF software version number
+  description: |-
+    FPS SDF software version number
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps/telescope-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps/tagged_scalars/telescope-1.0.0
+  title: FPS Telescope used to acquire the data
+  description: |-
+    FPS Telescope used to acquire the data
+# TVAC Schemas
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac-1.0.0
+  title: TVAC schema
+  description: |-
+    TVAC test data
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/cal_step-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/cal_step-1.0.0
+  title: TVAC Level 2 Calibration Step status information
+  description: |-
+    TVAC Level 2 Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/exposure-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/exposure-1.0.0
+  title: TVAC Exposure information
+  description: |-
+    TVAC Exposure information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/groundtest-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/groundtest-1.0.0
+  title: TVAC Ground Test Information
+  description: |-
+    TVAC Ground test description.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/guidestar-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/guidestar-1.0.0
+  title: TVAC Guidestar information
+  description: |-
+    TVAC Guidestar information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/statistics-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/statistics-1.0.0
+  title: TVAC Summary Statistics
+  description: |-
+    TVAC Summary Statistics
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/ref_file-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/ref_file-1.0.0
+  title: TVAC Calibration reference file names.
+  description: |-
+    TVAC Calibration reference file names.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/wfi_mode-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/wfi_mode-1.0.0
+  title: TVAC Roman WFI Instrument Mode
+  description: |-
+    TVAC Roman WFI Instrument
+# TVAC Tagged Scalars
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/calibration_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/calibration_software_version-1.0.0
+  title: TVAC Calibration software version
+  description: |-
+    TVAC Calibration software version number
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/filename-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/filename-1.0.0
+  title: TVAC Name of the file
+  description: |-
+    TVAC Name of the file
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/file_date-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/file_date-1.0.0
+  title: TVAC Date this file was created (UTC)
+  description: |-
+    TVAC Date this file was created (UTC)
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/model_type-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/model_type-1.0.0
+  title: TVAC Type of data model
+  description: |-
+    TVAC Type of data model
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/origin-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/origin-1.0.0
+  title: TVAC Organization responsible for creating file
+  description: |-
+    TVAC Organization responsible for creating file
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/prd_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/prd_software_version-1.0.0
+  title: TVAC S&OC PRD version number used in data processing
+  description: |-
+    TVAC S&OC PRD version number used in data processing
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/sdf_software_version-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/sdf_software_version-1.0.0
+  title: TVAC SDF software version number
+  description: |-
+    TVAC SDF software version number
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac/telescope-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac/tagged_scalars/telescope-1.0.0
+  title: TVAC Telescope used to acquire the data
+  description: |-
+    TVAC Telescope used to acquire the data
 # SSC data models
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/msos_stack-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/msos_stack-1.0.0
   title: MSOS Stack Level 3 Schema
   description: |-
     Level 3 schema for SSC's MSOS stack products
 ...
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/base_exposure-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tvac/exposure-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/base_exposure-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/tvac/exposure-1.0.0
 
 
 title: |
-  Base Exposure Information
+  TVAC Base Exposure Information
 
 type: object
 properties:
   type:
-    $ref: asdf://stsci.edu/datamodels/roman/schemas/exposure_type-1.0.0
+    $ref: asdf://stsci.edu/datamodels/roman/schemas/tvac/exposure_type-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(25)
-      destination: [WFIExposure.exposure_type, GuideWindow.exposure_type, WFICommon.exposure_type]
+      destination: [WFICommon.exposure_type]
   start_time:
     title: Exposure Start Time (UTC)
     description: |
       The UTC time at the beginning of the exposure.
     tag: tag:stsci.edu:asdf/time/time-1.*
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [WFIExposure.exposure_start_time, GuideWindow.exposure_start_time, WFICommon.exposure_start_time]
+      destination: [WFICommon.exposure_start_time]
   ngroups:
     title: Number of Resultants
     description: |
       The number of resultant frames in this exposure that were transmitted to
       the ground. The number of integrations of WFI data is always 1.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.exposure_ngroups, GuideWindow.exposure_ngroups, WFICommon.exposure_ngroups]
+      destination: [WFICommon.exposure_ngroups]
   nframes:
     title: Number of Reads
     description: |
       This is the number of science frames that are combined to produce a resultant frame.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.exposure_nframes, GuideWindow.exposure_nframes, WFICommon.exposure_nframes]
+      destination: [WFICommon.exposure_nframes]
   data_problem:
     title: Data Problem
     description: |
       A flag indicating an issue with science telemetry.
     type: boolean
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nchar(1)
-      destination: [WFIExposure.exposure_data_problem, GuideWindow.exposure_data_problem, WFICommon.exposure_data_problem]
+      destination: [WFICommon.exposure_data_problem]
   frame_divisor:
     title: Frame Divisor
     description: |
       The number of reads averaged to calculate a resultant. Value depends on
       the readout pattern used from the MultiAccum table.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.exposure_frame_divisor, GuideWindow.exposure_frame_divisor, WFICommon.exposure_frame_divisor]
+      destination: [WFICommon.exposure_frame_divisor]
   groupgap:
     title: Number of Frames Dropped Between Resultants
     description:
       The number of reads that are dropped, or not used to calculate a
       resultant.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.exposure_groupgap, GuideWindow.exposure_groupgap, WFICommon.exposure_groupgap]
+      destination: [WFICommon.exposure_groupgap]
   frame_time:
     title: Time Between Reads (s)
     description: |
       The amount of time elapsed between the end of one read and the beginning
       of the next.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [WFIExposure.exposure_frame_time, GuideWindow.exposure_frame_time, WFICommon.exposure_frame_time]
+      destination: [WFICommon.exposure_frame_time]
   group_time:
     title: Time Between Resultants (s)
     description: |
       The time that is the sum of the reads that are used to construct a
       resultant. This will depend on the MA table being used.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [WFIExposure.exposure_group_time, GuideWindow.exposure_group_time, WFICommon.exposure_group_time]
+      destination: [WFICommon.exposure_group_time]
   exposure_time:
     title: Exposure Time (s)
     description: |
       The time between the start of the first Reset/Read Science Frame of an
       Exposure and the completion of the final Read Only Science Frame of that
       Exposure.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [WFIExposure.exposure_time, GuideWindow.exposure_time, WFICommon.exposure_time]
+      destination: [WFICommon.exposure_time]
   ma_table_name:
     title: MA Table Name
     description: |
       The name of the MultiAccum table used for this exposure, as defined in the
       Project Reference Database.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [WFIExposure.ma_table_name, GuideWindow.ma_table_name, WFICommon.ma_table_name]
+      destination: [WFICommon.ma_table_name]
   ma_table_number:
     title: MA Table Number
     description: |
       The number of the MultiAccum table used for this exposure. Used in
       matching exposures to their corresponding calibration data.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [WFIExposure.ma_table_number, GuideWindow.ma_table_number, WFICommon.ma_table_number]
+      destination: [WFICommon.ma_table_number]
   read_pattern:
     title: Read Pattern
     description: |
       Enumeration of detector reads to resultants making up the L1 data
       downlinked from the observatory.
     type: array
     items:
@@ -171,15 +171,15 @@
         type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(3500)
-      destination: [WFIExposure.read_pattern, GuideWindow.read_pattern, WFICommon.read_pattern]
+      destination: [WFICommon.read_pattern]
 propertyOrder: [type, start_time,
            ngroups, nframes, data_problem,
            frame_divisor, groupgap, frame_time, group_time, exposure_time,
            ma_table_name, ma_table_number, read_pattern]
 flowStyle: block
 required: [type, start_time,
            ngroups, nframes, data_problem,
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/base_guidestar-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/fps/guidestar-1.0.0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,140 +1,140 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/base_guidestar-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/fps/guidestar-1.0.0
 
-title: Base Guide star window information
+title: FPS Base Guide star window information
 type: object
 properties:
   gw_id:
     title: Guide Star Window Identifier
     description: |
       Identification of the Guide Star Window.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(20)
-      destination: [WFIExposure.gw_id, GuideWindow.gw_id, WFICommon.gw_id]
+      destination: [WFICommon.gw_id]
   gw_fgs_mode:
     $ref: guidewindow_modes-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(18)
-      destination: [WFIExposure.gw_fgs_mode, GuideWindow.gw_fgs_mode, WFICommon.gw_fgs_mode]
+      destination: [WFICommon.gw_fgs_mode]
   data_start:
     title: Guide Data Start Time (MJD)
     description: |
       Start time of the guide window data taken for this exposure as a Modified
       Julian Date.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [WFIExposure.data_start, GuideWindow.data_start, WFICommon.data_start]
+      destination: [WFICommon.data_start]
   data_end:
     title: Guide Data End Time (MJD)
     description: |
       End time of the guide window data taken for this exposure as a Modified
       Julian Date.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [WFIExposure.data_end, GuideWindow.data_end, WFICommon.data_end]
+      destination: [WFICommon.data_end]
   gw_window_xstart:
     title: Guide Window X Start Position (pixels)
     description: |
       Minimum X position in the science coordinate frame of all tracking guide
       windows in this exposure measured in pixels.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_xstart, WFICommon.gw_window_xstart]
+      destination: [WFICommon.gw_window_xstart]
   gw_window_ystart:
     title: Guide Window Y Start Position (pixels)
     description: |
       Minimum Y position in the science coordinate frame of all tracking guide
       windows in this exposure measured in pixels.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_ystart, WFICommon.gw_window_ystart]
+      destination: [WFICommon.gw_window_ystart]
   gw_window_xstop:
     title: Guide Window X Stop Position (pixels)
     description: |
       Maximum X position in the science coordinate frame of all tracking guide
       windows in this exposure measured in pixels.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_xstop, WFICommon.gw_window_xstop]
+      destination: [WFICommon.gw_window_xstop]
   gw_window_ystop:
     title: Guide Window Y Stop Position (pixels)
     description: |
       Maximum Y position in the science coordinate frame of all tracking guide
       windows in this exposure measured in pixels
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_ystop, WFICommon.gw_window_ystop]
+      destination: [WFICommon.gw_window_ystop]
   gw_window_xsize:
     title: Guide Window Size in the X Direction (pixels)
     description: |
       Size of a single tracking guide window in this exposure measured along the
       X axis in units of pixels.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_xsize, WFICommon.gw_window_xsize]
+      destination: [WFICommon.gw_window_xsize]
   gw_window_ysize:
     title: Guide Window Size in the Y Direction (pixels)
     description: |
       Size of a single tracking guide window in this exposure measured along the
       Y axis in units of pixels.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Science Data Formatting
     archive_catalog:
       datatype: int
-      destination: [WFIExposure.gw_window_ysize, WFICommon.gw_window_ysize]
+      destination: [WFICommon.gw_window_ysize]
 
 propertyOrder: [gw_id, gw_fgs_mode,
                data_start, data_end, gw_window_xstart,
                gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
                gw_window_ysize]
 flowStyle: block
 required: [gw_id, gw_fgs_mode,
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/exposure_type-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/fps-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/fps-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 archive_meta: None
 
 type: object
 properties:
   meta:
     allOf:
-      - $ref: asdf://stsci.edu/datamodels/roman/schemas/ground_common-1.0.0
+      - $ref: asdf://stsci.edu/datamodels/roman/schemas/fps/common-1.0.0
       - type: object
         properties:
           groundtest:
-            tag: asdf://stsci.edu/datamodels/roman/tags/groundtest-1.0.0
+            tag: asdf://stsci.edu/datamodels/roman/tags/fps/groundtest-1.0.0
         required: [groundtest]
 
   data:
     title: Science data, including the border reference pixels.
     tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/ground_common-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tvac/common-1.0.0.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/ground_common-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/tvac/common-1.0.0
 
-title: Common metadata properties
+title: TVAC Common metadata properties
 
 allOf:
 # Meta Variables
-- $ref: asdf://stsci.edu/datamodels/roman/schemas/basic-1.0.0
+- $ref: asdf://stsci.edu/datamodels/roman/schemas/tvac/basic-1.0.0
 - type: object
   properties:
     # Meta Objects
     cal_step:
-      tag: asdf://stsci.edu/datamodels/roman/tags/l2_cal_step-1.0.0
+      tag: asdf://stsci.edu/datamodels/roman/tags/tvac/cal_step-1.0.0
     exposure:
-      tag: asdf://stsci.edu/datamodels/roman/tags/base_exposure-1.0.0
+      tag: asdf://stsci.edu/datamodels/roman/tags/tvac/exposure-1.0.0
     guidestar:
-      tag: asdf://stsci.edu/datamodels/roman/tags/base_guidestar-1.0.0
+      tag: asdf://stsci.edu/datamodels/roman/tags/tvac/guidestar-1.0.0
     instrument:
-      tag: asdf://stsci.edu/datamodels/roman/tags/wfi_mode-1.0.0
+      tag: asdf://stsci.edu/datamodels/roman/tags/tvac/wfi_mode-1.0.0
     ref_file:
-      tag: asdf://stsci.edu/datamodels/roman/tags/ref_file-1.0.0
+      tag: asdf://stsci.edu/datamodels/roman/tags/tvac/ref_file-1.0.0
     hdf5_meta:
       title: Original Raw HDF5 metadata
       type: object
     hdf5_telemetry:
       title: Original Raw HDF5 telemetry keywords
       type: string
     gw_meta:
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/groundtest-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/fps/groundtest-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/groundtest-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/fps/groundtest-1.0.0
 
-title: Ground Test Information
+title: FPS Ground Test Information
 type: object
 properties:
   test_name:
     title: I&T Test Name
     type: string
     archive_catalog:
       datatype: nvarchar(80)
@@ -53,29 +53,20 @@
     type: string
     archive_catalog:
       datatype: nvarchar(80)
       destination: [WFICommon.conversion_version]
   filename_pnt5:
     title: L0.5 File Name
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filename_pnt5]
   filepath_level_pnt5:
     title: L0.5 File Path
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filepath_level_pnt5]
   filename_l1a:
     title: L1A File Name
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filename_l1a]
   detector_id:
     title: SCA Identifier
     type: string
     archive_catalog:
       datatype: nvarchar(80)
       destination: [WFICommon.detector_id]
   detector_temp:
@@ -122,15 +113,14 @@
         enum: ["cm"]
   sensor_error:
     title: Sensor Error
     tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float64
     exact_datatype: true
     # needs ndim
-
 propertyOrder: [test_name, test_phase, test_environment, test_script,
                 product_date, product_version, conversion_date, conversion_version,
                 filename_pnt5, filepath_level_pnt5, filename_l1a, detector_id,
                 detector_temp, frames_temp, ota_temp, rcs_on, readout_col_num,
                 detector_pixel_size, sensor_error]
 flowStyle: block
 required: [test_name, test_phase, test_environment, test_script,
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/fps/cal_step-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,167 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/l2_cal_step-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/fps/cal_step-1.0.0
 
-title: Level 2 Calibration Status
+title: FPS Level 2 Calibration Status
 type: object
 properties:
   assign_wcs:
     title: Assign WCS Step
     description: |
       Step in ROMANCAL that assigns a World Coordinate System (WCS) object to a
       science image.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_assign_wcs, GuideWindow.s_assign_wcs, WFICommon.s_assign_wcs]
+      destination: [WFICommon.s_assign_wcs]
   flat_field:
     title: Flat Fielding Step
     descroption: |
       Step in ROMANCAL in which a science image is flat-fielded, whereby each
       detector pixel is calibrated to give the same signal for the same
       illumination, given its specific response. This is achieved using a
       flatfield reference image.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_flat_field, GuideWindow.s_flat_field, WFICommon.s_flat_field]
+      destination: [WFICommon.s_flat_field]
   dark:
     title: Dark Current Subtraction Step
     description: |
       Step in ROMANCAL performing the dark current correction by subtracting
       dark current reference data from science data.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_dark, GuideWindow.s_dark, WFICommon.s_dark]
+      destination: [WFICommon.s_dark]
   dq_init:
     title: Initialization of the Data Quality Extension Step
     description: |
       Step in ROMANCAL in which the pixeldq attribute of the input data model
       using the MASK reference file is initialized.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_dq_init, GuideWindow.s_dq_init, WFICommon.s_dq_init]
+      destination: [WFICommon.s_dq_init]
   flux:
     title: Flux Scale Application Step
     description: |
       Step in ROMANCAL which applies the scaling factors determined in the Photom calibrations step.
       The data are converted from DN/s to MJy/sr.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_flux, GuideWindow.s_flux, WFICommon.s_flux]
+      destination: [WFICommon.s_flux]
   jump:
     title: Cosmic Rays and Jump Detection Step
     description: |
       Step in ROMANCAL which performs a search for jumps in values in ramp that
       may be associated with cosmic rays.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_jump, GuideWindow.s_jump, WFICommon.s_jump]
+      destination: [WFICommon.s_jump]
   linearity:
     title: Linearity Correction Step
     description: |
       Step in ROMANCAL which performs a correction for the classical non-linear
       detector response.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_linearity, GuideWindow.s_linearity, WFICommon.s_linearity]
+      destination: [WFICommon.s_linearity]
   photom:
     title: Photometric Calibration Step
     description: |
       Step in ROMANCAL that adds photometric calibrations to the metadata of a
       data product.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_photom, GuideWindow.s_photom, WFICommon.s_photom]
+      destination: [WFICommon.s_photom]
   source_detection:
     title: Source Detection Step
     description: |
       Step in ROMANCAL to detect point sources in an image and catalog them.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_source_detection, GuideWindow.s_source_detection, WFICommon.s_source_detection]
+      destination: [WFICommon.s_source_detection]
   ramp_fit:
     title: Ramp Fit Step
     description: |
       Step in ROMANCAL to fit the counts versus time with a straight line and
       thus estimate the count rate for each pixel.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_ramp_fit, GuideWindow.s_ramp_fit, WFICommon.s_ramp_fit]
+      destination: [WFICommon.s_ramp_fit]
   refpix:
     title: Reference Pixel Correction Step
     description: |
       Step in ROMANCAL that corrects for additional signal from electronics
       contributing to (e.g. 1/f noise) using the reference pixels.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_refpix, GuideWindow.s_refpix, WFICommon.s_refpix]
+      destination: [WFICommon.s_refpix]
   saturation:
     title: Saturation Identification Step
     description: |
       Step in ROMANCAL which sets pixel flags to label that a pixel is at or
       above the saturation threshold. As part of this step, pixels that are zero
       or negative are also flagged.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_saturation, GuideWindow.s_saturation, WFICommon.s_saturation]
+      destination: [WFICommon.s_saturation]
   outlier_detection:
     title: Outlier Detection Step
     description: |
       Step in ROMANCAL which detects and flags outliers in a science image.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_outlier_detection, GuideWindow.s_outlier_detection, WFICommon.s_outlier_detection]
+      destination: [WFICommon.s_outlier_detection]
   tweakreg:
     title: Tweakreg step
     description: |
       Step in ROMANCAL that compares positions of point-like sources with
       coordinates from a Gaia catalog, and, if necessary, corrects an image's
       World Coordinate System alignment.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_tweakreg, GuideWindow.s_tweakreg, WFICommon.s_tweakreg]
+      destination: [WFICommon.s_tweakreg]
   skymatch:
     title: Sky Matching for Combining Overlapping Images Step
     description: |
       Step in ROMANCAL that computes sky background values of each input image
       and derives scalings to equalize overlapping regions.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_skymatch, GuideWindow.s_skymatch, WFICommon.s_skymatch]
+      destination: [WFICommon.s_skymatch]
 propertyOrder: [assign_wcs, flat_field, flux, dark, dq_init, jump, linearity, photom, source_detection,
                 outlier_detection, ramp_fit, refpix, saturation, skymatch, tweakreg]
 flowStyle: block
 required: [assign_wcs, flat_field, flux, dark, dq_init, jump, linearity, outlier_detection, photom,
            source_detection, ramp_fit, refpix, saturation, skymatch, tweakreg]
 additionalProperties: true
 ...
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -11,43 +11,43 @@
     description: |
       Step in ROMANCAL which applies the scaling factors determined in the Photom calibrations step.
       The data are converted from DN/s to MJy/sr.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_flux, GuideWindow.s_flux, WFIMosaic.s_flux]
+      destination: [ScienceRefData.s_flux]
   outlier_detection:
     title: Outlier Detection Step
     description: |
       Step in ROMANCAL which detects and flags outliers in a science image.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_outlier_detection, GuideWindow.s_outlier_detection, WFIMosaic.s_outlier_detection]
+      destination: [ScienceRefData.s_outlier_detection]
   skymatch:
     title: Sky Matching for Combining Overlapping Images Step
     description: |
       Step in ROMANCAL that computes sky background values of each input image
       and derives scalings to equalize overlapping regions.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_skymatch, GuideWindow.s_skymatch, WFIMosaic.s_skymatch]
+      destination: [ScienceRefData.s_skymatch]
   resample:
     title: Resampling Input Data onto a Regular Grid Step
     description: |
       Step in ROMANCAL which resamples each input 2D image based on its WCS and
       WCS distortion information on a grid that allows the combination of
       multiple resampled images into a single, undistorted product.
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.s_resample, GuideWindow.s_resample, WFIMosaic.s_resample]
+      destination: [ScienceRefData.s_resample]
 propertyOrder: [flux, outlier_detection, skymatch, resample]
 flowStyle: block
 required: [flux, outlier_detection, resample, skymatch]
 additionalProperties: true
 ...
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/segmentation_map-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/source_catalog-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/tvac-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tvac-1.0.0.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 archive_meta: None
 
 type: object
 properties:
   meta:
     allOf:
-      - $ref: asdf://stsci.edu/datamodels/roman/schemas/ground_common-1.0.0
+      - $ref: asdf://stsci.edu/datamodels/roman/schemas/tvac/common-1.0.0
       - type: object
         properties:
           groundtest:
-            tag: asdf://stsci.edu/datamodels/roman/tags/tvac_groundtest-1.0.0
+            tag: asdf://stsci.edu/datamodels/roman/tags/tvac/groundtest-1.0.0
         required: [groundtest]
 
   data:
     title: Science data, including the border reference pixels.
     tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/tvac/groundtest-1.0.0.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/tvac_groundtest-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/tvac/groundtest-1.0.0
 
 title: TVAC Ground Test Information
 type: object
 properties:
   test_name:
     title: I&T Test Name
     type: string
@@ -53,29 +53,20 @@
     type: string
     archive_catalog:
       datatype: nvarchar(80)
       destination: [WFICommon.conversion_version]
   filename_pnt5:
     title: L0.5 File Name
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filename_pnt5]
   filepath_level_pnt5:
     title: L0.5 File Path
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filepath_level_pnt5]
   filename_l1a:
     title: L1A File Name
     type: string
-    archive_catalog:
-      datatype: nvarchar(80)
-      destination: [WFICommon.filename_l1a]
   detector_id:
     title: SCA Identifier
     type: string
     archive_catalog:
       datatype: nvarchar(80)
       destination: [WFICommon.detector_id]
   detector_temp:
```

### Comparing `rad-0.19.4/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.20.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/src/rad.egg-info/PKG-INFO` & `rad-0.20.0/src/rad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.4
+Version: 0.20.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.4/src/rad.egg-info/SOURCES.txt` & `rad-0.20.0/src/rad.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -44,26 +44,22 @@
 src/rad.egg-info/entry_points.txt
 src/rad.egg-info/requires.txt
 src/rad.egg-info/top_level.txt
 src/rad/resources/__init__.py
 src/rad/resources/manifests/datamodels-1.0.yaml
 src/rad/resources/schemas/aperture-1.0.0.yaml
 src/rad/resources/schemas/associations-1.0.0.yaml
-src/rad/resources/schemas/base_exposure-1.0.0.yaml
-src/rad/resources/schemas/base_guidestar-1.0.0.yaml
 src/rad/resources/schemas/basic-1.0.0.yaml
 src/rad/resources/schemas/cal_logs-1.0.0.yaml
 src/rad/resources/schemas/common-1.0.0.yaml
 src/rad/resources/schemas/coordinates-1.0.0.yaml
 src/rad/resources/schemas/ephemeris-1.0.0.yaml
 src/rad/resources/schemas/exposure-1.0.0.yaml
 src/rad/resources/schemas/exposure_type-1.0.0.yaml
 src/rad/resources/schemas/fps-1.0.0.yaml
-src/rad/resources/schemas/ground_common-1.0.0.yaml
-src/rad/resources/schemas/groundtest-1.0.0.yaml
 src/rad/resources/schemas/guidestar-1.0.0.yaml
 src/rad/resources/schemas/guidewindow-1.0.0.yaml
 src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
 src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
 src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
 src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
 src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
@@ -83,24 +79,44 @@
 src/rad/resources/schemas/ref_file-1.0.0.yaml
 src/rad/resources/schemas/resample-1.0.0.yaml
 src/rad/resources/schemas/segmentation_map-1.0.0.yaml
 src/rad/resources/schemas/source_catalog-1.0.0.yaml
 src/rad/resources/schemas/source_detection-1.0.0.yaml
 src/rad/resources/schemas/target-1.0.0.yaml
 src/rad/resources/schemas/tvac-1.0.0.yaml
-src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
 src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
 src/rad/resources/schemas/visit-1.0.0.yaml
 src/rad/resources/schemas/wcsinfo-1.0.0.yaml
 src/rad/resources/schemas/wfi_detector-1.0.0.yaml
 src/rad/resources/schemas/wfi_image-1.0.0.yaml
 src/rad/resources/schemas/wfi_mode-1.0.0.yaml
 src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
 src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
 src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+src/rad/resources/schemas/fps/basic-1.0.0.yaml
+src/rad/resources/schemas/fps/cal_step-1.0.0.yaml
+src/rad/resources/schemas/fps/common-1.0.0.yaml
+src/rad/resources/schemas/fps/exposure-1.0.0.yaml
+src/rad/resources/schemas/fps/exposure_type-1.0.0.yaml
+src/rad/resources/schemas/fps/groundtest-1.0.0.yaml
+src/rad/resources/schemas/fps/guidestar-1.0.0.yaml
+src/rad/resources/schemas/fps/guidewindow_modes-1.0.0.yaml
+src/rad/resources/schemas/fps/ref_file-1.0.0.yaml
+src/rad/resources/schemas/fps/statistics-1.0.0.yaml
+src/rad/resources/schemas/fps/wfi_detector-1.0.0.yaml
+src/rad/resources/schemas/fps/wfi_mode-1.0.0.yaml
+src/rad/resources/schemas/fps/wfi_optical_element-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/calibration_software_version-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/file_date-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/filename-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/model_type-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/origin-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/prd_software_version-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/sdf_software_version-1.0.0.yaml
+src/rad/resources/schemas/fps/tagged_scalars/telescope-1.0.0.yaml
 src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
 src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
 src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
 src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
 src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
 src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
@@ -118,12 +134,33 @@
 src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+src/rad/resources/schemas/tvac/basic-1.0.0.yaml
+src/rad/resources/schemas/tvac/cal_step-1.0.0.yaml
+src/rad/resources/schemas/tvac/common-1.0.0.yaml
+src/rad/resources/schemas/tvac/exposure-1.0.0.yaml
+src/rad/resources/schemas/tvac/exposure_type-1.0.0.yaml
+src/rad/resources/schemas/tvac/groundtest-1.0.0.yaml
+src/rad/resources/schemas/tvac/guidestar-1.0.0.yaml
+src/rad/resources/schemas/tvac/guidewindow_modes-1.0.0.yaml
+src/rad/resources/schemas/tvac/ref_file-1.0.0.yaml
+src/rad/resources/schemas/tvac/statistics-1.0.0.yaml
+src/rad/resources/schemas/tvac/wfi_detector-1.0.0.yaml
+src/rad/resources/schemas/tvac/wfi_mode-1.0.0.yaml
+src/rad/resources/schemas/tvac/wfi_optical_element-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/calibration_software_version-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/file_date-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/filename-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/model_type-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/origin-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/prd_software_version-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/sdf_software_version-1.0.0.yaml
+src/rad/resources/schemas/tvac/tagged_scalars/telescope-1.0.0.yaml
 tests/__init__.py
 tests/conftest.py
 tests/test_integration.py
 tests/test_manifest.py
 tests/test_schemas.py
```

### Comparing `rad-0.19.4/tests/test_integration.py` & `rad-0.20.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/tests/test_manifest.py` & `rad-0.20.0/tests/test_manifest.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,9 +26,13 @@
     # to a higher standard:
     assert "title" in entry
     assert "description" in entry
 
     # Check the URIs
     assert entry["tag_uri"].startswith("asdf://stsci.edu/datamodels/roman/tags/")
     uri_suffix = entry["tag_uri"].split("asdf://stsci.edu/datamodels/roman/tags/")[-1]
-    assert entry["schema_uri"].endswith(uri_suffix)
-    assert entry["schema_uri"].startswith("asdf://stsci.edu/datamodels/roman/schemas/")
+    # Remove tagged scalars from the uri string
+    schema_uri = entry["schema_uri"]
+    if "tagged_scalars" in schema_uri.split("/"):
+        schema_uri = schema_uri.replace("tagged_scalars/", "")
+    assert schema_uri.endswith(uri_suffix)
+    assert schema_uri.startswith("asdf://stsci.edu/datamodels/roman/schemas/")
```

### Comparing `rad-0.19.4/tests/test_schemas.py` & `rad-0.20.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.4/tox.ini` & `rad-0.20.0/tox.ini`

 * *Files identical despite different names*

