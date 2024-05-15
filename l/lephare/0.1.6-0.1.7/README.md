# Comparing `tmp/lephare-0.1.6.tar.gz` & `tmp/lephare-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.6.tar", last modified: Fri May 10 23:27:27 2024, max compression
+gzip compressed data, was "lephare-0.1.7.tar", last modified: Wed May 15 03:33:57 2024, max compression
```

## Comparing `lephare-0.1.6.tar` & `lephare-0.1.7.tar`

### file list

```diff
@@ -1,262 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-10 23:27:21.000000 lephare-0.1.6/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-10 23:27:21.000000 lephare-0.1.6/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-10 23:27:21.000000 lephare-0.1.6/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.591685 lephare-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/compile-cpp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-10 23:27:21.000000 lephare-0.1.6/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 23:27:21.000000 lephare-0.1.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-10 23:27:21.000000 lephare-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 23:27:21.000000 lephare-0.1.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-10 23:27:21.000000 lephare-0.1.6/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-10 23:27:21.000000 lephare-0.1.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 23:27:21.000000 lephare-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-10 23:27:27.627685 lephare-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-10 23:27:21.000000 lephare-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/doxygen/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/keywords.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/legacy_install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Building_list_of_onesources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Data_retrieval.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_SED_manipulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_cosmo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_full_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Example_of_usage_of_magSvc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Minimal_photoz_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/docs/notebooks/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/COSMOS_first100specz.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks/data/output.para
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 23:27:21.000000 lephare-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.595685 lephare-0.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/figuresLPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/figuresLPZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-10 23:27:21.000000 lephare-0.1.6/examples/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-10 23:27:21.000000 lephare-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:27:27.627685 lephare-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-10 23:27:21.000000 lephare-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.587685 lephare-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.599686 lephare-0.1.6/src/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_flt.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_photoz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/filterSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/magSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/mag_gal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/sedtolib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lephare/zphota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/src/lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:27:27.000000 lephare-0.1.6/src/lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/PDF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/PDF.h
--rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SED.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SED.h
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SEDLib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/SEDLib.h
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/_bindings.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/cosmology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/cosmology.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/ext_curv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/filter_extinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/flt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/flt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/globals.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/globals.h
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/keyword.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/keyword.h
--rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag.h
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/mag_gal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/oneElLambda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/oneElLambda.h
--rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/onesource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/onesource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/opa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/opa.h
--rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/photoz_lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/photoz_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/sedtolib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-10 23:27:21.000000 lephare-0.1.6/src/lib/zphota.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/alloutputkeys.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/calzetti.dat
--rw-r--r--   0 runner    (1001) docker     (127)    84794 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/example.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/COSMOS.para
--rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/COSMOS_first100specz.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/examples/output.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/ext/
--rwxr-xr-x   0 runner    (1001) docker     (127)   104052 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/ext/MW_seaton.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)    72411 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/ext/SB_calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.587685 lephare-0.1.6/tests/data/filt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.607685 lephare-0.1.6/tests/data/filt/subaru/
--rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/filt/subaru/IB527.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/opa/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/OPACITY.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau00.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau01.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau02.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau03.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau04.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau05.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau06.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau07.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau08.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau09.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau10.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau11.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau12.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau13.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau14.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau15.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau16.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau17.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau18.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau19.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau20.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau21.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau22.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau23.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau24.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau25.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau26.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau27.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau28.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau29.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau30.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau31.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau32.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau33.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau34.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau35.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau36.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau37.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau38.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau39.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau40.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau41.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau42.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau43.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau44.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau45.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau46.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau47.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau48.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau49.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau50.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau51.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau52.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau53.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau54.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau55.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau56.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau57.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau58.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau59.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau60.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau61.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau62.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau63.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau64.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau65.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau66.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau67.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau68.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau69.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau70.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau71.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau72.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau73.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau74.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau75.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau76.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau77.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau78.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau79.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/opa/tau80.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/GAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/GAL/o5v.sed.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/QSO/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/QSO/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/QSO/o5v.sed.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.623685 lephare-0.1.6/tests/data/sed/STAR/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/STAR/ONE_SED.list
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/STAR/o5v.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/WDgd71.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/sed/o5v.sed.ext
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/tau10.out
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/test_data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/test_file_names.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/tests/data/vega/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1592 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/BD+17.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)     3957 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/BD+17o4708.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/SunLCB.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/VegaLCB.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   100244 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/a0v.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    93156 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/data/vega/a0v_n.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:27:27.627685 lephare-0.1.6/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_data_retrieval_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_oneElLambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_onesource.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_sed.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-10 23:27:21.000000 lephare-0.1.6/tests/lephare/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.069474 lephare-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 03:33:50.000000 lephare-0.1.7/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 03:33:50.000000 lephare-0.1.7/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 03:33:50.000000 lephare-0.1.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 03:33:50.000000 lephare-0.1.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.025474 lephare-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.025474 lephare-0.1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.029474 lephare-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/compile-cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-15 03:33:50.000000 lephare-0.1.7/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-15 03:33:50.000000 lephare-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 03:33:50.000000 lephare-0.1.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-15 03:33:50.000000 lephare-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-15 03:33:50.000000 lephare-0.1.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-15 03:33:50.000000 lephare-0.1.7/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-15 03:33:50.000000 lephare-0.1.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 03:33:50.000000 lephare-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-15 03:33:57.069474 lephare-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 03:33:50.000000 lephare-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.029474 lephare-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.029474 lephare-0.1.7/docs/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/doxygen/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/keywords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/legacy_install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.029474 lephare-0.1.7/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Building_list_of_onesources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Data_retrieval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Example_SED_manipulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Example_cosmo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Example_full_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Example_of_usage_of_magSvc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Minimal_photoz_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.033474 lephare-0.1.7/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/data/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/data/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks/data/output.para
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 03:33:50.000000 lephare-0.1.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.033474 lephare-0.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-15 03:33:50.000000 lephare-0.1.7/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-05-15 03:33:50.000000 lephare-0.1.7/examples/figuresLPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-05-15 03:33:50.000000 lephare-0.1.7/examples/figuresLPZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-15 03:33:50.000000 lephare-0.1.7/examples/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-15 03:33:50.000000 lephare-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:33:57.069474 lephare-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-15 03:33:50.000000 lephare-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.021474 lephare-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.033474 lephare-0.1.7/src/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/_flt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/filterSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/magSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/mag_gal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/sedtolib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lephare/zphota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.069474 lephare-0.1.7/src/lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-15 03:33:57.000000 lephare-0.1.7/src/lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 03:33:56.000000 lephare-0.1.7/src/lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.041474 lephare-0.1.7/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/PDF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/PDF.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72115 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/SED.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/SED.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/SEDLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/SEDLib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/_bindings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/cosmology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/cosmology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/ext_curv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/filter_extinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20186 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/flt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/flt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/globals.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/globals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/keyword.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/keyword.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/mag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/mag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/mag_gal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/oneElLambda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/oneElLambda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80072 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/onesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/onesource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/opa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/opa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61669 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/photoz_lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/photoz_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/sedtolib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-15 03:33:50.000000 lephare-0.1.7/src/lib/zphota.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.041474 lephare-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.045474 lephare-0.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/alloutputkeys.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/calzetti.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    84794 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/example.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.045474 lephare-0.1.7/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/examples/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)    66240 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/examples/COSMOS_first100specz.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/examples/output.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.045474 lephare-0.1.7/tests/data/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104052 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/ext/MW_seaton.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72411 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/ext/SB_calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.021474 lephare-0.1.7/tests/data/filt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.045474 lephare-0.1.7/tests/data/filt/subaru/
+-rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/filt/subaru/IB527.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.061474 lephare-0.1.7/tests/data/opa/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/OPACITY.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau00.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau01.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau02.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau03.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau04.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau05.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau06.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau07.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau08.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau09.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau10.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau11.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau12.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau13.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau14.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau15.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau16.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau17.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau18.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau19.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau20.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau21.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau22.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau23.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau24.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau25.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau26.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau27.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau28.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau29.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau30.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau31.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau32.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau33.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau34.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau35.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau36.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau37.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau38.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau39.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau40.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau41.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau42.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau43.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau44.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau45.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau46.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau47.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau48.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau49.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau50.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau51.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau52.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau53.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau54.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau55.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau56.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau57.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau58.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau59.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau60.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau61.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau62.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau63.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau64.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau65.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau66.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau67.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau68.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau69.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau70.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau71.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau72.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau73.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau74.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau75.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau76.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau77.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau78.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau79.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/opa/tau80.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.061474 lephare-0.1.7/tests/data/sed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.065474 lephare-0.1.7/tests/data/sed/GAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.065474 lephare-0.1.7/tests/data/sed/GAL/BETHERMIN12/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/GAL/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/GAL/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.065474 lephare-0.1.7/tests/data/sed/QSO/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/QSO/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/QSO/o5v.sed.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.065474 lephare-0.1.7/tests/data/sed/STAR/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/STAR/ONE_SED.list
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/STAR/o5v.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/WDgd71.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/sed/o5v.sed.ext
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/tau10.out
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/test_data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/test_file_names.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.065474 lephare-0.1.7/tests/data/vega/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1592 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/BD+17.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3957 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/BD+17o4708.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24434 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/SunLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24455 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/VegaLCB.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   100244 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/a0v.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93156 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/data/vega/a0v_n.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:33:57.069474 lephare-0.1.7/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_data_retrieval_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_magsvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_oneElLambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_onesource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_sed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-15 03:33:50.000000 lephare-0.1.7/tests/lephare/test_zphota.py
```

### Comparing `lephare-0.1.6/.copier-answers.yml` & `lephare-0.1.7/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.gitattributes` & `lephare-0.1.7/.gitattributes`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lephare-0.1.7/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lephare-0.1.7/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/pull_request_template.md` & `lephare-0.1.7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/build-documentation.yml` & `lephare-0.1.7/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/compile-cpp.yml` & `lephare-0.1.7/.github/workflows/compile-cpp.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/pre-commit-ci.yml` & `lephare-0.1.7/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/publish-to-pypi.yml` & `lephare-0.1.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/smoke-test.yml` & `lephare-0.1.7/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.github/workflows/testing-and-coverage.yml` & `lephare-0.1.7/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.gitignore` & `lephare-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.pre-commit-config.yaml` & `lephare-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.readthedocs.yml` & `lephare-0.1.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/.setup_dev.sh` & `lephare-0.1.7/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/CMakeLists.txt` & `lephare-0.1.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/LICENSE` & `lephare-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/PKG-INFO` & `lephare-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.6
+Version: 0.1.7
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -95,14 +95,15 @@
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
 >> git submodule update --init --recursive
+>> conda install -c conda-forge cxx-compiler
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
@@ -111,16 +112,12 @@
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
 
-## Citation
-
-If using this code in scientific research please cite the following papers:
-
 
 This project was automatically generated using the LINCC-Frameworks 
 [python-project-template](https://github.com/lincc-frameworks/python-project-template).
 For more information about the project template see the 
 [documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.6/README.md` & `lephare-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
 >> git submodule update --init --recursive
+>> conda install -c conda-forge cxx-compiler
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
@@ -56,16 +57,12 @@
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
 
-## Citation
-
-If using this code in scientific research please cite the following papers:
-
 
 This project was automatically generated using the LINCC-Frameworks 
 [python-project-template](https://github.com/lincc-frameworks/python-project-template).
 For more information about the project template see the 
 [documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.6/docs/Makefile` & `lephare-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/conf.py` & `lephare-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/doxygen/Doxyfile` & `lephare-0.1.7/docs/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/index.rst` & `lephare-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/keywords.rst` & `lephare-0.1.7/docs/keywords.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/legacy_install.rst` & `lephare-0.1.7/docs/legacy_install.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Building_list_of_onesources.ipynb` & `lephare-0.1.7/docs/notebooks/Building_list_of_onesources.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Data_retrieval.ipynb` & `lephare-0.1.7/docs/notebooks/Data_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Example_SED_manipulation.ipynb` & `lephare-0.1.7/docs/notebooks/Example_SED_manipulation.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Example_cosmo.ipynb` & `lephare-0.1.7/docs/notebooks/Example_cosmo.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Example_full_run.ipynb` & `lephare-0.1.7/docs/notebooks/Example_full_run.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Example_of_usage_of_magSvc.ipynb` & `lephare-0.1.7/docs/notebooks/Example_of_usage_of_magSvc.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Minimal_photoz_run.ipynb` & `lephare-0.1.7/docs/notebooks/Minimal_photoz_run.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/README.md` & `lephare-0.1.7/docs/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb` & `lephare-0.1.7/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/data/COSMOS.para` & `lephare-0.1.7/docs/notebooks/data/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/data/COSMOS_first100specz.fits` & `lephare-0.1.7/docs/notebooks/data/COSMOS_first100specz.fits`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks/data/output.para` & `lephare-0.1.7/docs/notebooks/data/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/docs/notebooks.rst` & `lephare-0.1.7/docs/notebooks.rst`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/examples/color.py` & `lephare-0.1.7/examples/color.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/examples/figuresLPP.py` & `lephare-0.1.7/examples/figuresLPP.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/examples/figuresLPZ.py` & `lephare-0.1.7/examples/figuresLPZ.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/examples/spec.py` & `lephare-0.1.7/examples/spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/pyproject.toml` & `lephare-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/setup.py` & `lephare-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/__init__.py` & `lephare-0.1.7/src/lephare/__init__.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/_flt.py` & `lephare-0.1.7/src/lephare/_flt.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/_pdf.py` & `lephare-0.1.7/src/lephare/_pdf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/_photoz.py` & `lephare-0.1.7/src/lephare/_photoz.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/_spec.py` & `lephare-0.1.7/src/lephare/_spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/_utils.py` & `lephare-0.1.7/src/lephare/_utils.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/data_manager.py` & `lephare-0.1.7/src/lephare/data_manager.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/data_retrieval.py` & `lephare-0.1.7/src/lephare/data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/filter.py` & `lephare-0.1.7/src/lephare/filter.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/filterSvc.py` & `lephare-0.1.7/src/lephare/filterSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/magSvc.py` & `lephare-0.1.7/src/lephare/magSvc.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,11 +40,14 @@
             instance = GalMag
         elif objtype[0].upper() == "Q":
             keywords += ["QSO_LIB_IN", "QSO_LIB_OUT"]
             instance = QSOMag
         elif objtype[0].upper() == "S":
             keywords += ["STAR_LIB_IN", "STAR_LIB_OUT"]
             instance = StarMag
+        else:
+            raise ValueError(f"Unknown objtype: {objtype}")
+
         keymap = read_config(config_file)
         keymap["t"] = keyword("t", objtype)
         keymap["c"] = keyword("c", config_file)
         return instance(keymap)
```

