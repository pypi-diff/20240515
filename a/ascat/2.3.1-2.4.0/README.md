# Comparing `tmp/ascat-2.3.1.tar.gz` & `tmp/ascat-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascat-2.3.1.tar", last modified: Thu Jan 18 12:29:14 2024, max compression
+gzip compressed data, was "ascat-2.4.0.tar", last modified: Wed May 15 12:57:12 2024, max compression
```

## Comparing `ascat-2.3.1.tar` & `ascat-2.4.0.tar`

### file list

```diff
@@ -1,133 +1,147 @@
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:14.136089 ascat-2.3.1/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      588 2023-04-06 20:37:57.000000 ascat-2.3.1/.coveragerc
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.504090 ascat-2.3.1/.github/
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.540089 ascat-2.3.1/.github/workflows/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     2300 2023-11-05 00:05:21.000000 ascat-2.3.1/.github/workflows/ascat_ubuntu.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     1296 2023-11-05 00:05:21.000000 ascat-2.3.1/.github/workflows/ascat_windows.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      597 2023-10-30 10:28:59.000000 ascat-2.3.1/.github/workflows/upload_pypi.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      532 2023-04-06 20:37:57.000000 ascat-2.3.1/.gitignore
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      129 2023-10-30 10:28:59.000000 ascat-2.3.1/.gitmodules
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      795 2023-12-15 13:36:42.000000 ascat-2.3.1/.readthedocs.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      134 2023-04-06 20:37:57.000000 ascat-2.3.1/AUTHORS.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     3581 2024-01-18 12:25:44.000000 ascat-2.3.1/CHANGELOG.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     1074 2023-12-19 13:24:40.000000 ascat-2.3.1/LICENSE.txt
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     4519 2024-01-18 12:29:14.136089 ascat-2.3.1/PKG-INFO
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     3825 2023-12-15 13:36:42.000000 ascat-2.3.1/README.rst
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.660089 ascat-2.3.1/docs/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     1154 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/Makefile
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.660089 ascat-2.3.1/docs/_static/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)       18 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/_static/.gitignore
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    10772 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/ascat_bufr_format.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)       41 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/authors.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)       43 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/changelog.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     9714 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/conf.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      225 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/env.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     3821 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/examples.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     1387 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/index.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)       67 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/license.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    92416 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_cgls_swi_ts.ipynb
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     2654 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_cgls_swi_ts.rst
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.660089 ascat-2.3.1/docs/read_cgls_swi_ts_files/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    65951 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   578048 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_eumetsat.ipynb
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    35677 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_eumetsat.rst
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.712089 ascat-2.3.1/docs/read_eumetsat_files/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    99279 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_19_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   151416 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_5_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   151239 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_8_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   719257 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr.ipynb
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     5719 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr.rst
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.780089 ascat-2.3.1/docs/read_hsaf_cdr_files/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68510 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    77447 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    78359 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   162796 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    78897 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    65970 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)  1256504 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt.ipynb
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    11409 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt.rst
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.864089 ascat-2.3.1/docs/read_hsaf_nrt_files/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   173484 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   168175 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   165841 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   171571 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    33102 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    31452 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)   186561 2023-04-06 20:37:57.000000 ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)       39 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/readme.rst
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      233 2023-12-15 13:36:42.000000 ascat-2.3.1/docs/requirements.txt
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      219 2023-11-05 00:05:21.000000 ascat-2.3.1/environment.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      194 2023-11-05 00:05:21.000000 ascat-2.3.1/environment_win.yml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      346 2023-12-15 13:36:42.000000 ascat-2.3.1/pyproject.toml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     1405 2024-01-18 12:29:14.136089 ascat-2.3.1/setup.cfg
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      700 2023-12-15 13:36:42.000000 ascat-2.3.1/setup.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.504090 ascat-2.3.1/src/
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.884089 ascat-2.3.1/src/ascat/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      577 2023-12-15 13:36:42.000000 ascat-2.3.1/src/ascat/__init__.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     7019 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/cgls.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.884089 ascat-2.3.1/src/ascat/download/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    20661 2024-01-18 12:24:29.000000 ascat-2.3.1/src/ascat/download/connectors.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     8317 2023-12-15 14:35:53.000000 ascat-2.3.1/src/ascat/download/interface.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.884089 ascat-2.3.1/src/ascat/eumetsat/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)        0 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/eumetsat/__init__.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    17208 2023-11-05 00:05:21.000000 ascat-2.3.1/src/ascat/eumetsat/level1.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    12436 2023-11-05 00:05:21.000000 ascat-2.3.1/src/ascat/eumetsat/level2.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    29346 2023-12-19 13:14:57.000000 ascat-2.3.1/src/ascat/file_handling.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     9481 2023-11-05 00:05:21.000000 ascat-2.3.1/src/ascat/h_saf.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:13.884089 ascat-2.3.1/src/ascat/read_native/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)        0 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/__init__.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    21703 2023-11-05 00:05:21.000000 ascat-2.3.1/src/ascat/read_native/bufr.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    13374 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/cdr.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68901 2023-11-05 00:05:21.000000 ascat-2.3.1/src/ascat/read_native/eps_native.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:14.136089 ascat-2.3.1/src/ascat/read_native/formats/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      700 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/ccsds.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     5400 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps.dtd
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    67604 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps.xsl
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    34467 2023-10-30 10:28:59.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    63559 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    63563 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    66425 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    66555 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    39840 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    37290 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    36662 2023-10-30 10:28:59.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68252 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68256 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    71118 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    70852 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    44139 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    42894 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    36664 2023-10-30 10:28:59.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68252 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    68256 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    71118 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    70852 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    44137 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    42843 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    25967 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    32143 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    31812 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    25966 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    31948 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    31615 2023-04-06 20:37:57.000000 ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     9631 2023-10-30 10:28:59.000000 ascat-2.3.1/src/ascat/read_native/hdf5.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    18014 2023-10-30 10:28:59.000000 ascat-2.3.1/src/ascat/read_native/nc.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    14072 2023-12-15 15:10:16.000000 ascat-2.3.1/src/ascat/read_native/ragged_array_ts.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     8280 2023-11-28 15:43:14.000000 ascat-2.3.1/src/ascat/utils.py
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:14.136089 ascat-2.3.1/src/ascat.egg-info/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     4519 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/PKG-INFO
--rwx------   0 shahn    (1428007374) domain users (1428000513)     3950 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/SOURCES.txt
--rwx------   0 shahn    (1428007374) domain users (1428000513)        1 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/dependency_links.txt
--rwx------   0 shahn    (1428007374) domain users (1428000513)      144 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/entry_points.txt
--rwx------   0 shahn    (1428007374) domain users (1428000513)        1 2020-11-03 17:45:10.000000 ascat-2.3.1/src/ascat.egg-info/not-zip-safe
--rwx------   0 shahn    (1428007374) domain users (1428000513)       86 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/requires.txt
--rwx------   0 shahn    (1428007374) domain users (1428000513)        6 2024-01-18 12:29:13.000000 ascat-2.3.1/src/ascat.egg-info/top_level.txt
-drwxr-xr-x   0 shahn    (1428007374) domain users (1428000513)        0 2024-01-18 12:29:14.136089 ascat-2.3.1/tests/
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)      273 2023-12-15 13:36:42.000000 ascat-2.3.1/tests/conftest.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     3755 2023-10-30 10:28:59.000000 ascat-2.3.1/tests/test_cgls.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     4042 2023-04-06 20:37:57.000000 ascat-2.3.1/tests/test_download.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    19118 2023-10-30 10:28:59.000000 ascat-2.3.1/tests/test_file_handling.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    19572 2023-11-05 00:05:21.000000 ascat-2.3.1/tests/test_h_saf.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    20515 2023-11-05 00:05:21.000000 ascat-2.3.1/tests/test_level1.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)    17741 2023-11-05 00:05:21.000000 ascat-2.3.1/tests/test_level2.py
--rw-r--r--   0 shahn    (1428007374) domain users (1428000513)     2851 2023-12-15 13:36:42.000000 ascat-2.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 12:57:06.000000 ascat-2.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.550478 ascat-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.554479 ascat-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 12:57:06.000000 ascat-2.4.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 12:57:06.000000 ascat-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 12:57:06.000000 ascat-2.4.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 12:57:06.000000 ascat-2.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 12:57:06.000000 ascat-2.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-15 12:57:06.000000 ascat-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-15 12:57:06.000000 ascat-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-15 12:57:12.582479 ascat-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-15 12:57:06.000000 ascat-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/ascat_bufr_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/docs_env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    33620 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/org/xarray_readers_tutorial.org
+-rw-r--r--   0 runner    (1001) docker     (127)    92416 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.562478 ascat-2.4.0/docs/read_cgls_swi_ts_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    65951 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   578048 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.566479 ascat-2.4.0/docs/read_eumetsat_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    99279 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151416 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151239 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_8_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   719257 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.566479 ascat-2.4.0/docs/read_hsaf_cdr_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    68510 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77447 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78359 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162796 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78897 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65970 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1256504 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/docs/read_hsaf_nrt_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   173484 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168175 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165841 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171571 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186561 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1289682 2024-05-15 12:57:06.000000 ascat-2.4.0/docs/xarray_readers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 12:57:06.000000 ascat-2.4.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 12:57:06.000000 ascat-2.4.0/environment_win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 12:57:06.000000 ascat-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-15 12:57:12.582479 ascat-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 12:57:06.000000 ascat-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.554479 ascat-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/aggregate/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/cgls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/download/
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/download/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/download/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.570479 ascat-2.4.0/src/ascat/eumetsat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/eumetsat/level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29708 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/h_saf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.574478 ascat-2.4.0/src/ascat/read_native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21703 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/cdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/eps_native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.578479 ascat-2.4.0/src/ascat/read_native/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/ccsds.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)    67604 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    34467 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63559 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63563 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66425 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66555 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39840 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    37290 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36662 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44139 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44137 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42843 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25966 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31948 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89975 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/ragged_array_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57936 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/read_native/xarray_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.578479 ascat-2.4.0/src/ascat/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/regrid/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-15 12:57:06.000000 ascat-2.4.0/src/ascat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/src/ascat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 12:57:12.000000 ascat-2.4.0/src/ascat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:57:12.582479 ascat-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/get_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/skip_test_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_cgls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_h_saf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-15 12:57:06.000000 ascat-2.4.0/tests/test_level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-15 12:57:06.000000 ascat-2.4.0/tox.ini
```

### Comparing `ascat-2.3.1/.coveragerc` & `ascat-2.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/.github/workflows/ascat_ubuntu.yml` & `ascat-2.4.0/.github/workflows/ubuntu.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: ascat_ubuntu
+name: ubuntu
 
 on:
   push:
   pull_request:
   schedule:
     - cron: "0 0 * * *" # daily
 
@@ -10,65 +10,75 @@
   build:
     name: Build py${{ matrix.python-version }} @ ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: ["ubuntu-latest"]
+        ymlfile: ["environment.yml"]
 
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: false # does not work with self-hosted testdata
-      - name: Checkout Testdata
+      - name: Checkout test data
         shell: bash -l {0}
         run : |
           git submodule init
+          git submodule sync
           git submodule update
       - uses: conda-incubator/setup-miniconda@v2.0.1
         with:
-          miniconda-version: "latest"
-          auto-update-conda: true
+          miniforge-variant: Mambaforge
+          miniforge-version: "latest"
+          channel-priority: flexible
           python-version: ${{ matrix.python-version }}
-          environment-file: environment.yml
+          environment-file: ${{ matrix.ymlfile }}
           activate-environment: ascat_env
           auto-activate-base: false
-      - name: Print environment infos
+      - name: Print infos
         shell: bash -l {0}
         run: |
+          git status
           conda info -a
           conda list
           pip list
           which pip
           which python
       - name: Export Environment
         shell: bash -l {0}
         run: |
           mkdir -p .artifacts
           filename=env_py${{ matrix.python-version }}_${{ matrix.os }}.yml
           conda env export --no-builds | grep -v "prefix" > .artifacts/$filename