### Comparing `lephare-0.1.6/src/lephare/mag_gal.py` & `lephare-0.1.7/src/lephare/mag_gal.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/prepare.py` & `lephare-0.1.7/src/lephare/prepare.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import datetime
 import os
 
 import yaml
 
 import lephare as lp
 
-__all__ = ["prepare", "overwrite_config", "read_yaml_config", "write_yaml_config", "write_para_config"]
+__all__ = [
+    "prepare",
+    "overwrite_config",
+    "read_yaml_config",
+    "write_yaml_config",
+    "write_para_config",
+    "keymap_to_string_dict",
+    "string_dict_to_keymap",
+]
 
 
 def prepare(config, star_config=None, gal_config=None, qso_config=None):
     """Run the prepare stages of LePHARE
 
     In order to run "zphota" we must create the filter files, run sedtolib to
     create the SED libraries, and finally run mag_gal, to create the
@@ -25,14 +33,18 @@
     star_config : dict of lephare.keyword or None
         Config values to override for stars
     gal_config : dict of lephare.keyword or None
         Config values to override for galaxies
     qso_config : dict of lephare.keyword or None
         Config values to override for QSO.
     """
+    # check that the config is string to keyword map
+    for k in config:
+        assert isinstance(config[k], lp.keyword)
+
     object_types = {"STAR": star_config, "GAL": gal_config, "QSO": qso_config}
     # Run the filter command
     # load filters from config
     filter_lib = lp.FilterSvc.from_keymap(config)
     # Get location to store filter files
     filter_output = os.path.join(os.environ["LEPHAREWORK"], "filt", config["FILTER_FILE"].value)
     # Write filter files
@@ -119,7 +131,23 @@
     now = datetime.datetime.now().strftime("%Y%m%dT%H%M%S")
     para_contents = f"# File written automatically at {now}\n"
     for k in keymap:
         para_contents += f"{k} {keymap[k].value}\n"
     with open(para_file_path, "w") as file_handle:
         file_handle.write(para_contents)
         file_handle.close()
+
+
+def keymap_to_string_dict(keymap):
+    """Convert a dictionary of keywords to a dictionary of strings"""
+    config_dict = {}
+    for k in keymap:
+        config_dict[keymap[k].name] = keymap[k].value
+    return config_dict
+
+
+def string_dict_to_keymap(string_dict):
+    """Convert a dictionary of strings to a dictionary of keywords"""
+    keymap = {}
+    for k in string_dict:
+        keymap[k] = lp.keyword(k, str(string_dict[k]))
+    return keymap
```

### Comparing `lephare-0.1.6/src/lephare/process.py` & `lephare-0.1.7/src/lephare/process.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import os
+import shutil
+
 import numpy as np
 
 import lephare as lp
 
-__all__ = ["process", "table_to_data", "calculate_offsets"]
+__all__ = ["object_types", "process", "table_to_data", "calculate_offsets", "load_sed_list"]
+
+object_types = ["STAR", "GAL", "QSO"]
 
 
 def process(config, input, col_names=None, standard_names=False, filename=None, offsets=None):
     """Run all required steps to produce photometric redshift estimates
 
     Parameters
     ==========
@@ -215,7 +220,82 @@
     # Replace nans with -99
 
     mask = np.isnan(flux)
     mask |= np.isnan(flux_err)
     flux[mask] = -99.0
     flux_err[mask] = -99.0
     return id, flux, flux_err, context, zspec, string_data
+
+
+def load_sed_list(path_to_list, object_type, absolute_paths=False):
+    """Take a sed list and move it with the sed files to the work directory.
+
+    We want to be able to load SED lists from other sources. These may use
+    absolute paths or relative to the list file. They must adopt the lepahre
+    standard which is relative to the sed/$TYPE/ directory
+
+    Parameters
+    ==========
+    path_to_list : str
+        The path to the SED list file. This can be absolute or relative.
+    object_type : {'STAR', 'GAL', 'QSO'}
+        The type of object. Must be one of "STAR", "GAL", or "QSO".
+    absolute_paths : bool
+        Set to True if list of absolute paths and not relative to list file
+
+    Returns
+    =======
+        new_config_val : str
+            The location of the new list file with respect to current
+            LEPHAREWORK directory. This is the value to set in the config.
+    """
+    # The type must by one of the three lephare standards
+    assert object_type in object_types
+    # The original file must exist
+    assert os.path.isfile(path_to_list)
+
+    # Set folder and file names.
+    name = path_to_list.split("/")[-1].split(".")[0]
+    old_dir = os.path.dirname(path_to_list)
+    new_dir = f"{lp.dm.lephare_dir}/sed/{object_type}/{name}"
+    new_list_file = f"{new_dir}/{name}.list"
+    # Create the config value that needs to be passed to lephare.
+    new_config_val = f"sed/{object_type}/{name}"
+    if os.path.exists(new_list_file):
+        print(
+            f"List file already exists at {new_list_file}\n"
+            "The SEDs may already have been loaded to the work directory."
+        )
+        return new_config_val
+
+    # Get the list of sed files.
+    with open(path_to_list, "r") as f:
+        lines = f.readlines()
+    sed_files = []
+    for line in lines:
+        # Ignore commented files
+        if line.strip()[0] != "#":
+            sed_files.append(line.replace("\n", ""))
+
+    # Make the folder to hold the seds.
+    assert not os.path.isdir(new_dir)
+    print(
+        f"Creating new sed directory at {new_dir}.\n" "Attempting to copy sed files and list files in place."
+    )
+    os.makedirs(new_dir)
+
+    # Make the new list of files with paths from the type folder
+    new_list = ""
+    for sed_file in sed_files:
+        new_file = f"{sed_file.split('/')[-1]}"
+        new_list += f"{name}/{new_file}\n"
+        # Copy files
+        if absolute_paths:
+            shutil.copyfile(sed_file, f"{new_dir}/{new_file}")
+        else:
+            shutil.copyfile(f"{old_dir}/{sed_file.split('/')[-1]}", f"{new_dir}/{new_file}")
+
+    # Open the list file for writing and add all the seds
+    with open(new_list_file, "w") as file:
+        # Define the data to be written
+        file.write(new_list)
+    return new_config_val
```

### Comparing `lephare-0.1.6/src/lephare/runner.py` & `lephare-0.1.7/src/lephare/runner.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/sedtolib.py` & `lephare-0.1.7/src/lephare/sedtolib.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lephare/zphota.py` & `lephare-0.1.7/src/lephare/zphota.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,23 +91,14 @@
     def __init__(self, config_file=None):
         super().__init__(zphota_config_keys, config_file)
 
     def run(self, **kwargs):
         # update keymap and verbosity based on call arguments
         # this is only when the code is called from python session
         self.verbose = kwargs.pop("verbose", self.verbose)
-        for k, v in kwargs.items():
-            if k == "typ":
-                self.typ = v.upper()
-                continue
-            # if k == "config":
-            #     self.config = config_file
-            #     continue
-            if k.upper() in self.keymap:
-                self.keymap[k.upper()] = keyword(k.upper(), str(v))
         self.keymap["c"] = keyword("c", self.config)
 
         photoz = PhotoZ(self.keymap)
         autoadapt = (self.keymap["AUTO_ADAPT"]).split_bool("NO", 1)[0]
         if autoadapt:
             adapt_srcs = photoz.read_autoadapt_sources()
             a0, a1 = photoz.run_autoadapt(adapt_srcs)
```

### Comparing `lephare-0.1.6/src/lephare.egg-info/PKG-INFO` & `lephare-0.1.7/src/lephare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.6
+Version: 0.1.7
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Stéphane Arnouts <stephane.arnouts@lam.fr>, Olivier Ilbert <olivier.ilbert@lam.fr>, Johann Cohen-Tanugi <johann.cohen-tanugi@in2p3.fr>, Raphael Shirley <rshirley@mpe.mpg.de>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -95,14 +95,15 @@
 ```
 
 Once you have created a new environment, you can install this project for local
 development using the following commands:
 
 ```
 >> git submodule update --init --recursive
+>> conda install -c conda-forge cxx-compiler
 >> pip install -e .'[dev]'
 >> pre-commit install
 >> conda install pandoc
 ```
 
 Notes:
 1. The single quotes around `'[dev]'` may not be required for your operating system.
@@ -111,16 +112,12 @@
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
 
-## Citation
-
-If using this code in scientific research please cite the following papers:
-
 
 This project was automatically generated using the LINCC-Frameworks 
 [python-project-template](https://github.com/lincc-frameworks/python-project-template).
 For more information about the project template see the 
 [documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.6/src/lephare.egg-info/SOURCES.txt` & `lephare-0.1.7/src/lephare.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,17 @@
 tests/lephare/test_cosmology.py
 tests/lephare/test_data_manager.py
 tests/lephare/test_data_retrieval.py
 tests/lephare/test_data_retrieval_registry.py
 tests/lephare/test_filter.py
 tests/lephare/test_globals.py
 tests/lephare/test_keyword.py
+tests/lephare/test_magsvc.py
 tests/lephare/test_oneElLambda.py
 tests/lephare/test_onesource.py
+tests/lephare/test_pdf.py
 tests/lephare/test_prepare.py
 tests/lephare/test_process.py
 tests/lephare/test_runner.py
 tests/lephare/test_sed.py
-tests/lephare/test_spec.py
+tests/lephare/test_spec.py
+tests/lephare/test_zphota.py
```

### Comparing `lephare-0.1.6/src/lib/Makefile` & `lephare-0.1.7/src/lib/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/PDF.cpp` & `lephare-0.1.7/src/lib/PDF.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/PDF.h` & `lephare-0.1.7/src/lib/PDF.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/SED.cpp` & `lephare-0.1.7/src/lib/SED.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/SED.h` & `lephare-0.1.7/src/lib/SED.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/SEDLib.cpp` & `lephare-0.1.7/src/lib/SEDLib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/SEDLib.h` & `lephare-0.1.7/src/lib/SEDLib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/_bindings.cc` & `lephare-0.1.7/src/lib/_bindings.cc`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/cosmology.cpp` & `lephare-0.1.7/src/lib/cosmology.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/cosmology.h` & `lephare-0.1.7/src/lib/cosmology.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/ext.cpp` & `lephare-0.1.7/src/lib/ext.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/ext.h` & `lephare-0.1.7/src/lib/ext.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/ext_curv.cpp` & `lephare-0.1.7/src/lib/ext_curv.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/filter.cpp` & `lephare-0.1.7/src/lib/filter.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/filter_extinc.cpp` & `lephare-0.1.7/src/lib/filter_extinc.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/flt.cpp` & `lephare-0.1.7/src/lib/flt.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/flt.h` & `lephare-0.1.7/src/lib/flt.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/globals.cpp` & `lephare-0.1.7/src/lib/globals.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/globals.h` & `lephare-0.1.7/src/lib/globals.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/keyword.cpp` & `lephare-0.1.7/src/lib/keyword.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/keyword.h` & `lephare-0.1.7/src/lib/keyword.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/mag.cpp` & `lephare-0.1.7/src/lib/mag.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/mag.h` & `lephare-0.1.7/src/lib/mag.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/mag_gal.cpp` & `lephare-0.1.7/src/lib/mag_gal.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/oneElLambda.cpp` & `lephare-0.1.7/src/lib/oneElLambda.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/oneElLambda.h` & `lephare-0.1.7/src/lib/oneElLambda.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/onesource.cpp` & `lephare-0.1.7/src/lib/onesource.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/onesource.h` & `lephare-0.1.7/src/lib/onesource.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/opa.cpp` & `lephare-0.1.7/src/lib/opa.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/opa.h` & `lephare-0.1.7/src/lib/opa.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/photoz_lib.cpp` & `lephare-0.1.7/src/lib/photoz_lib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/photoz_lib.h` & `lephare-0.1.7/src/lib/photoz_lib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/sedtolib.cpp` & `lephare-0.1.7/src/lib/sedtolib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/src/lib/zphota.cpp` & `lephare-0.1.7/src/lib/zphota.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/conftest.py` & `lephare-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/alloutputkeys.txt` & `lephare-0.1.7/tests/data/alloutputkeys.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/calzetti.dat` & `lephare-0.1.7/tests/data/calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/example.spec` & `lephare-0.1.7/tests/data/example.spec`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/examples/COSMOS.para` & `lephare-0.1.7/tests/data/examples/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/examples/COSMOS_first100specz.fits` & `lephare-0.1.7/tests/data/examples/COSMOS_first100specz.fits`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/examples/output.para` & `lephare-0.1.7/tests/data/examples/output.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/ext/MW_seaton.dat` & `lephare-0.1.7/tests/data/ext/MW_seaton.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/ext/SB_calzetti.dat` & `lephare-0.1.7/tests/data/ext/SB_calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/filt/subaru/IB527.pb` & `lephare-0.1.7/tests/data/filt/subaru/IB527.pb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/OPACITY.dat` & `lephare-0.1.7/tests/data/opa/OPACITY.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau00.out` & `lephare-0.1.7/tests/data/opa/tau00.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau01.out` & `lephare-0.1.7/tests/data/opa/tau01.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau02.out` & `lephare-0.1.7/tests/data/opa/tau02.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau03.out` & `lephare-0.1.7/tests/data/opa/tau03.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau04.out` & `lephare-0.1.7/tests/data/opa/tau04.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau05.out` & `lephare-0.1.7/tests/data/opa/tau05.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau06.out` & `lephare-0.1.7/tests/data/opa/tau06.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau07.out` & `lephare-0.1.7/tests/data/opa/tau07.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau08.out` & `lephare-0.1.7/tests/data/opa/tau08.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau09.out` & `lephare-0.1.7/tests/data/opa/tau09.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau10.out` & `lephare-0.1.7/tests/data/opa/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau11.out` & `lephare-0.1.7/tests/data/opa/tau11.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau12.out` & `lephare-0.1.7/tests/data/opa/tau12.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau13.out` & `lephare-0.1.7/tests/data/opa/tau13.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau14.out` & `lephare-0.1.7/tests/data/opa/tau14.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau15.out` & `lephare-0.1.7/tests/data/opa/tau15.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau16.out` & `lephare-0.1.7/tests/data/opa/tau16.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau17.out` & `lephare-0.1.7/tests/data/opa/tau17.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau18.out` & `lephare-0.1.7/tests/data/opa/tau18.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau19.out` & `lephare-0.1.7/tests/data/opa/tau19.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau20.out` & `lephare-0.1.7/tests/data/opa/tau20.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau21.out` & `lephare-0.1.7/tests/data/opa/tau21.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau22.out` & `lephare-0.1.7/tests/data/opa/tau22.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau23.out` & `lephare-0.1.7/tests/data/opa/tau23.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau24.out` & `lephare-0.1.7/tests/data/opa/tau24.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau25.out` & `lephare-0.1.7/tests/data/opa/tau25.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau26.out` & `lephare-0.1.7/tests/data/opa/tau26.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau27.out` & `lephare-0.1.7/tests/data/opa/tau27.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau28.out` & `lephare-0.1.7/tests/data/opa/tau28.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau29.out` & `lephare-0.1.7/tests/data/opa/tau29.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau30.out` & `lephare-0.1.7/tests/data/opa/tau30.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau31.out` & `lephare-0.1.7/tests/data/opa/tau31.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau32.out` & `lephare-0.1.7/tests/data/opa/tau32.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau33.out` & `lephare-0.1.7/tests/data/opa/tau33.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau34.out` & `lephare-0.1.7/tests/data/opa/tau34.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau35.out` & `lephare-0.1.7/tests/data/opa/tau35.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau36.out` & `lephare-0.1.7/tests/data/opa/tau36.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau37.out` & `lephare-0.1.7/tests/data/opa/tau37.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau38.out` & `lephare-0.1.7/tests/data/opa/tau38.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau39.out` & `lephare-0.1.7/tests/data/opa/tau39.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau40.out` & `lephare-0.1.7/tests/data/opa/tau40.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau41.out` & `lephare-0.1.7/tests/data/opa/tau41.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau42.out` & `lephare-0.1.7/tests/data/opa/tau42.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau43.out` & `lephare-0.1.7/tests/data/opa/tau43.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau44.out` & `lephare-0.1.7/tests/data/opa/tau44.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau45.out` & `lephare-0.1.7/tests/data/opa/tau45.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau46.out` & `lephare-0.1.7/tests/data/opa/tau46.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau47.out` & `lephare-0.1.7/tests/data/opa/tau47.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau48.out` & `lephare-0.1.7/tests/data/opa/tau48.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau49.out` & `lephare-0.1.7/tests/data/opa/tau49.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau50.out` & `lephare-0.1.7/tests/data/opa/tau50.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau51.out` & `lephare-0.1.7/tests/data/opa/tau51.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau52.out` & `lephare-0.1.7/tests/data/opa/tau52.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau53.out` & `lephare-0.1.7/tests/data/opa/tau53.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau54.out` & `lephare-0.1.7/tests/data/opa/tau54.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau55.out` & `lephare-0.1.7/tests/data/opa/tau55.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau56.out` & `lephare-0.1.7/tests/data/opa/tau56.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau57.out` & `lephare-0.1.7/tests/data/opa/tau57.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau58.out` & `lephare-0.1.7/tests/data/opa/tau58.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau59.out` & `lephare-0.1.7/tests/data/opa/tau59.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau60.out` & `lephare-0.1.7/tests/data/opa/tau60.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau61.out` & `lephare-0.1.7/tests/data/opa/tau61.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau62.out` & `lephare-0.1.7/tests/data/opa/tau62.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau63.out` & `lephare-0.1.7/tests/data/opa/tau63.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau64.out` & `lephare-0.1.7/tests/data/opa/tau64.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau65.out` & `lephare-0.1.7/tests/data/opa/tau65.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau66.out` & `lephare-0.1.7/tests/data/opa/tau66.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau67.out` & `lephare-0.1.7/tests/data/opa/tau67.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau68.out` & `lephare-0.1.7/tests/data/opa/tau68.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau69.out` & `lephare-0.1.7/tests/data/opa/tau69.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau70.out` & `lephare-0.1.7/tests/data/opa/tau70.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau71.out` & `lephare-0.1.7/tests/data/opa/tau71.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau72.out` & `lephare-0.1.7/tests/data/opa/tau72.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau73.out` & `lephare-0.1.7/tests/data/opa/tau73.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau74.out` & `lephare-0.1.7/tests/data/opa/tau74.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau75.out` & `lephare-0.1.7/tests/data/opa/tau75.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau76.out` & `lephare-0.1.7/tests/data/opa/tau76.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau77.out` & `lephare-0.1.7/tests/data/opa/tau77.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau78.out` & `lephare-0.1.7/tests/data/opa/tau78.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau79.out` & `lephare-0.1.7/tests/data/opa/tau79.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/opa/tau80.out` & `lephare-0.1.7/tests/data/opa/tau80.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat` & `lephare-0.1.7/tests/data/sed/GAL/BETHERMIN12/sed_z1_MS.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/GAL/o5v.sed.ext` & `lephare-0.1.7/tests/data/sed/GAL/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/QSO/o5v.sed.ext` & `lephare-0.1.7/tests/data/sed/QSO/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/STAR/o5v.sed.ext` & `lephare-0.1.7/tests/data/sed/STAR/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/WDgd71.sed.ext` & `lephare-0.1.7/tests/data/sed/WDgd71.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/sed/o5v.sed.ext` & `lephare-0.1.7/tests/data/sed/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/tau10.out` & `lephare-0.1.7/tests/data/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/BD+17.sed` & `lephare-0.1.7/tests/data/vega/BD+17.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/BD+17o4708.sed` & `lephare-0.1.7/tests/data/vega/BD+17o4708.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/SunLCB.sed` & `lephare-0.1.7/tests/data/vega/SunLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/VegaLCB.sed` & `lephare-0.1.7/tests/data/vega/VegaLCB.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/a0v.sed` & `lephare-0.1.7/tests/data/vega/a0v.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/data/vega/a0v_n.sed` & `lephare-0.1.7/tests/data/vega/a0v_n.sed`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_cosmology.py` & `lephare-0.1.7/tests/lephare/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_data_manager.py` & `lephare-0.1.7/tests/lephare/test_data_manager.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_data_retrieval.py` & `lephare-0.1.7/tests/lephare/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_data_retrieval_registry.py` & `lephare-0.1.7/tests/lephare/test_data_retrieval_registry.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_filter.py` & `lephare-0.1.7/tests/lephare/test_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 
+import matplotlib
 import numpy as np
 import pytest
 from lephare import (
     Filter,
     flt,  # noqa: E402
 )
 from lephare.filterSvc import FilterSvc  # noqa: E402
 
+matplotlib.use("Agg")
+
 
 @pytest.fixture
 def filter_file(test_data_dir):
     return os.path.join(test_data_dir, "filt/subaru/IB527.pb")
 
 
 def test_flt_class(filter_file):
@@ -54,7 +57,17 @@
     config_file_path = os.path.join(test_data_dir, "examples/COSMOS.para")
     input_args = {"verbose": True, "TRANS_TYPE": 42}
     filter = Filter(config_file=config_file_path)
     filter.run(**input_args)
     assert len(filter.keymap)
     assert filter.verbose
     assert filter.keymap["TRANS_TYPE"].value == "42"
+
+
+def test_flt_plot_filter_curve():
+    """Simple test that exercises the plot_filter_curve method."""
+    tophat = flt(100.0, 200.0, 50)
+    tophat.plot_filter_curve()
+    tophat.plot_filter_curve(normed=True)
+
+    # this is assertion doesn't mean anything, just here to assert _something_.
+    assert tophat.name == ""
```

### Comparing `lephare-0.1.6/tests/lephare/test_keyword.py` & `lephare-0.1.7/tests/lephare/test_keyword.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_oneElLambda.py` & `lephare-0.1.7/tests/lephare/test_oneElLambda.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_onesource.py` & `lephare-0.1.7/tests/lephare/test_onesource.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_process.py` & `lephare-0.1.7/tests/lephare/test_process.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_runner.py` & `lephare-0.1.7/tests/lephare/test_runner.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.6/tests/lephare/test_sed.py` & `lephare-0.1.7/tests/lephare/test_sed.py`

 * *Files identical despite different names*