-      - name: Upload Artifacts
-        uses: actions/upload-artifact@v2
-        with:
-          name: os_py_environments
-          path: .artifacts/*
       - name: Install package and test
         shell: bash -l {0}
         run: |
-          pip install .
-          pip install pytest==6.2.5 coverage==5.2.1 tomli==1.2.3
-          python setup.py test
+          pip install -e .[testing]
+          pytest --cache-clear
       - name: Upload Coverage
         shell: bash -l {0}
         run: |
           pip install coveralls && coveralls --service=github
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           COVERALLS_FLAG_NAME: ${{ matrix.python-version }}
           COVERALLS_PARALLEL: true
+      - name: Create wheel and dist package
+        shell: bash -l {0}
+        run: |
+          git status
+          pip install setuptools_scm
+          python setup.py sdist --dist-dir .artifacts/dist
+          ls .artifacts/dist
+      - name: Upload Artifacts
+        uses: actions/upload-artifact@v2
+        with:
+          name: Artifacts
+          path: .artifacts/*
   coveralls:
     name: Submit Coveralls
     needs: build
     runs-on: ubuntu-latest
     container: python:3-slim
     steps:
       - name: Finished
```

### Comparing `ascat-2.3.1/.github/workflows/ascat_windows.yml` & `ascat-2.4.0/.github/workflows/windows.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: ascat_windows
+name: windows
 
 on:
   push:
   pull_request:
   schedule:
     - cron: '0 0 * * *' # daily
 
@@ -10,39 +10,42 @@
   build:
     name: Build py${{ matrix.python-version }} @ ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: ['windows-latest']
+        ymlfile: ["environment_win.yml"]
 
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: false # does not work with self-hosted testdata
-      - name: Checkout Testdata
+      - name: Checkout test data
         shell: bash -l {0}
         run : |
           git submodule init
+          git submodule sync
           git submodule update
       - uses: conda-incubator/setup-miniconda@v2.0.1
         with:
-          miniconda-version: "latest"
-          auto-update-conda: false
+          miniforge-variant: Mambaforge
+          miniforge-version: "latest"
+          channel-priority: flexible
           python-version: ${{ matrix.python-version }}
-          environment-file: environment_win.yml
+          environment-file: ${{ matrix.ymlfile }}
           activate-environment: ascat_env
           auto-activate-base: false
-      - name: Print environment infos
+      - name: Print infos
         shell: bash -l {0}
         run: |
+          git status
           conda info -a
           conda list
           pip list
           which pip
           which python
       - name: Install package and test
         shell: bash -l {0}
         run: |
-          pip install .
-          pip install pytest==6.2.5 tomli==1.2.3 pytest-cov==2.12.1
-          python setup.py test
+          pip install -e .[testing]
+          pytest --cache-clear
```

### Comparing `ascat-2.3.1/.github/workflows/upload_pypi.yml` & `ascat-2.4.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/.gitignore` & `ascat-2.4.0/.gitignore`

 * *Files 27% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 .pytest_cache/
 
 # Build and docs folder/files
 build/*
 dist/*
 sdist/*
 docs/api/*
+docs/org/obipy-resources/
+docs/org/*.ipynb
 docs/_rst/*
 docs/_build/*
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
-miniconda.sh
+miniconda.sh
```

### Comparing `ascat-2.3.1/CHANGELOG.rst` & `ascat-2.4.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+Version 2.4.0
+=============
+
+- Update file handling read_period
+- Refactor xarray readers/writers into SwathFileCollection, CellFileCollection,
+  and CellFileCollectionStack
+- Add tutorial for xarray readers/writers
+- Add CLI for aggregating ASCAT swath data
+- Add CLI for regridding ASCAT swath data to a regular lat/lon grid
+
 Version 2.3.1
 =============
 
 - Add str to path conversion for H SAF FTP download
 
 Version 2.3.0
 =============
```

### Comparing `ascat-2.3.1/LICENSE.txt` & `ascat-2.4.0/LICENSE.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 TU Wien
+Copyright (c) 2024 TU Wien
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ascat-2.3.1/docs/Makefile` & `ascat-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/ascat_bufr_format.rst` & `ascat-2.4.0/docs/ascat_bufr_format.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/conf.py` & `ascat-2.4.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,31 +68,36 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
+    "myst_nb",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = ".rst"
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".ipynb": "myst-nb",
+    ".myst": "myst-nb",
+}
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "ascat"
-copyright = "2023, TU Wien"
+copyright = "2024, TU Wien"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
@@ -149,23 +154,23 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+# html_theme_options = {
+#     "sidebar_width": "300px",
+#     "page_width": "1200px"
+# }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -280,7 +285,11 @@
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+
+
+# -- MyST-NB config ----------------------------------------------------------
+nb_execution_mode = 'off'
```

### Comparing `ascat-2.3.1/docs/examples.rst` & `ascat-2.4.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/index.rst` & `ascat-2.4.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 .. toctree::
    :maxdepth: 2
 
    Overview <readme>
    examples.rst
    ascat_bufr_format
+   xarray_readers_tutorial.ipynb
    License <license>
    Authors <authors>
-   Changelog <changelog>
    Module Reference <api/modules>
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `ascat-2.3.1/docs/read_cgls_swi_ts.ipynb` & `ascat-2.4.0/docs/read_cgls_swi_ts.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_cgls_swi_ts.rst` & `ascat-2.4.0/docs/read_cgls_swi_ts.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png` & `ascat-2.4.0/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_eumetsat.ipynb` & `ascat-2.4.0/docs/read_eumetsat.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_eumetsat.rst` & `ascat-2.4.0/docs/read_eumetsat.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_19_0.png` & `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_19_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_5_0.png` & `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_5_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_eumetsat_files/read_eumetsat_8_0.png` & `ascat-2.4.0/docs/read_eumetsat_files/read_eumetsat_8_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr.ipynb` & `ascat-2.4.0/docs/read_hsaf_cdr.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr.rst` & `ascat-2.4.0/docs/read_hsaf_cdr.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png` & `ascat-2.4.0/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt.ipynb` & `ascat-2.4.0/docs/read_hsaf_nrt.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt.rst` & `ascat-2.4.0/docs/read_hsaf_nrt.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png` & `ascat-2.4.0/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/setup.cfg` & `ascat-2.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = ascat
 description = Read and visualize for data from the Advanced Scatterometer (ASCAT)
 author = TU Wien
 author_email = remote.sensing@geo.tuwien.ac.at
 license = MIT
 license_files = LICENSE.txt
-long_description = file: README.rst
+long_description = file: README.md
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://tuwien.at/mg/geo/rs
 project_urls = 
 	Documentation = https://ascat.readthedocs.org/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
@@ -35,14 +35,16 @@
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	hsaf_download = ascat.download.interface:run_hsaf_download
 	eumetsat_download = ascat.download.interface:run_eumetsat_download
+	ascat_swath_agg = ascat.aggregate.interface:run_temporal_swath_agg
+	ascat_swath_regrid = ascat.regrid.interface:run_swath_regrid
 
 [tool:pytest]
 addopts = 
 	--cov ascat --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `ascat-2.3.1/setup.py` & `ascat-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/__init__.py` & `ascat-2.4.0/src/ascat/__init__.py`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/cgls.py` & `ascat-2.4.0/src/ascat/cgls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/download/connectors.py` & `ascat-2.4.0/src/ascat/download/connectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/download/interface.py` & `ascat-2.4.0/src/ascat/download/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/eumetsat/level1.py` & `ascat-2.4.0/src/ascat/eumetsat/level1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -20,34 +20,33 @@
 # GEOINFORMATION BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 """
 Readers for ASCAT Level 1b data for various file formats.
 """
 
 import os
+from datetime import timedelta
 from collections import defaultdict
 
 import numpy as np
 
 from ascat.read_native.nc import AscatL1bNcFile
 from ascat.read_native.hdf5 import AscatL1bHdf5File
 from ascat.read_native.bufr import AscatL1bBufrFile
 from ascat.read_native.eps_native import AscatL1bEpsFile
 from ascat.utils import get_toi_subset, get_roi_subset
 from ascat.file_handling import ChronFiles
 
 
 class AscatL1bFile:
-
     """
     Class reading ASCAT Level 1b files.
     """
 
     def __init__(self, filename, file_format=None):
         """
         Initialize.
@@ -161,15 +160,14 @@
     else:
         file_format = os.path.splitext(filename)[1]
 
     return file_format
 
 
 class AscatL1bBufrFileList(ChronFiles):
-
     """
     Class reading ASCAT L1b BUFR files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -188,16 +186,17 @@
         """
         sat_lut = {"a": 2, "b": 1, "c": 3}
         self.sat = sat_lut[sat]
 
         self.product = product.upper()
 
         if filename_template is None:
-            filename_template = ("M0{sat}-ASCA-ASC{product}1B0200-NA-9.1-"
-                                 "{date}.000000000Z-*-*.bfr")
+            filename_template = (
+                "M0{sat}-ASCA-ASC{product}1B0200-NA-9.1-"
+                "{date}.000000000Z-{placeholder1}-{placeholder2}.bfr")
 
         super().__init__(path, AscatL1bFile, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -209,39 +208,27 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat, "product": self.product}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat,
+            "product": self.product,
+            "placeholder1": "*",
+            "placeholder2": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[29:43],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
@@ -260,15 +247,14 @@
             else:
                 data = np.hstack(data)
 
         return data
 
 
 class AscatL1bNcFileList(ChronFiles):
-
     """
     Class reading ASCAT L1b NetCDF files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -289,15 +275,15 @@
 
         lut = {"szr": "125", "szo": "250"}
         self.product = lut[product]
 
         if filename_template is None:
             filename_template = (
                 "W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOP{sat}+"
-                "ASCAT_C_EUMP_{date}_*_eps_o_{product}_l1.nc")
+                "ASCAT_C_EUMP_{date}_{placeholder}_eps_o_{product}_l1.nc")
 
         super().__init__(path, AscatL1bFile, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -309,40 +295,26 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat.upper(),
-                       "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat.upper(),
+            "product": self.product.upper(),
+            "placeholder": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[62:76],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
@@ -361,15 +333,14 @@
             else:
                 data = np.hstack(data)
 
         return data
 
 
 class AscatL1bEpsFileList(ChronFiles):
-
     """
     Class reading ASCAT L1b Eps files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -387,15 +358,15 @@
                 "ASCA_{product}_1B_M0{sat}_{date}Z_*_*_*_*.nat")
         """
         sat_lut = {"a": 2, "b": 1, "c": 3, "?": "?"}
         self.sat = sat_lut[sat]
         self.product = product
 
         if filename_template is None:
-            filename_template = "ASCA_{product}_1B_M0{sat}_{date}Z_*_*_*_*.nat"
+            filename_template = "ASCA_{product}_1B_M0{sat}_{date}Z_{placeholder1}_{placeholder2}_{placeholder3}_{placeholder4}.nat"
 
         super().__init__(path, AscatL1bFile, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -407,39 +378,29 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat, "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat,
+            "product": self.product.upper(),
+            "placeholder1": "*",
+            "placeholder2": "*",
+            "placeholder3": "*",
+            "placeholder4": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[16:30],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
@@ -485,15 +446,14 @@
 
         merged_data = (merged_data, metadata)
 
         return merged_data
 
 
 class AscatL1bHdf5FileList(ChronFiles):
-
     """
     Class reading ASCAT L1b HDF5 files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -507,15 +467,15 @@
               "ASCA_SZF_1B_M0{sat}_{date}Z_*_*_*_*.h5")
         """
         sat_lut = {"a": "2", "b": "1", "c": "3", "?": "?"}
         self.sat = sat_lut[sat]
         self.product = product
 
         if filename_template is None:
-            filename_template = "ASCA_{product}_1B_M0{sat}_{date}Z_*_*_*_*.h5"
+            filename_template = "ASCA_{product}_1B_M0{sat}_{date}Z_{placeholder1}_{placeholder2}_{placeholder3}_{placeholder4}.h5"
 
         super().__init__(path, AscatL1bFile, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -527,39 +487,29 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat, "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat,
+            "product": self.product.upper(),
+            "placeholder1": "*",
+            "placeholder2": "*",
+            "placeholder3": "*",
+            "placeholder4": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[16:30],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
```

### Comparing `ascat-2.3.1/src/ascat/eumetsat/level2.py` & `ascat-2.4.0/src/ascat/eumetsat/level2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -20,32 +20,29 @@
 # GEOINFORMATION BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 """
 Readers for ASCAT Level 2 data for various file formats.
 """
 
 import os
 import numpy as np
-from datetime import datetime
 
 from ascat.read_native.nc import AscatL2NcFile
 from ascat.read_native.bufr import AscatL2BufrFile
 from ascat.read_native.eps_native import AscatL2EpsFile
 from ascat.utils import get_toi_subset, get_roi_subset
 from ascat.file_handling import ChronFiles
 
 
 class AscatL2File:
-
     """
     Class reading ASCAT Level 2 files.
     """
 
     def __init__(self, filename, file_format=None):
         """
         Initialize AscatL2File.
@@ -156,30 +153,29 @@
     else:
         file_format = os.path.splitext(filename)[1]
 
     return file_format
 
 
 class AscatL2BufrFileList(ChronFiles):
-
     """
     Class reading ASCAT L2 BUFR files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
         """
         sat_lut = {"a": 2, "b": 1, "c": 3}
         self.sat = sat_lut[sat]
         self.product = product
 
         if filename_template is None:
-            filename_template = ("M0{sat}-ASCA-ASC{product}*-*-*-"
-                                 "{date}.000000000Z-*-*.bfr")
+            filename_template = ("M0{sat}-ASCA-ASC{product}{placeholder1}-{placeholder2}-{placeholder3}-"
+                                 "{date}.000000000Z-{placeholder4}-{placeholder5}.bfr")
 
         super().__init__(path, AscatL2File, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -191,39 +187,30 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat, "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat,
+            "product": self.product.upper(),
+            "placeholder1": "*",
+            "placeholder2": "*",
+            "placeholder3": "*",
+            "placeholder4": "*",
+            "placeholder5": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[25:39],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
@@ -242,15 +229,14 @@
             else:
                 data = np.hstack(data)
 
         return data
 
 
 class AscatL2NcFileList(ChronFiles):
-
     """
     Class reading ASCAT L1b NetCDF files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -261,25 +247,25 @@
             Path to input data.
         sat : str
             Metop satellite ("a", "b", "c").
         product : str
             Product type ("szf", "szr", "szo").
         filename_template : str, optional
             Filename template (default:
-            "M0{sat}-ASCA-ASC{product}1B0200-NA-9.1-{date}.000000000Z-*-*.bfr")
+            "M0{sat}-ASCA-ASC{product}1B0200-NA-9.1-{date}.000000000Z-{placeholder1}-{placeholder2}.bfr")
         """
         self.sat = sat
 
         lut = {"smr": "125", "smo": "250"}
         self.product = lut[product]
 
         if filename_template is None:
             filename_template = (
                 "W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOP{sat}+"
-                "ASCAT_C_EUMP_{date}_*_eps_o_{product}_ssm_l2.nc")
+                "ASCAT_C_EUMP_{date}_{placeholder}_eps_o_{product}_ssm_l2.nc")
 
         super().__init__(path, AscatL2File, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -291,40 +277,26 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat.upper(),
-                       "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat.upper(),
+            "product": self.product.upper(),
+            "placeholder": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[62:76],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
@@ -343,15 +315,14 @@
             else:
                 data = np.hstack(data)
 
         return data
 
 
 class AscatL2EpsFileList(ChronFiles):
-
     """
     Class reading ASCAT L2 Eps files.
     """
 
     def __init__(self, path, sat, product, filename_template=None):
         """
         Initialize.
@@ -369,15 +340,15 @@
                 "ASCA_{product}_02_M0{sat}_{date}Z_*_*_*_*.nat")
         """
         sat_lut = {"a": 2, "b": 1, "c": 3, "?": "?"}
         self.sat = sat_lut[sat]
         self.product = product
 
         if filename_template is None:
-            filename_template = "ASCA_{product}_02_M0{sat}_{date}Z_*_*_*_*.nat"
+            filename_template = "ASCA_{product}_02_M0{sat}_{date}Z_{placeholder1}_{placeholder2}_{placeholder3}_{placeholder4}.nat"
 
         super().__init__(path, AscatL2File, filename_template, None)
 
     def _fmt(self, timestamp):
         """
         Definition of filename and subfolder format.
 
@@ -389,39 +360,29 @@
         Returns
         -------
         fn_fmt : dict
             Filename format.
         sf_fmt : dict
             Subfolder format.
         """
-        fn_read_fmt = {"date": timestamp.strftime("%Y%m%d%H%M%S"),
-                       "sat": self.sat, "product": self.product.upper()}
+        fn_read_fmt = {
+            "date": timestamp.strftime("%Y%m%d%H%M%S"),
+            "sat": self.sat,
+            "product": self.product.upper(),
+            "placeholder1": "*",
+            "placeholder2": "*",
+            "placeholder3": "*",
+            "placeholder4": "*",
+        }
         fn_write_fmt = None
         sf_read_fmt = None
         sf_write_fmt = sf_read_fmt
 
         return fn_read_fmt, sf_read_fmt, fn_write_fmt, sf_write_fmt
 
-    # def _parse_date(self, filename):
-    #     """
-    #     Parse date from filename.
-
-    #     Parameters
-    #     ----------
-    #     filename : str
-    #         Filename.
-
-    #     Returns
-    #     -------
-    #     date : datetime
-    #         Parsed date.
-    #     """
-    #     return datetime.strptime(os.path.basename(filename)[16:30],
-    #                              "%Y%m%d%H%M%S")
-
     def _merge_data(self, data):
         """
         Merge data.
 
         Parameters
         ----------
         data : list
```

### Comparing `ascat-2.3.1/src/ascat/file_handling.py` & `ascat-2.4.0/src/ascat/file_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -700,15 +700,16 @@
         dates : list of datetime
             Parsed date of filename (only returned if return_date=True).
         """
         fn_read_fmt, sf_read_fmt, _, _ = self._fmt(timestamp)
         fn_read_fmt[date_field] = timestamp.strftime(search_date_fmt)
 
         fs = FileSearch(self.root_path, self.ft.fn_templ, self.ft.sf_templ)
-        filenames = sorted(fs.search(fn_read_fmt, sf_read_fmt))
+        key_func = lambda x: self._parse_date(x, date_field, date_field_fmt)
+        filenames = sorted(fs.search(fn_read_fmt, sf_read_fmt), key=key_func)
 
         if return_date:
             dates = []
             for filename in filenames:
                 dates.append(
                     self._parse_date(filename, date_field, date_field_fmt))
             return filenames, dates
@@ -719,14 +720,15 @@
         self,
         dt_start,
         dt_end,
         dt_delta=timedelta(days=1),
         search_date_fmt="%Y%m%d*",
         date_field="date",
         date_field_fmt="%Y%m%d",
+        end_inclusive=True,
     ):
         """
         Search files for time period.
 
         Parameters
         ----------
         dt_start : datetime
@@ -737,45 +739,50 @@
             Time delta used to jump through search date.
         search_fmt : str, optional
             Search date string format used during file search (default: %Y%m%d*).
         date_field : str, optional
             Date field name (default: "date").
         date_field_fmt : str, optional
             Date field string format (default: %Y%m%d).
+        end_inclusive : bool, optional
+            Include files from a dt_delta length period beyond dt_end if True
+            (default: False).
 
         Returns
         -------
         filenames : list of str
             Filenames.
         """
         filenames = []
 
-        for dt_cur in np.arange(dt_start, dt_end + dt_delta,
-                                dt_delta).astype(datetime):
+        dt_end = dt_end + dt_delta if end_inclusive else dt_end
+
+        for dt_cur in np.arange(dt_start, dt_end, dt_delta).astype(datetime):
             files, dates = self.search_date(
                 dt_cur,
-                search_date_fmt,
-                date_field,
-                date_field_fmt,
+                search_date_fmt=search_date_fmt,
+                date_field=date_field,
+                date_field_fmt=date_field_fmt,
                 return_date=True)
             for f, dt in zip(files, dates):
-                if f not in filenames and dt >= dt_start and dt < dt_end + dt_delta:
+                if f not in filenames and dt >= dt_start and dt < dt_end:
                     filenames.append(f)
 
         return filenames
 
     def read_period(
         self,
         dt_start,
         dt_end,
         dt_delta=timedelta(days=1),
         dt_buffer=timedelta(days=1),
         search_date_fmt="%Y%m%d*",
         date_field="date",
         date_field_fmt="%Y%m%d",
+        end_inclusive=True,
         **kwargs,
     ):
         """
         Read data for given interval.
 
         Parameters
         ----------
@@ -798,15 +805,15 @@
         Returns
         -------
         data : dict, numpy.ndarray
             Data stored in file.
         """
         filenames = self.search_period(dt_start - dt_buffer, dt_end, dt_delta,
                                        search_date_fmt, date_field,
-                                       date_field_fmt)
+                                       date_field_fmt, end_inclusive)
 
         data = []
 
         for filename in filenames:
             self._open(filename)
             d = self.fid.read_period(dt_start, dt_end, **kwargs)
             if d is not None:
```

### Comparing `ascat-2.3.1/src/ascat/h_saf.py` & `ascat-2.4.0/src/ascat/h_saf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/read_native/bufr.py` & `ascat-2.4.0/src/ascat/read_native/bufr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/read_native/cdr.py` & `ascat-2.4.0/src/ascat/read_native/cdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/read_native/eps_native.py` & `ascat-2.4.0/src/ascat/read_native/eps_native.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/ccsds.xml` & `ascat-2.4.0/src/ascat/read_native/formats/ccsds.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps.dtd` & `ascat-2.4.0/src/ascat/read_native/formats/eps.dtd`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps.xsl` & `ascat-2.4.0/src/ascat/read_native/formats/eps.xsl`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smo_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml` & `ascat-2.4.0/src/ascat/read_native/formats/eps_ascatl2smr_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.3.1/src/ascat/read_native/hdf5.py` & `ascat-2.4.0/src/ascat/read_native/hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/read_native/nc.py` & `ascat-2.4.0/src/ascat/read_native/nc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
```

### Comparing `ascat-2.3.1/src/ascat/utils.py` & `ascat-2.4.0/src/ascat/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien, Department of Geodesy and Geoinformation
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -296,7 +296,79 @@
         else:
             if isinstance(ds, xr.Dataset):
                 ds = ds.sel(obs=np.nonzero(subset.values)[0])
             elif isinstance(ds, np.ndarray):
                 ds = ds[subset]
 
     return ds
+
+
+class Spacecraft:
+    """
+    Spacecraft class.
+    """
+
+    valid_spacecraft_names = [
+        "METOPA", "METOPB", "METOPC", "METOP-A", "METOP-B", "METOP-C",
+        "METOP-SG B1", "METOP-SG B2", "METOP-SG B3"
+    ]
+
+    def __init__(self, name):
+        """
+        Initialize spacecraft class.
+
+        Parameters
+        ----------
+        name : str
+            Spacecraft name.
+        """
+        if name not in Spacecraft.valid_spacecraft_names:
+            valid_names = ' ,'.join(Spacecraft.valid_spacecraft_names)
+            msg = f"Spacecraft {name} unknown. Valid options: {valid_names}"
+            raise RuntimeError(msg)
+
+        satellite_dict = {
+            "METOPA": "METOPA",
+            "METOPB": "METOPB",
+            "METOPC": "METOPC",
+            "METOP-A": "METOPA",
+            "METOP-B": "METOPB",
+            "METOP-C": "METOPC",
+            "METOP-SG B1": "METOP-SGB1",
+            "METOP-SG B2": "METOP-SGB2",
+            "METOP-SG B3": "METOP-SGB3"
+        }
+
+        platform_dict = {
+            "METOPA": "Metop",
+            "METOPB": "Metop",
+            "METOPC": "Metop",
+            "METOP-SGB1": "Metop-SG",
+            "METOP-SGB2": "Metop-SG",
+            "METOP-SGB3": "Metop-SG"
+        }
+
+        sensor_dict = {"Metop": "ASCAT", "Metop-SG": "SCA"}
+
+        sat_name_dict = {
+            "METOPA": "A",
+            "METOPB": "B",
+            "METOPC": "C",
+            "METOP-SGB1": "B1",
+            "METOP-SGB2": "B2",
+            "METOP-SGB3": "B3"
+        }
+
+        sat_id_dict = {
+            "METOPA": 3,
+            "METOPB": 4,
+            "METOPC": 5,
+            "METOP-SGB1": 6,
+            "METOP-SGB2": 7,
+            "METOP-SGB3": 8
+        }
+
+        self.satellite = satellite_dict[name]
+        self.platform = platform_dict[self.satellite]
+        self.sensor = sensor_dict[self.platform]
+        self.sat_name = sat_name_dict[self.satellite]
+        self.sat_id = sat_id_dict[self.satellite]
```

### Comparing `ascat-2.3.1/src/ascat.egg-info/SOURCES.txt` & `ascat-2.4.0/src/ascat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 .coveragerc
 .gitignore
 .gitmodules
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE.txt
-README.rst
+README.md
 environment.yml
 environment_win.yml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/ascat_ubuntu.yml
-.github/workflows/ascat_windows.yml
+.github/workflows/ubuntu.yml
 .github/workflows/upload_pypi.yml
+.github/workflows/windows.yml
 docs/Makefile
 docs/ascat_bufr_format.rst
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
-docs/env.yml
+docs/docs_env.yml
 docs/examples.rst
 docs/index.rst
 docs/license.rst
 docs/read_cgls_swi_ts.ipynb
 docs/read_cgls_swi_ts.rst
 docs/read_eumetsat.ipynb
 docs/read_eumetsat.rst
 docs/read_hsaf_cdr.ipynb
 docs/read_hsaf_cdr.rst
 docs/read_hsaf_nrt.ipynb
 docs/read_hsaf_nrt.rst
 docs/readme.rst
 docs/requirements.txt
+docs/xarray_readers_tutorial.ipynb
 docs/_static/.gitignore
+docs/org/xarray_readers_tutorial.org
 docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
 docs/read_eumetsat_files/read_eumetsat_19_0.png
 docs/read_eumetsat_files/read_eumetsat_5_0.png
 docs/read_eumetsat_files/read_eumetsat_8_0.png
 docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
 docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
 docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
@@ -60,26 +62,30 @@
 src/ascat.egg-info/PKG-INFO
 src/ascat.egg-info/SOURCES.txt
 src/ascat.egg-info/dependency_links.txt
 src/ascat.egg-info/entry_points.txt
 src/ascat.egg-info/not-zip-safe
 src/ascat.egg-info/requires.txt
 src/ascat.egg-info/top_level.txt
+src/ascat/aggregate/__init__.py
+src/ascat/aggregate/aggregators.py
+src/ascat/aggregate/interface.py
 src/ascat/download/connectors.py
 src/ascat/download/interface.py
 src/ascat/eumetsat/__init__.py
 src/ascat/eumetsat/level1.py
 src/ascat/eumetsat/level2.py
 src/ascat/read_native/__init__.py
 src/ascat/read_native/bufr.py
 src/ascat/read_native/cdr.py
 src/ascat/read_native/eps_native.py
 src/ascat/read_native/hdf5.py
 src/ascat/read_native/nc.py
 src/ascat/read_native/ragged_array_ts.py
+src/ascat/read_native/xarray_io.py
 src/ascat/read_native/formats/ccsds.xml
 src/ascat/read_native/formats/eps.dtd
 src/ascat/read_native/formats/eps.xsl
 src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
 src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
@@ -102,14 +108,19 @@
 src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
 src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
 src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
 src/ascat/read_native/formats/eps_ascatl2smo_4.xml
 src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
 src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
 src/ascat/read_native/formats/eps_ascatl2smr_4.xml
+src/ascat/regrid/__init__.py
+src/ascat/regrid/interface.py
+src/ascat/regrid/regrid.py
 tests/conftest.py
+tests/get_path.py
+tests/skip_test_ragged_array.py
 tests/test_cgls.py
 tests/test_download.py
 tests/test_file_handling.py
 tests/test_h_saf.py
 tests/test_level1.py
 tests/test_level2.py
```

### Comparing `ascat-2.3.1/tests/test_cgls.py` & `ascat-2.4.0/tests/test_cgls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -20,32 +20,31 @@
 # GEOINFORMATION BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 """
 Tests for reading CGLOPS SWI data.
 """
 
-from ascat.cgls import SWI_TS
-import os
 import pandas as pd
 import numpy as np
 import pytest
 
+from get_path import get_testdata_path
+from ascat.cgls import SWI_TS
+
 
 def test_swi_ts_reader():
     """
     Test SWI time series reader.
     """
-    data_path = os.path.join(
-        os.path.dirname(__file__), 'ascat_test_data', 'cglops', 'swi_ts')
+    data_path = get_testdata_path() / "cglops" / "swi_ts"
 
     rd = SWI_TS(data_path)
     data = rd.read(3002621, mask_frozen=False)
     data_sorted = data.sort_index()
 
     assert np.all(data_sorted.index == data.index)
     # just check if enough data is there
@@ -64,33 +63,31 @@
     assert np.all(data_sorted.index == reference_index)
 
 
 def test_swi_ts_reader_no_data_in_folder():
     """
     Test SWI time series reader when no data is in folder.
     """
-    data_path = os.path.join(
-        os.path.dirname(__file__), 'ascat_test_data', 'cglops', 'swi_ts_non_existing')
+    data_path = get_testdata_path() / "cglops" / "swi_ts_non_existing"
 
     with pytest.raises(IOError):
         SWI_TS(data_path)
 
 
 def test_swi_ts_qflag_reading():
     """
     Test SWI time series quality flag reader.
     """
-    data_path = os.path.join(
-        os.path.dirname(__file__), 'ascat_test_data', 'cglops', 'swi_ts')
+    data_path = get_testdata_path() / "cglops" / "swi_ts"
     rd = SWI_TS(data_path, parameters=['SWI_001', 'QFLAG_001', 'SSF'])
     data = rd.read(3002621, mask_frozen=True)
     # check if QFLAG is correctly read. It should have as many NaN values as
     # SWI
     assert len(data[data.loc[:, 'QFLAG_001'] != np.nan]) > 0
-    assert (len(data[data.loc[:, 'QFLAG_001'] == np.nan]) ==
-            len(data[data.loc[:, 'SWI_001'] == np.nan]))
+    assert (len(data[data.loc[:, 'QFLAG_001'] == np.nan]) == len(
+        data[data.loc[:, 'SWI_001'] == np.nan]))
 
 
 if __name__ == "__main__":
     test_swi_ts_reader()
     test_swi_ts_qflag_reading()
     test_swi_ts_reader_no_data_in_folder()
```

### Comparing `ascat-2.3.1/tests/test_download.py` & `ascat-2.4.0/tests/test_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -20,31 +20,37 @@
 # GEOINFORMATION BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 """
 Test download.
 """
 
 import os
 import unittest
 from tempfile import mkdtemp
 from datetime import datetime, timedelta
 
 from ascat.download.connectors import HsafConnector
 from ascat.download.connectors import EumConnector
 
-credentials = {'EUM': {'consumer_key': os.getenv('EUM_CONSUMER_KEY'),
-                       'consumer_secret': os.getenv('EUM_CONSUMER_SECRET')},
-               'HSAF': {'user': os.getenv('HSAF_FTP_USER'),
-                        'password': os.getenv('HSAF_FTP_PASSWORD')}}
+credentials = {
+    'EUM': {
+        'consumer_key': os.getenv('EUM_CONSUMER_KEY'),
+        'consumer_secret': os.getenv('EUM_CONSUMER_SECRET')
+    },
+    'HSAF': {
+        'user': os.getenv('HSAF_FTP_USER'),
+        'password': os.getenv('HSAF_FTP_PASSWORD')
+    }
+}
+
 
 class TestDownload(unittest.TestCase):
 
     def setUp(self):
         """
         Get connection details.
         """
@@ -70,16 +76,16 @@
         """
         Test EUMETSAT download.
         """
         product = "EO:EUM:DAT:METOP:SOMO12"
 
         connector = EumConnector()
         connector.connect(credentials['EUM'])
-        connector.download(product, self.local_path, self.start_date,
-                           self.end_date, limit=1)
+        connector.download(
+            product, self.local_path, self.start_date, self.end_date, limit=1)
 
     @unittest.skipIf(credentials['HSAF']['user'] is None,
                      "Skip H SAF connection test")
     def test_hsaf_connect(self):
         """
         Test H SAF connection.
         """
@@ -93,13 +99,18 @@
         """
         Test H SAF download.
         """
         remote_path = '/products/h08/h08_cur_mon_nc'
 
         connector = HsafConnector()
         connector.connect(credentials['HSAF'])
-        connector.download(remote_path, self.local_path, self.start_date,
-                           self.end_date, limit=1)
+        connector.download(
+            remote_path,
+            self.local_path,
+            self.start_date,
+            self.end_date,
+            limit=1)
         connector.close()
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ascat-2.3.1/tests/test_file_handling.py` & `ascat-2.4.0/tests/test_file_handling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -48,41 +48,39 @@
     """
     Generate fake test data.
     """
     tmpdir = Path(tempfile.mkdtemp())
 
     for num in ["01", "02", "03"]:
         for tile in ["EN01212", "EN01234", "EN01256"]:
-            folder = tmpdir / Path(f"temperature/{tile}")
-
+            folder = tmpdir / "temperature" / tile
             folder.mkdir(parents=True, exist_ok=True)
 
-            filename = tmpdir / Path(
-                f"temperature/{tile}/202201{num}_ascat.csv")
+            filename = tmpdir / "temperature" / tile / f"202201{num}_ascat.csv"
 
             csv_file = Csv(filename, mode="w")
             file_dates = [
                 datetime.strptime(f"202201{num}", "%Y%m%d") +
                 timedelta(seconds=(3600 * i + seconds))
                 for i, seconds in enumerate(range(3500, 3700))
             ]
 
             file_temps = random.choices(range(20, 35), k=15)
             dtype = np.dtype([("date", "datetime64[s]"),
                               ("temperature", "float32")])
-            write_data = np.array(list(zip(file_dates, file_temps)),
-                                  dtype=dtype)
+            write_data = np.array(
+                list(zip(file_dates, file_temps)), dtype=dtype)
             csv_file.write(write_data)
 
     for num in ["01", "02", "03"]:
         for tile in ["EN01212", "EN01234", "EN01256"]:
             prev_time = datetime.strptime(f"202201{num}0000", "%Y%m%d%H%M")
             next_day = prev_time + timedelta(days=1)
 
-            folder = tmpdir / Path(f"precipitation/{tile}")
+            folder = tmpdir / "precipitation" / tile
             folder.mkdir(parents=True, exist_ok=True)
 
             while prev_time < next_day:
                 file_dates = [
                     prev_time + timedelta(seconds=i)
                     for i in range(random.randrange(120, 180))
                     if (random.randrange(10) < 7)
@@ -98,20 +96,20 @@
                 d1, d2 = file_dates[0].strftime(
                     "%Y%m%d"), file_dates[-2].strftime("%Y%m%d")
                 t1, t2 = file_dates[0].strftime(
                     "%H%M%S"), file_dates[-2].strftime("%H%M%S")
                 filename = folder / Path(f"ascat_{d1}_{t1}-{d2}_{t2}.csv")
 
                 csv_file = Csv(filename, mode="w")
-                file_precips = random.choices(range(0, 5),
-                                              k=len(file_dates) - 1)
+                file_precips = random.choices(
+                    range(0, 5), k=len(file_dates) - 1)
                 dtype = np.dtype([("date", "datetime64[s]"),
                                   ("precipitation", "float32")])
-                write_data = np.array(list(zip(file_dates[:-1], file_precips)),
-                                      dtype=dtype)
+                write_data = np.array(
+                    list(zip(file_dates[:-1], file_precips)), dtype=dtype)
                 csv_file.write(write_data)
                 prev_time = file_dates[-1]
 
     return tmpdir
 
 
 class CustomTestCase(unittest.TestCase):
@@ -144,15 +142,15 @@
 
     def test_template_property(self):
         """
         Test the template property.
         """
         self.assertEqual(
             str(self.template.template),
-            str(self.tmpdir / "{variable}/{tile}/{date}_*.{suffix}"))
+            str(self.tmpdir / "{variable}" / "{tile}" / "{date}_*.{suffix}"))
 
     def test_build_filename(self):
         """
         Test the build_filename method.
         """
         fn_fmt = {"date": "20220101", "suffix": "csv"}
         sf_fmt = {
@@ -161,15 +159,15 @@
             },
             "tiles": {
                 "tile": "EN01234"
             }
         }
         self.assertEqual(
             self.template.build_filename(fn_fmt, sf_fmt),
-            str(self.tmpdir / "temperature/EN01234/20220101_*.csv"))
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_*.csv"))
 
     def test_build_basename(self):
         """
         Test the build_basename method.
         """
         fmt = {"date": "20220101", "suffix": "csv"}
         self.assertEqual(self.template.build_basename(fmt), "20220101_*.csv")
@@ -182,16 +180,16 @@
             "variables": {
                 "variable": "temperature"
             },
             "tiles": {
                 "tile": "EN01234"
             }
         }
-        self.assertEqual(self.template.build_subfolder(fmt),
-                         ["temperature", "EN01234"])
+        self.assertEqual(
+            self.template.build_subfolder(fmt), ["temperature", "EN01234"])
 
 
 class TestFileSearch(CustomTestCase):
     """
     Tests for FileSearch class.
     """
 
@@ -215,15 +213,15 @@
             "tiles": {
                 "tile": "EN01234"
             }
         }
         recursive = False
         search_result = self.filesearch.search(fn_fmt, sf_fmt, recursive)
         expected_result = [
-            str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv")
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv")
         ]
         self.assertEqual(search_result, expected_result)
 
     def test_search_wc(self):
         """
         Test search with wildcard.
         """
@@ -236,24 +234,23 @@
                 "tile": "EN012*"
             }
         }
         recursive = False
         search_result = self.filesearch.search(fn_fmt, sf_fmt, recursive)
         expected_result = [
             str(item) for item in [
-                self.tmpdir /
-                "temperature/EN01234/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220103_ascat.csv"
+                self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv",
+                self.tmpdir / "temperature" / "EN01234" / "20220102_ascat.csv",
+                self.tmpdir / "temperature" / "EN01234" / "20220103_ascat.csv",
+                self.tmpdir / "temperature" / "EN01212" / "20220101_ascat.csv",
+                self.tmpdir / "temperature" / "EN01212" / "20220102_ascat.csv",
+                self.tmpdir / "temperature" / "EN01212" / "20220103_ascat.csv",
+                self.tmpdir / "temperature" / "EN01256" / "20220101_ascat.csv",
+                self.tmpdir / "temperature" / "EN01256" / "20220102_ascat.csv",
+                self.tmpdir / "temperature" / "EN01256" / "20220103_ascat.csv"
             ]
         ]
         self.assertEqual(sorted(search_result), sorted(expected_result))
 
     def test_isearch(self):
         """
         Test isearch.
@@ -266,15 +263,15 @@
             "tiles": {
                 "tile": "EN01234"
             }
         }
         recursive = False
         search_result = self.filesearch.isearch(fn_fmt, sf_fmt, recursive)
         expected_result = iter(
-            [str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv")])
+            [str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv")])
 
         self.assertEqual(list(search_result), list(expected_result))
 
     def test_isearch_wc(self):
         """
         Test isearch with wildcard.
         """
@@ -287,24 +284,23 @@
                 "tile": "EN012*"
             }
         }
         recursive = False
         search_result = self.filesearch.isearch(fn_fmt, sf_fmt, recursive)
         expected_result = iter([
             str(item) for item in [
-                self.tmpdir /
-                "temperature/EN01212/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220103_ascat.csv"
+                self.tmpdir / "temperature" /"EN01212"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220103_ascat.csv"
             ]
         ])
         self.assertEqual(sorted(search_result), sorted(expected_result))
 
     def test_create_search_func(self):
         """
         Test custom search function.
@@ -323,15 +319,15 @@
             return fn_fmt, sf_fmt
 
         recursive = False
         custom_search_func = self.filesearch.create_search_func(
             custom_func, recursive)
         search_result = custom_search_func("20220101", "temperature")
         expected_result = [
-            str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv")
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv")
         ]
         self.assertEqual(search_result, expected_result)
 
     def test_create_search_func_wc(self):
         """
         Test custom search function with wildcard.
         """
@@ -350,24 +346,23 @@
 
         recursive = False
         custom_search_func = self.filesearch.create_search_func(
             custom_func, recursive)
         search_result = custom_search_func("202201*", "temperature")
         expected_result = [
             str(item) for item in [
-                self.tmpdir /
-                "temperature/EN01234/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220103_ascat.csv"
+                self.tmpdir / "temperature" /"EN01234"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220103_ascat.csv"
             ]
         ]
         self.assertEqual(sorted(search_result), sorted(expected_result))
 
     def test_create_isearch_func(self):
         """
         Test custom isearch function with wildcard.
@@ -386,15 +381,15 @@
             return fn_fmt, sf_fmt
 
         recursive = False
         custom_isearch_func = self.filesearch.create_isearch_func(
             custom_func, recursive)
         search_result = custom_isearch_func("20220101", "temperature")
         expected_result = iter(
-            [str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv")])
+            [str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv")])
 
         self.assertEqual(list(search_result), list(expected_result))
 
     def test_create_isearch_func_wc(self):
         """
         Test custom isearch function with wildcard.
         """
@@ -413,24 +408,23 @@
 
         recursive = False
         custom_isearch_func = self.filesearch.create_isearch_func(
             custom_func, recursive)
         search_result = custom_isearch_func("202201*", "temperature")
         expected_result = iter([
             str(item) for item in [
-                self.tmpdir /
-                "temperature/EN01234/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01234/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01212/20220103_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220101_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220102_ascat.csv", self.tmpdir /
-                "temperature/EN01256/20220103_ascat.csv"
+                self.tmpdir / "temperature" /"EN01234"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01234"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01212"/ "20220103_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220101_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220102_ascat.csv",
+                self.tmpdir / "temperature" /"EN01256"/ "20220103_ascat.csv"
             ]
         ])
         self.assertEqual(sorted(search_result), sorted(expected_result))
 
 
 class TestChronFiles(CustomTestCase):
     """
@@ -460,48 +454,60 @@
                                       sf_read_fmt)
 
     def test_search_date(self):
         """
         Test search date.
         """
         timestamp = datetime(2022, 1, 1)
-        filenames = self.chron_files.search_date(timestamp,
-                                                 date_str="%Y%m%d",
-                                                 date_field="date")
+        filenames = self.chron_files.search_date(
+            timestamp, date_field_fmt="%Y%m%d", date_field="date")
         expected_filenames = [
-            str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv")
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv")
         ]
         self.assertEqual(filenames, expected_filenames)
 
     def test_search_period(self):
         """
         Test search period.
         """
         dt_start = datetime(2022, 1, 1)
         dt_end = datetime(2022, 1, 3)
-        filenames = self.chron_files.search_period(dt_start,
-                                                   dt_end,
-                                                   dt_delta=timedelta(days=1))
+        filenames = self.chron_files.search_period(
+            dt_start, dt_end, dt_delta=timedelta(days=1))
+        expected_filenames = [
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv"),
+            str(self.tmpdir / "temperature" / "EN01234" / "20220102_ascat.csv"),
+            str(self.tmpdir / "temperature" / "EN01234" / "20220103_ascat.csv")
+        ]
+        self.assertTrue(filenames)
+        self.assertEqual(filenames, expected_filenames)
+
+    def test_search_period_exclusive(self):
+        """
+        Test search period.
+        """
+        dt_start = datetime(2022, 1, 1)
+        dt_end = datetime(2022, 1, 3)
+        filenames = self.chron_files.search_period(
+            dt_start, dt_end, dt_delta=timedelta(days=1), end_inclusive=False)
         expected_filenames = [
-            str(self.tmpdir / "temperature/EN01234/20220101_ascat.csv"),
-            str(self.tmpdir / "temperature/EN01234/20220102_ascat.csv"),
-            str(self.tmpdir / "temperature/EN01234/20220103_ascat.csv")
+            str(self.tmpdir / "temperature" / "EN01234" / "20220101_ascat.csv"),
+            str(self.tmpdir / "temperature" / "EN01234" / "20220102_ascat.csv"),
         ]
         self.assertTrue(filenames)
         self.assertEqual(filenames, expected_filenames)
 
     def test_read_period(self):
         """
         Test read period.
         """
         dt_start = datetime(2022, 1, 1, hour=12, minute=30)
         dt_end = datetime(2022, 1, 2, hour=12, minute=30)
-        data = self.chron_files.read_period(dt_start,
-                                            dt_end,
-                                            dt_delta=timedelta(days=1))
+        data = self.chron_files.read_period(
+            dt_start, dt_end, dt_delta=timedelta(days=1))
 
         self.assertTrue(data["date"].min() >= dt_start)
         self.assertTrue(data["date"].max() <= dt_end)
 
 
 class TestCsvFiles(unittest.TestCase):
     """
@@ -523,17 +529,16 @@
                           ("temperature", "float32")])
 
         dates = np.arange("2000-01-01", "2000-01-10", dtype="datetime64[D]")
 
         tmp_data = {}
 
         for date in dates:
-            dt = np.arange(date,
-                           date + np.timedelta64(1, "D"),
-                           dtype="datetime64[h]")
+            dt = np.arange(
+                date, date + np.timedelta64(1, "D"), dtype="datetime64[h]")
             temperature = random.choices(range(0, 40), k=dt.size)
             data = np.array(list(zip(dt, temperature)), dtype=dtype)
 
             self.csv.write(data, date.astype(datetime))
             tmp_data[date] = data
 
         for date in dates:
```

### Comparing `ascat-2.3.1/tests/test_h_saf.py` & `ascat-2.4.0/tests/test_h_saf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -21,44 +21,44 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import os
 import sys
 import pytest
 import unittest
 from datetime import datetime
 
 import numpy as np
 import numpy.testing as nptest
 
 from ascat.h_saf import H14GribFileList
 from ascat.h_saf import AscatNrtBufrFileList
 from ascat.h_saf import AscatSsmDataRecord
 
+from get_path import get_testdata_path
+
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatNrtSsm(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test data.
         """
-        self.root_path = os.path.join(os.path.dirname(__file__),
-                                      'ascat_test_data', 'hsaf')
+        self.root_path = get_testdata_path() / "hsaf"
 
     def test_h16_read(self):
         """
         Test read file.
         """
         dt = datetime(2017, 2, 20, 11, 15, 0)
-        path = os.path.join(self.root_path, 'h16')
+        path = self.root_path / 'h16'
         product = 'h16'
 
         h16 = AscatNrtBufrFileList(path, product)
         data, metadata = h16.read(dt)
 
         sm_should = np.array([
             0., 3.6, 7.8, 8.2, 12.3, 14.7, 21.6, 26.7, 30.6, 32.2, 43., 50.5,
@@ -86,24 +86,23 @@
         sm_mean_should = np.array([
             32.8, 35.1, 37.8, 39.2, 39., 38., 36.2, 39.6, 43.8, 45.6, 46.1,
             47., 43.7, 46., 46.7
         ])
 
         nptest.assert_allclose(data['lat'][798:813], lats_should, atol=1e-5)
         nptest.assert_allclose(data['sm'][798:813], sm_should, atol=0.01)
-        nptest.assert_allclose(data['sm_mean'][798:813],
-                               sm_mean_should,
-                               atol=0.01)
+        nptest.assert_allclose(
+            data['sm_mean'][798:813], sm_mean_should, atol=0.01)
 
     def test_h101_read(self):
         """
         Test read file.
         """
         dt = datetime(2017, 2, 20, 10, 42, 0)
-        path = os.path.join(self.root_path, 'h101')
+        path = self.root_path / 'h101'
         product_id = 'h101'
 
         h101 = AscatNrtBufrFileList(path, product_id)
         data, metadata = h101.read(dt)
 
         sm_should = np.array([
             26.1, 31.5, 49.5, 64.3, 80.3, 87.9, 24.5, 18.5, 20., 12.9, 6.3,
@@ -120,24 +119,23 @@
         sm_mean_should = np.array([
             22.8, 27., 31.8, 38.3, 44.3, 52.4, 24.8, 27.8, 24.7, 23.9, 22.8,
             25., 25.6, 26.1, 25.9, 26.9, 28.5, 27.8, 24.3, 22.7
         ])
 
         nptest.assert_allclose(data['lat'][1800:1820], lats_should, atol=1e-5)
         nptest.assert_allclose(data['sm'][1800:1820], sm_should, atol=0.01)
-        nptest.assert_allclose(data['sm_mean'][1800:1820],
-                               sm_mean_should,
-                               atol=0.01)
+        nptest.assert_allclose(
+            data['sm_mean'][1800:1820], sm_mean_should, atol=0.01)
 
     def test_h102_read(self):
         """
         Test read file.
         """
         dt = datetime(2017, 2, 20, 10, 42, 0)
-        path = os.path.join(self.root_path, 'h102')
+        path = self.root_path / 'h102'
         product_id = 'h102'
 
         h102 = AscatNrtBufrFileList(path, product_id)
         data, metadata = h102.read(dt)
 
         sm_should = np.array([
             45.8, 43.5, 41.7, 42.7, 38.6, 31.1, 23.4, 21.7, 23.6, 26.8, 30.5,
@@ -153,24 +151,23 @@
         sm_mean_should = np.array([
             50.8, 44.5, 36.3, 29.9, 28.7, 29.1, 30., 30.1, 30.8, 33., 34.9,
             35.7, 35.2, 34.2, 32.9, 32.9, 34.5, 32.7, 30.6
         ])
 
         nptest.assert_allclose(data['lat'][0:19], lats_should, atol=1e-5)
         nptest.assert_allclose(data['sm'][0:19], sm_should, atol=0.01)
-        nptest.assert_allclose(data['sm_mean'][0:19],
-                               sm_mean_should,
-                               atol=0.01)
+        nptest.assert_allclose(
+            data['sm_mean'][0:19], sm_mean_should, atol=0.01)
 
     def test_h103_read(self):
         """
         Test read file.
         """
         dt = datetime(2017, 2, 20, 10, 30, 0)
-        path = os.path.join(self.root_path, 'h103')
+        path = self.root_path / 'h103'
         product_id = 'h103'
 
         h103 = AscatNrtBufrFileList(path, product_id)
         data, metadata = h103.read(dt)
 
         sm_should = np.array([
             20.4, 15.2, 4.2, 0., 0.7, 6.8, 14.2, 21.9, 23.7, 17.4, 14.8, 19.8,
@@ -186,28 +183,26 @@
         sm_mean_should = np.array([
             14., 14., 13.8, 13.5, 13.3, 13.1, 12.8, 12.6, 12.6, 12., 12.1,
             12.6, 13.2, 14.1, 13.9, 12.4, 10.9, 10.3, 10.7
         ])
 
         nptest.assert_allclose(data['lat'][0:19], lats_should, atol=1e-5)
         nptest.assert_allclose(data['sm'][0:19], sm_should, atol=0.01)
-        nptest.assert_allclose(data['sm_mean'][0:19],
-                               sm_mean_should,
-                               atol=0.01)
+        nptest.assert_allclose(
+            data['sm_mean'][0:19], sm_mean_should, atol=0.01)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_H14(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test data.
         """
-        self.root_path = os.path.join(os.path.dirname(__file__),
-                                      'ascat_test_data', 'hsaf', 'h14')
+        self.root_path = get_testdata_path() / "hsaf" / "h14"
 
     def test_read(self):
         """
         Test read file.
         """
         dt = datetime(2014, 5, 15, 0)
         h14 = H14GribFileList(self.root_path)
@@ -221,40 +216,37 @@
         for var in data:
             assert data[var].shape == (800, 1600)
 
 
 class Test_AscatSsmDataRecord(unittest.TestCase):
 
     def setUp(self):
-
-        path = os.path.dirname(__file__)
+        path = get_testdata_path()
 
         self.gpi = 3066159
-        self.cdr_path = os.path.join(path, 'ascat_test_data', 'hsaf')
-        self.grid_path = os.path.join(path, 'ascat_test_data', 'hsaf', 'grid')
-        self.static_layer_path = os.path.join(path, 'ascat_test_data', 'hsaf',
-                                              'static_layer')
+        self.cdr_path = path / "hsaf"
+        self.grid_path = str(path / "hsaf" / "grid")
+        self.static_layer_path = str(path / "hsaf" / "static_layer")
 
     def test_read_h25(self):
         """
         Test read H25.
         """
-        self.h25 = AscatSsmDataRecord(os.path.join(self.cdr_path, 'h25'),
-                                      self.grid_path,
-                                      static_layer_path=self.static_layer_path)
+        self.h25 = AscatSsmDataRecord(
+            str(self.cdr_path / 'h25'),
+            self.grid_path,
+            static_layer_path=self.static_layer_path)
 
         data = self.h25.read(self.gpi, absolute_sm=True)
         assert data.attrs['gpi'] == self.gpi
 
-        np.testing.assert_approx_equal(data.attrs['lon'],
-                                       19.03533,
-                                       significant=4)
-        np.testing.assert_approx_equal(data.attrs['lat'],
-                                       70.05438,
-                                       significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lon'], 19.03533, significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lat'], 70.05438, significant=4)
 
         assert len(data) == 7737
         assert data.iloc[15].name.to_pydatetime() == datetime(
             2007, 1, 7, 10, 49, 9, 4)
         assert data.iloc[15]['sm'] == 22
         assert data.iloc[15]['ssf'] == 1
         assert data.iloc[15]['sm_noise'] == 6
@@ -263,49 +255,43 @@
         assert data.iloc[15]['orbit_dir'].decode('utf-8') == 'D'
         assert data.iloc[15]['proc_flag'] == 0
 
         np.testing.assert_equal(data.iloc[15]['abs_sm_gldas'], np.nan)
         np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_gldas'],
                                        np.nan)
 
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_hwsd'],
-                                       0.1078,
-                                       significant=6)
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_hwsd'],
-                                       0.0294,
-                                       significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_hwsd'], 0.1078, significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_noise_hwsd'], 0.0294, significant=6)
 
         assert data.attrs['topo_complex'] == 9
         assert data.attrs['wetland_frac'] == 41
 
-        np.testing.assert_approx_equal(data.attrs['porosity_gldas'],
-                                       np.nan,
-                                       significant=5)
-        np.testing.assert_approx_equal(data.attrs['porosity_hwsd'],
-                                       0.49000001,
-                                       significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_gldas'], np.nan, significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_hwsd'], 0.49000001, significant=5)
 
     def test_read_h108(self):
         """
         Test read H108.
         """
         self.h108 = AscatSsmDataRecord(
-            os.path.join(self.cdr_path, 'h108'),
+            str(self.cdr_path / 'h108'),
             self.grid_path,
             static_layer_path=self.static_layer_path)
 
         data = self.h108.read(self.gpi, absolute_sm=True)
         assert data.attrs['gpi'] == self.gpi
 
-        np.testing.assert_approx_equal(data.attrs['lon'],
-                                       19.03533,
-                                       significant=4)
-        np.testing.assert_approx_equal(data.attrs['lat'],
-                                       70.05438,
-                                       significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lon'], 19.03533, significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lat'], 70.05438, significant=4)
 
         assert len(data) == 8222
         assert data.iloc[15].name.to_pydatetime() == datetime(
             2007, 1, 7, 10, 49, 9, 4)
         assert data.iloc[15]['sm'] == 22
         assert data.iloc[15]['ssf'] == 2
         assert data.iloc[15]['sm_noise'] == 6
@@ -314,47 +300,42 @@
         assert data.iloc[15]['orbit_dir'].decode('utf-8') == 'D'
         assert data.iloc[15]['proc_flag'] == 0
 
         np.testing.assert_equal(data.iloc[15]['abs_sm_gldas'], np.nan)
         np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_gldas'],
                                        np.nan)
 
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_hwsd'],
-                                       0.1078,
-                                       significant=6)
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_hwsd'],
-                                       0.0294,
-                                       significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_hwsd'], 0.1078, significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_noise_hwsd'], 0.0294, significant=6)
 
         assert data.attrs['topo_complex'] == 9
         assert data.attrs['wetland_frac'] == 41
 
         np.testing.assert_equal(data.attrs['porosity_gldas'], np.nan)
-        np.testing.assert_approx_equal(data.attrs['porosity_hwsd'],
-                                       0.49000001,
-                                       significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_hwsd'], 0.49000001, significant=5)
 
     def test_read_h109(self):
         """
         Test read H109.
         """
         self.h109 = AscatSsmDataRecord(
-            os.path.join(self.cdr_path, 'h109'),
+            str(self.cdr_path / 'h109'),
             self.grid_path,
             static_layer_path=self.static_layer_path)
 
         data = self.h109.read(self.gpi, absolute_sm=True)
         assert data.attrs['gpi'] == self.gpi
 
-        np.testing.assert_approx_equal(data.attrs['lon'],
-                                       19.03533,
-                                       significant=4)
-        np.testing.assert_approx_equal(data.attrs['lat'],
-                                       70.05438,
-                                       significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lon'], 19.03533, significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lat'], 70.05438, significant=4)
 
         assert len(data) == 11736
         assert data.iloc[15].name.to_pydatetime() == \
             datetime(2007, 1, 7, 10, 49, 9, 379200)
         assert data.iloc[15]['sm'] == 27
         assert data.iloc[15]['ssf'] == 1
         assert data.iloc[15]['sm_noise'] == 5
@@ -365,47 +346,42 @@
         assert data.iloc[15]['corr_flag'] == 16
         assert data.iloc[15]['sat_id'] == 3
 
         np.testing.assert_equal(data.iloc[15]['abs_sm_gldas'], np.nan)
         np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_gldas'],
                                        np.nan)
 
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_hwsd'],
-                                       0.1323,
-                                       significant=6)
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_hwsd'],
-                                       0.0245,
-                                       significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_hwsd'], 0.1323, significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_noise_hwsd'], 0.0245, significant=6)
 
         assert data.attrs['topo_complex'] == 9
         assert data.attrs['wetland_frac'] == 41
 
         np.testing.assert_equal(data.attrs['porosity_gldas'], np.nan)
-        np.testing.assert_approx_equal(data.attrs['porosity_hwsd'],
-                                       0.49000001,
-                                       significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_hwsd'], 0.49000001, significant=5)
 
     def test_read_h110(self):
         """
         Test read H110.
         """
         self.h110 = AscatSsmDataRecord(
-            os.path.join(self.cdr_path, 'h110'),
+            str(self.cdr_path / 'h110'),
             self.grid_path,
             static_layer_path=self.static_layer_path)
 
         data = self.h110.read(self.gpi, absolute_sm=True)
         assert data.attrs['gpi'] == self.gpi
 
-        np.testing.assert_approx_equal(data.attrs['lon'],
-                                       19.03533,
-                                       significant=4)
-        np.testing.assert_approx_equal(data.attrs['lat'],
-                                       70.05438,
-                                       significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lon'], 19.03533, significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lat'], 70.05438, significant=4)
 
         assert len(data) == 1148
         assert data.iloc[15].name.to_pydatetime() == datetime(
             2016, 1, 3, 19, 34, 28, 99200)
         assert data.iloc[15]['sm'] == 48
         assert data.iloc[15]['ssf'] == 1
         assert data.iloc[15]['sm_noise'] == 5
@@ -416,47 +392,42 @@
         assert data.iloc[15]['corr_flag'] == 0
         assert data.iloc[15]['sat_id'] == 4
 
         np.testing.assert_equal(data.iloc[15]['abs_sm_gldas'], np.nan)
         np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_gldas'],
                                        np.nan)
 
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_hwsd'],
-                                       0.2352,
-                                       significant=6)
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_hwsd'],
-                                       0.0245,
-                                       significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_hwsd'], 0.2352, significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_noise_hwsd'], 0.0245, significant=6)
 
         assert data.attrs['topo_complex'] == 9
         assert data.attrs['wetland_frac'] == 41
 
         np.testing.assert_equal(data.attrs['porosity_gldas'], np.nan)
-        np.testing.assert_approx_equal(data.attrs['porosity_hwsd'],
-                                       0.49000001,
-                                       significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_hwsd'], 0.49000001, significant=5)
 
     def test_read_h111(self):
         """
         Test read H111.
         """
         self.h111 = AscatSsmDataRecord(
-            os.path.join(self.cdr_path, 'h111'),
+            str(self.cdr_path / 'h111'),
             self.grid_path,
             static_layer_path=self.static_layer_path)
 
         data = self.h111.read(self.gpi, absolute_sm=True)
         assert data.attrs['gpi'] == self.gpi
 
-        np.testing.assert_approx_equal(data.attrs['lon'],
-                                       19.03533,
-                                       significant=4)
-        np.testing.assert_approx_equal(data.attrs['lat'],
-                                       70.05438,
-                                       significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lon'], 19.03533, significant=4)
+        np.testing.assert_approx_equal(
+            data.attrs['lat'], 70.05438, significant=4)
 
         assert len(data) == 13715
         assert data.iloc[15].name.to_pydatetime() == datetime(
             2007, 1, 7, 10, 49, 9, 379200)
         assert data.iloc[15]['sm'] == 28
         assert data.iloc[15]['ssf'] == 1
         assert data.iloc[15]['sm_noise'] == 5
@@ -467,37 +438,34 @@
         assert data.iloc[15]['corr_flag'] == 4
         assert data.iloc[15]['sat_id'] == 3
 
         np.testing.assert_equal(data.iloc[15]['abs_sm_gldas'], np.nan)
         np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_gldas'],
                                        np.nan)
 
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_hwsd'],
-                                       0.1372,
-                                       significant=6)
-        np.testing.assert_approx_equal(data.iloc[15]['abs_sm_noise_hwsd'],
-                                       0.0245,
-                                       significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_hwsd'], 0.1372, significant=6)
+        np.testing.assert_approx_equal(
+            data.iloc[15]['abs_sm_noise_hwsd'], 0.0245, significant=6)
 
         assert data.attrs['topo_complex'] == 9
         assert data.attrs['wetland_frac'] == 41
 
         np.testing.assert_equal(data.attrs['porosity_gldas'], np.nan)
-        np.testing.assert_approx_equal(data.attrs['porosity_hwsd'],
-                                       0.49000001,
-                                       significant=5)
+        np.testing.assert_approx_equal(
+            data.attrs['porosity_hwsd'], 0.49000001, significant=5)
 
     def test_read_2points_cell_switch(self):
         """
         Test reading of two points in two different cells.
         This did not work in the past when the static layer class
         was closed too soon.
         """
         self.h111 = AscatSsmDataRecord(
-            os.path.join(self.cdr_path, 'h111'),
+            str(self.cdr_path / 'h111'),
             self.grid_path,
             static_layer_path=self.static_layer_path)
 
         gpi = 3066159
         data = self.h111.read(gpi, absolute_sm=True)
         assert data.attrs['gpi'] == gpi
```

### Comparing `ascat-2.3.1/tests/test_level1.py` & `ascat-2.4.0/tests/test_level1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -24,66 +24,47 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 Test ASCAT Level 1 reader.
 """
 
-import os
 import sys
 import pytest
 import unittest
 from datetime import datetime
 
 import numpy as np
 import numpy.testing as nptest
 
 from ascat.eumetsat.level1 import AscatL1bFile
 from ascat.eumetsat.level1 import AscatL1bNcFileList
 from ascat.eumetsat.level1 import AscatL1bEpsFileList
 from ascat.eumetsat.level1 import AscatL1bBufrFileList
 from ascat.eumetsat.level1 import AscatL1bHdf5FileList
 
+from get_path import get_testdata_path
+
 float32_nan = -999999.
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL1bFile(unittest.TestCase):
 
     def setUp(self):
-        data_path = os.path.join(os.path.dirname(__file__), "ascat_test_data",
-                                 "eumetsat", "ASCAT_generic_reader_data")
+        data_path = get_testdata_path(
+        ) / "eumetsat" / "ASCAT_generic_reader_data"
 
-        name_b = os.path.join(
-            data_path, "bufr",
-            "M02-ASCA-ASCSZR1B0200-NA-9.1-20100609013900.000000000Z-20130824233100-1280350.bfr"
-        )
-        name_e = os.path.join(
-            data_path, "eps_nat",
-            "ASCA_SZR_1B_M02_20100609013900Z_20100609032058Z_R_O_20130824233100Z.nat"
-        )
-        name_n = os.path.join(
-            data_path, "nc",
-            "W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20100609013900_18872_eps_o_125_l1.nc"
-        )
-
-        name_e11 = os.path.join(
-            data_path, "eps_nat",
-            "ASCA_SZR_1B_M02_20071212071500Z_20071212085659Z_R_O_20081225063118Z.nat"
-        )
-
-        name_e_szf = os.path.join(
-            data_path, "eps_nat",
-            "ASCA_SZF_1B_M01_20180611041800Z_20180611055959Z_N_O_20180611050637Z.nat"
-        )
-
-        name_h = os.path.join(
-            data_path, "hdf5",
-            "ASCA_SZF_1B_M01_20180611041800Z_20180611055959Z_N_O_20180611050637Z.h5"
-        )
+        name_b = data_path / "bufr" / "M02-ASCA-ASCSZR1B0200-NA-9.1-20100609013900.000000000Z-20130824233100-1280350.bfr"
+        name_e = data_path / "eps_nat" / "ASCA_SZR_1B_M02_20100609013900Z_20100609032058Z_R_O_20130824233100Z.nat"
+        name_n = data_path / "nc" / "W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20100609013900_18872_eps_o_125_l1.nc"
+
+        name_e11 = data_path / "eps_nat" / "ASCA_SZR_1B_M02_20071212071500Z_20071212085659Z_R_O_20081225063118Z.nat"
+        name_e_szf = data_path / "eps_nat" / "ASCA_SZF_1B_M01_20180611041800Z_20180611055959Z_N_O_20180611050637Z.nat"
+        name_h = data_path / "hdf5" / "ASCA_SZF_1B_M01_20180611041800Z_20180611055959Z_N_O_20180611050637Z.h5"
 
         self.bufr = AscatL1bFile(name_b)
         self.nc = AscatL1bFile(name_n)
 
         self.eps = AscatL1bFile(name_e)
         self.eps_fmv11 = AscatL1bFile(name_e11)
 
@@ -142,22 +123,24 @@
         hdf5_fields = [
             "sigma0_full", "inc_angle_full", "as_des_pass", "land_frac",
             "swath_indicator"
         ]
 
         for antenna in ["lf-vv", "lm-vv", "la-vv", "rf-vv", "rm-vv", "ra-vv"]:
             for coord in ["lon", "lat"]:
-                nptest.assert_allclose(eps_data[antenna][coord],
-                                       h5_data[antenna][coord],
-                                       atol=1e-4)
+                nptest.assert_allclose(
+                    eps_data[antenna][coord],
+                    h5_data[antenna][coord],
+                    atol=1e-4)
 
             for eps_field, hdf5_field in zip(eps_fields, hdf5_fields):
-                nptest.assert_allclose(eps_data[antenna][eps_field],
-                                       h5_data[antenna][hdf5_field],
-                                       atol=0.1)
+                nptest.assert_allclose(
+                    eps_data[antenna][eps_field],
+                    h5_data[antenna][hdf5_field],
+                    atol=0.1)
 
     def test_szx_eps(self):
         """
         Test read SZX EPS.
         """
         self.reader, metadata = self.eps.read(generic=True)
 
@@ -199,17 +182,16 @@
             "2010-06-09T01:39:00.000", "2010-06-09T01:39:01.874",
             "2010-06-09T01:39:01.874", "2010-06-09T01:39:01.874"
         ],
                             dtype="datetime64[ms]")
 
         nptest.assert_allclose(self.reader["lat"][:25], lat_should, atol=1e-5)
         nptest.assert_allclose(self.reader["lon"][:25], lon_should, atol=1e-5)
-        nptest.assert_allclose(self.reader["sig"][:25, 0],
-                               sig_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            self.reader["sig"][:25, 0], sig_should, atol=1e-5)
         nptest.assert_allclose(self.reader["kp"][:25, 0], kp_should, atol=1e-5)
         nptest.assert_equal(self.reader["time"][75:85], t_should)
 
     def test_szx_eps_fmv11(self):
         """
         Test read SZX EPS format version 11.
         """
@@ -253,17 +235,16 @@
             "2007-12-12T07:15:00.000", "2007-12-12T07:15:01.876",
             "2007-12-12T07:15:01.876", "2007-12-12T07:15:01.876"
         ],
                             dtype="datetime64[ms]")
 
         nptest.assert_allclose(self.reader["lat"][:25], lat_should, atol=1e-5)
         nptest.assert_allclose(self.reader["lon"][:25], lon_should, atol=1e-5)
-        nptest.assert_allclose(self.reader["sig"][:25, 0],
-                               sig_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            self.reader["sig"][:25, 0], sig_should, atol=1e-5)
         nptest.assert_allclose(self.reader["kp"][:25, 0], kp_should, atol=1e-5)
         nptest.assert_equal(self.reader["time"][75:85], t_should)
 
     def test_szf_eps(self):
         """
         Test read SZF EPS format.
         """
@@ -298,62 +279,59 @@
             "2018-06-11T04:18:01.479", "2018-06-11T04:18:01.479",
             "2018-06-11T04:18:01.479", "2018-06-11T04:18:01.479",
             "2018-06-11T04:18:01.479", "2018-06-11T04:18:01.479",
             "2018-06-11T04:18:01.479", "2018-06-11T04:18:01.479"
         ],
                             dtype="datetime64[ms]")
 
-        nptest.assert_allclose(self.reader["lf-vv"]["lat"][:25],
-                               lat_should,
-                               atol=1e-5)
-        nptest.assert_allclose(self.reader["lf-vv"]["lon"][:25],
-                               lon_should,
-                               atol=1e-5)
-        nptest.assert_allclose(self.reader["lf-vv"]["sig"][:25],
-                               sig_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            self.reader["lf-vv"]["lat"][:25], lat_should, atol=1e-5)
+        nptest.assert_allclose(
+            self.reader["lf-vv"]["lon"][:25], lon_should, atol=1e-5)
+        nptest.assert_allclose(
+            self.reader["lf-vv"]["sig"][:25], sig_should, atol=1e-5)
         nptest.assert_equal(self.reader["lf-vv"]["time"][190:200], t_should)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL1bFileList(unittest.TestCase):
     """
     Test read AscatL1bFileList in various formats.
     """
 
     def setUp(self):
         """
         Setup test data.
         """
-        root_path = os.path.join(os.path.dirname(__file__), "ascat_test_data",
-                                 "eumetsat", "ASCAT_generic_reader_data")
+        root_path = get_testdata_path(
+        ) / "eumetsat" / "ASCAT_generic_reader_data"
 
-        path = os.path.join(root_path, "bufr")
+        path = root_path / "bufr"
         sat = "a"
         product = "szr"
         self.bufr_szr = AscatL1bBufrFileList(path, sat, product)
 
-        path = os.path.join(root_path, "nc")
+        path = root_path / "nc"
         sat = "a"
         product = "szr"
         self.nc_szr = AscatL1bNcFileList(path, sat, product)
 
-        path = os.path.join(root_path, "eps_nat")
+        path = root_path / "eps_nat"
         sat = "a"
         product = "szr"
         self.eps_szr = AscatL1bEpsFileList(path, sat, product)
 
         sat = "b"
         product = "szf"
-        path = os.path.join(root_path, "eps_nat")
+        path = root_path / "eps_nat"
         self.eps_szf = AscatL1bEpsFileList(path, sat, product)
 
         sat = "b"
         product = "szf"
-        path = os.path.join(root_path, "hdf5")
+        path = root_path / "hdf5"
         self.hdf5_szf = AscatL1bHdf5FileList(path, sat, product)
 
     def test_szr_read_date(self):
         """
         Test read date for SZR formats.
         """
         dt = datetime(2010, 6, 9, 1, 39, 0)
@@ -395,25 +373,22 @@
     def test_szr_read_period(self):
         """
         Test read period for SZR formats.
         """
         dt_start = datetime(2010, 6, 9, 1, 39, 0)
         dt_end = datetime(2010, 6, 9, 2, 0, 0)
 
-        date_str = "%Y%m%d%H%M%S"
+        date_field_fmt = "%Y%m%d%H%M%S"
 
-        bufr_data, bufr_metadata = self.bufr_szr.read_period(dt_start,
-                                                             dt_end,
-                                                             date_str=date_str)
-        nc_data, nc_metadata = self.nc_szr.read_period(dt_start,
-                                                       dt_end,
-                                                       date_str=date_str)
-        eps_data, eps_metadata = self.eps_szr.read_period(dt_start,
-                                                          dt_end,
-                                                          date_str=date_str)
+        bufr_data, bufr_metadata = self.bufr_szr.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
+        nc_data, nc_metadata = self.nc_szr.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
+        eps_data, eps_metadata = self.eps_szr.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
 
         for f in ["lat", "lon"]:
             nptest.assert_allclose(bufr_data[f], eps_data[f], atol=1e-2)
             nptest.assert_allclose(eps_data[f], nc_data[f], atol=1e-2)
             nptest.assert_allclose(nc_data[f], bufr_data[f], atol=1e-2)
 
         matching = [
@@ -430,17 +405,16 @@
         # BUFR contain less accurate data so we only compare 0.1 accuracy.
         for field in matching:
             nan_mask = (nc_data[field] == float32_nan)
             eps_data[field][nan_mask] = float32_nan
             bufr_data[field][nan_mask] = float32_nan
             valid = ((eps_data[field] > -25))
 
-            nptest.assert_allclose(bufr_data[field][valid],
-                                   eps_data[field][valid],
-                                   atol=0.1)
+            nptest.assert_allclose(
+                bufr_data[field][valid], eps_data[field][valid], atol=0.1)
 
     def test_szf_read_date(self):
         """
         Test read date for SZF formats.
         """
         dt = datetime(2018, 6, 11, 4, 18, 0)
 
@@ -454,50 +428,52 @@
         hdf5_fields = [
             "sigma0_full", "inc_angle_full", "as_des_pass", "land_frac",
             "swath_indicator"
         ]
 
         for antenna in ["lf-vv", "lm-vv", "la-vv", "rf-vv", "rm-vv", "ra-vv"]:
             for coord in ["lon", "lat"]:
-                nptest.assert_allclose(eps_data[antenna][coord],
-                                       hdf5_data[antenna][coord],
-                                       atol=1e-4)
+                nptest.assert_allclose(
+                    eps_data[antenna][coord],
+                    hdf5_data[antenna][coord],
+                    atol=1e-4)
 
             for eps_field, hdf5_field in zip(eps_fields, hdf5_fields):
-                nptest.assert_allclose(eps_data[antenna][eps_field],
-                                       hdf5_data[antenna][hdf5_field],
-                                       atol=0.1)
+                nptest.assert_allclose(
+                    eps_data[antenna][eps_field],
+                    hdf5_data[antenna][hdf5_field],
+                    atol=0.1)
 
     def test_szf_read_period(self):
         """
         Test read period for SZF formats.
         """
         dt_start = datetime(2018, 6, 11, 4, 18, 0)
         dt_end = datetime(2018, 6, 11, 4, 19, 0)
 
-        date_str = "%Y%m%d%H%M%S"
-        eps_data, eps_metadata = self.eps_szf.read_period(dt_start,
-                                                          dt_end,
-                                                          date_str=date_str)
-        hdf5_data, hdf5_metadata = self.hdf5_szf.read_period(dt_start,
-                                                             dt_end,
-                                                             date_str=date_str)
+        date_field_fmt = "%Y%m%d%H%M%S"
+        eps_data, eps_metadata = self.eps_szf.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
+        hdf5_data, hdf5_metadata = self.hdf5_szf.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
 
         for antenna in ["lf-vv", "lm-vv", "la-vv", "rf-vv", "rm-vv", "ra-vv"]:
             for coord in ["lon", "lat"]:
-                nptest.assert_allclose(eps_data[antenna][coord],
-                                       hdf5_data[antenna][coord],
-                                       atol=1e-4)
+                nptest.assert_allclose(
+                    eps_data[antenna][coord],
+                    hdf5_data[antenna][coord],
+                    atol=1e-4)
 
             matching = [
                 "sig", "inc", "azi", "sat_id", "as_des_pass", "land_frac",
                 "f_usable", "f_land", "beam_number", "swath_indicator"
             ]
 
             for field in matching:
-                nptest.assert_allclose(eps_data[antenna][coord],
-                                       hdf5_data[antenna][coord],
-                                       atol=0.1)
+                nptest.assert_allclose(
+                    eps_data[antenna][coord],
+                    hdf5_data[antenna][coord],
+                    atol=0.1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ascat-2.3.1/tests/test_level2.py` & `ascat-2.4.0/tests/test_level2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, TU Wien, Department of Geodesy and Geoinformation
+# Copyright (c) 2024, TU Wien
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #    * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 #    * Redistributions in binary form must reproduce the above copyright
@@ -40,37 +40,33 @@
 from ascat.read_native.bufr import AscatL2BufrFile
 from ascat.read_native.nc import AscatL2NcFile
 from ascat.eumetsat.level2 import AscatL2File
 from ascat.eumetsat.level2 import AscatL2NcFileList
 from ascat.eumetsat.level2 import AscatL2BufrFileList
 from ascat.eumetsat.level2 import AscatL2EpsFileList
 
+from get_path import get_testdata_path
+
 eps_float_nan = -2147483648.
 bufr_float_nan = 1.7e+38
 uint8_nan = np.iinfo(np.uint8).max
 uint16_nan = np.iinfo(np.uint16).max
 float32_nan = -999999.
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL2BufrFile(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test files.
         """
-        data_path = os.path.join(os.path.dirname(__file__), 'ascat_test_data',
-                                 'eumetsat', 'ASCAT_L2_SM_125', 'bufr',
-                                 'Metop_B')
-
-        fname = os.path.join(
-            data_path,
-            'M01-ASCA-ASCSMR02-NA-5.0-20170220050900.000000000Z-20170220055833-1207110.bfr'
-        )
-
+        data_path = get_testdata_path(
+        ) / "eumetsat/ASCAT_L2_SM_125/bufr/Metop_B"
+        fname = data_path / 'M01-ASCA-ASCSMR02-NA-5.0-20170220050900.000000000Z-20170220055833-1207110.bfr'
         self.reader = AscatL2BufrFile(fname)
 
     def test_read(self):
         """
         Test read.
         """
         data, metadata = self.reader.read()
@@ -91,35 +87,30 @@
         ssm_mean_should = np.array([
             36.7, 35.4, 33.4, 32.5, 32.5, 32., 31.2, 29.4, 28.7, 27.6, 25.8,
             25.4, 25.5, 25.3, 24.4, 23.4, 22.3, 21.3, 20.4, 20.4, 19.9, 19.7,
             20.3, 21.5, 22.9
         ])
 
         nptest.assert_allclose(data['lat'][:25], lats_should, atol=1e-5)
-        nptest.assert_allclose(data['Surface Soil Moisture (Ms)'][:25],
-                               ssm_should,
-                               atol=1e-5)
-        nptest.assert_allclose(data['Mean Surface Soil Moisture'][:25],
-                               ssm_mean_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            data['Surface Soil Moisture (Ms)'][:25], ssm_should, atol=1e-5)
+        nptest.assert_allclose(
+            data['Mean Surface Soil Moisture'][:25],
+            ssm_mean_should,
+            atol=1e-5)
 
 
 class Test_AscatL2NcFile(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test files.
         """
-        data_path = os.path.join(os.path.dirname(__file__), 'ascat_test_data',
-                                 'eumetsat', 'ASCAT_L2_SM_125', 'nc',
-                                 'Metop_A')
-        fname = os.path.join(
-            data_path,
-            'W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20170220041500_53652_eps_o_125_ssm_l2.nc'
-        )
+        data_path = get_testdata_path() / "eumetsat/ASCAT_L2_SM_125/nc/Metop_A"
+        fname = data_path / 'W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20170220041500_53652_eps_o_125_ssm_l2.nc'
         self.reader = AscatL2NcFile(fname)
 
     def test_read(self):
         """
         Test read.
         """
         data, metadata = self.reader.read()
@@ -143,82 +134,93 @@
             24.51000023, 26.01000023, 27.04999924, 26.94999886, 26.63999939,
             27.09999847, 27.56999969, 27.43000031, 26.64999962, 26.53999901,
             27.48999977, 28.20999908, 28.38999939, 28.79999924, 29.21999931,
             30.01000023, 30.97999954, 31.27999878, 31.8599987, 32.05999756
         ])
 
         nptest.assert_allclose(data['latitude'][:25], lats_should, atol=1e-5)
-        nptest.assert_allclose(data['soil_moisture'][:25],
-                               ssm_should,
-                               atol=1e-5)
-        nptest.assert_allclose(data['mean_soil_moisture'][:25],
-                               ssm_mean_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            data['soil_moisture'][:25], ssm_should, atol=1e-5)
+        nptest.assert_allclose(
+            data['mean_soil_moisture'][:25], ssm_mean_should, atol=1e-5)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL2NcFile_AscatL2BufrFile(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test files.
         """
-        data_path = os.path.join(os.path.dirname(__file__), 'ascat_test_data',
-                                 'eumetsat', 'ASCAT_L2_SM_125')
-        fname_nc = os.path.join(
-            data_path, 'nc', 'Metop_A',
-            'W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20170220041500_53652_eps_o_125_ssm_l2.nc'
-        )
+        data_path = get_testdata_path() / "eumetsat/ASCAT_L2_SM_125"
+
+        fname_nc = data_path / "nc/Metop_A/W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPA+ASCAT_C_EUMP_20170220041500_53652_eps_o_125_ssm_l2.nc"
         self.reader_nc = AscatL2NcFile(fname_nc)
 
-        fname_bufr = os.path.join(
-            data_path, 'bufr', 'Metop_A',
-            'M02-ASCA-ASCSMR02-NA-5.0-20170220041500.000000000Z-20170220055656-1207110.bfr'
-        )
+        fname_bufr = data_path / "bufr/Metop_A/M02-ASCA-ASCSMR02-NA-5.0-20170220041500.000000000Z-20170220055656-1207110.bfr"
         self.reader_bufr = AscatL2BufrFile(fname_bufr)
 
     def test_read(self):
         """
         Test read.
         """
         data_nc, metadata = self.reader_nc.read()
         data_bufr, metadata = self.reader_bufr.read()
 
-        nptest.assert_allclose(data_nc['latitude'],
-                               data_bufr['lat'],
-                               atol=1e-4)
+        nptest.assert_allclose(
+            data_nc['latitude'], data_bufr['lat'], atol=1e-4)
 
         nc_bufr_matching = {
-            'slope40': 'Slope At 40 Deg Incidence Angle',
+            'slope40':
+                'Slope At 40 Deg Incidence Angle',
             'sigma40_error':
-            'Estimated Error In Sigma0 At 40 Deg Incidence Angle',
-            'utc_line_nodes': None,
-            'wet_backscatter': 'Wet Backscatter',
-            'swath_indicator': None,
-            'frozen_soil_probability': 'Frozen Land Surface Fraction',
-            'wetland_flag': 'Inundation And Wetland Fraction',
+                'Estimated Error In Sigma0 At 40 Deg Incidence Angle',
+            'utc_line_nodes':
+                None,
+            'wet_backscatter':
+                'Wet Backscatter',
+            'swath_indicator':
+                None,
+            'frozen_soil_probability':
+                'Frozen Land Surface Fraction',
+            'wetland_flag':
+                'Inundation And Wetland Fraction',
             # The processing flag definition between BUFR and netCDF is slightly different
             # 'proc_flag1': 'Soil Moisture Processing Flag',
-            'proc_flag2': None,
-            'abs_line_number': None,
-            'sat_track_azi': None,
-            'sigma40': 'Backscatter',
-            'soil_moisture': 'Surface Soil Moisture (Ms)',
-            'soil_moisture_error': 'Estimated Error In Surface Soil Moisture',
+            'proc_flag2':
+                None,
+            'abs_line_number':
+                None,
+            'sat_track_azi':
+                None,
+            'sigma40':
+                'Backscatter',
+            'soil_moisture':
+                'Surface Soil Moisture (Ms)',
+            'soil_moisture_error':
+                'Estimated Error In Surface Soil Moisture',
             # 'rainfall_flag': 'Rain Fall Detection',
-            'soil_moisture_sensitivity': 'Soil Moisture Sensitivity',
-            'corr_flags': 'Soil Moisture Correction Flag',
-            'dry_backscatter': 'Dry Backscatter',
-            'aggregated_quality_flag': None,
-            'mean_soil_moisture': 'Mean Surface Soil Moisture',
-            'as_des_pass': None,
+            'soil_moisture_sensitivity':
+                'Soil Moisture Sensitivity',
+            'corr_flags':
+                'Soil Moisture Correction Flag',
+            'dry_backscatter':
+                'Dry Backscatter',
+            'aggregated_quality_flag':
+                None,
+            'mean_soil_moisture':
+                'Mean Surface Soil Moisture',
+            'as_des_pass':
+                None,
             'slope40_error':
-            'Estimated Error In Slope At 40 Deg Incidence Angle',
-            'topography_flag': 'Topographic Complexity',
-            'snow_cover_probability': 'Snow Cover'
+                'Estimated Error In Slope At 40 Deg Incidence Angle',
+            'topography_flag':
+                'Topographic Complexity',
+            'snow_cover_probability':
+                'Snow Cover'
         }
 
         # BUFR contains less accurate data so we only compare to 0.1
         for nc_name in nc_bufr_matching:
 
             bufr_name = nc_bufr_matching[nc_name]
             if bufr_name is None:
@@ -238,41 +240,30 @@
                          & (~np.isnan(data_bufr[bufr_name])))
             else:
                 valid = ((data_nc[nc_name] != eps_float_nan)
                          & (~np.isnan(data_nc[nc_name]))
                          & (data_bufr[bufr_name] != bufr_float_nan)
                          & (~np.isnan(data_bufr[bufr_name])))
 
-            nptest.assert_allclose(data_nc[nc_name][valid],
-                                   data_bufr[bufr_name][valid],
-                                   atol=0.1)
+            nptest.assert_allclose(
+                data_nc[nc_name][valid], data_bufr[bufr_name][valid], atol=0.1)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL2File(unittest.TestCase):
 
     def setUp(self):
         """
         Setup test files.
         """
-        data_path = os.path.join(os.path.dirname(__file__), 'ascat_test_data',
-                                 'eumetsat', 'ASCAT_generic_reader_data')
+        data_path = get_testdata_path() / "eumetsat/ASCAT_generic_reader_data"
 
-        name_b = os.path.join(
-            data_path, 'bufr',
-            'M01-ASCA-ASCSMO02-NA-5.0-20180612035700.000000000Z-20180612044530-1281300.bfr'
-        )
-        name_e = os.path.join(
-            data_path, 'eps_nat',
-            'ASCA_SMO_02_M01_20180612035700Z_20180612053856Z_N_O_20180612044530Z.nat'
-        )
-        name_n = os.path.join(
-            data_path, 'nc',
-            'W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPB+ASCAT_C_EUMP_20180612035700_29742_eps_o_250_ssm_l2.nc'
-        )
+        name_b = data_path / "bufr/M01-ASCA-ASCSMO02-NA-5.0-20180612035700.000000000Z-20180612044530-1281300.bfr"
+        name_e = data_path / "eps_nat/ASCA_SMO_02_M01_20180612035700Z_20180612053856Z_N_O_20180612044530Z.nat"
+        name_n = data_path / "nc/W_XX-EUMETSAT-Darmstadt,SURFACE+SATELLITE,METOPB+ASCAT_C_EUMP_20180612035700_29742_eps_o_250_ssm_l2.nc"
 
         self.bufr = AscatL2File(name_b)
         self.eps = AscatL2File(name_e)
         self.nc = AscatL2File(name_n)
 
     def test_read_all_formats(self):
         """
@@ -358,44 +349,42 @@
             '2018-06-12T03:57:03.750', '2018-06-12T03:57:03.750'
         ],
                             dtype='datetime64[ms]')
 
         nptest.assert_allclose(eps_ds['lat'][:25], lat_should, atol=1e-5)
         nptest.assert_allclose(eps_ds['lon'][:25], lon_should, atol=1e-5)
         nptest.assert_allclose(eps_ds['sm'][:25], sm_should, atol=1e-5)
-        nptest.assert_allclose(eps_ds['sm_mean'][:25],
-                               sm_mean_should,
-                               atol=1e-5)
+        nptest.assert_allclose(
+            eps_ds['sm_mean'][:25], sm_mean_should, atol=1e-5)
         nptest.assert_equal(eps_ds['time'][35:45], t_should)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason="Does not work on Windows")
 class Test_AscatL2FileList(unittest.TestCase):
     """
     Test read AscatL2FileList in various formats.
     """
 
     def setUp(self):
         """
         Setup test data.
         """
-        root_path = os.path.join(os.path.dirname(__file__), 'ascat_test_data',
-                                 'eumetsat', 'ASCAT_generic_reader_data')
+        root_path = get_testdata_path() / "eumetsat/ASCAT_generic_reader_data"
 
-        path = os.path.join(root_path, 'bufr')
+        path = root_path / 'bufr'
         sat = 'b'
         product = 'smo'
         self.bufr_smo = AscatL2BufrFileList(path, sat, product)
 
-        path = os.path.join(root_path, 'nc')
+        path = root_path / 'nc'
         sat = 'b'
         product = 'smo'
         self.nc_smo = AscatL2NcFileList(path, sat, product)
 
-        path = os.path.join(root_path, 'eps_nat')
+        path = root_path / 'eps_nat'
         sat = 'b'
         product = 'smo'
         self.eps_smo = AscatL2EpsFileList(path, sat, product)
 
     def test_smo_read_date(self):
         """
         Test read date for SMO formats.
@@ -403,39 +392,39 @@
         dt = datetime(2018, 6, 12, 3, 57, 0)
 
         bufr_data, metadata = self.bufr_smo.read(dt)
         nc_data, metadata = self.nc_smo.read(dt)
         eps_data, metadata = self.eps_smo.read(dt)
 
         for coord in ['lon', 'lat']:
-            nptest.assert_allclose(bufr_data[coord],
-                                   eps_data[coord],
-                                   atol=1e-4)
+            nptest.assert_allclose(
+                bufr_data[coord], eps_data[coord], atol=1e-4)
             nptest.assert_allclose(eps_data[coord], nc_data[coord], atol=1e-4)
             nptest.assert_allclose(nc_data[coord], bufr_data[coord], atol=1e-4)
 
     def test_smo_read_period(self):
         """
         Test read period for SMO formats.
         """
         dt_start = datetime(2018, 6, 12, 4, 0, 0)
         dt_end = datetime(2018, 6, 12, 4, 13, 0)
 
+        date_field_fmt = "%Y%m%d%H%M%S"
+
         bufr_data, metadata = self.bufr_smo.read_period(
-            dt_start, dt_end, date_str="%Y%m%d%H%M%S")
-        nc_data, metadata = self.nc_smo.read_period(dt_start,
-                                                    dt_end,
-                                                    date_str="%Y%m%d%H%M%S")
-        eps_data, metadata = self.eps_smo.read_period(dt_start,
-                                                      dt_end,
-                                                      date_str="%Y%m%d%H%M%S")
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
+
+        nc_data, metadata = self.nc_smo.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
+
+        eps_data, metadata = self.eps_smo.read_period(
+            dt_start, dt_end, date_field_fmt=date_field_fmt)
 
         for coord in ['lon', 'lat']:
-            nptest.assert_allclose(bufr_data[coord],
-                                   eps_data[coord],
-                                   atol=1e-4)
+            nptest.assert_allclose(
+                bufr_data[coord], eps_data[coord], atol=1e-4)
             nptest.assert_allclose(eps_data[coord], nc_data[coord], atol=1e-4)
             nptest.assert_allclose(nc_data[coord], bufr_data[coord], atol=1e-4)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ascat-2.3.1/tox.ini` & `ascat-2.4.0/tox.ini`

 * *Files identical despite different names*

