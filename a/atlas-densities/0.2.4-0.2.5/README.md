# Comparing `tmp/atlas-densities-0.2.4.tar.gz` & `tmp/atlas-densities-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-densities-0.2.4.tar", last modified: Thu Apr 18 12:15:18 2024, max compression
+gzip compressed data, was "atlas-densities-0.2.5.tar", last modified: Wed May 15 14:27:56 2024, max compression
```

## Comparing `atlas-densities-0.2.4.tar` & `atlas-densities-0.2.5.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.437560 atlas-densities-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22025 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities/app/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43635 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.445560 atlas-densities-0.2.4/atlas_densities/app/data/
--rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.445560 atlas-densities-0.2.4/atlas_densities/app/data/markers/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_bbp.json
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/measurements/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/gaba_papers.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/homogenous_regions.csv
--rw-r--r--   0 runner    (1001) docker     (127)   839727 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/measurements.csv
--rw-r--r--   0 runner    (1001) docker     (127)   347207 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)   291827 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc3.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/non_density_measurements.csv
--rw-r--r--   0 runner    (1001) docker     (127)   199258 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/std_cells.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/ca1_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/group_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/isocortex_23_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/isocortex_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/thalamus_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/composition.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.453560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.457560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)   930916 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.457560 atlas-densities-0.2.4/atlas_densities/combination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/atlas_densities/densities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/cell_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    26599 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_composition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)   230179 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/bbpp82_628_linear_program.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/cell_densities.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/combination.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/mtype_densities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (127)    55115 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/static/atlas-densities.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_refined_inhibitory_neuron_densities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/combination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/test_annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/test_markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.437560 atlas-densities-0.2.4/tests/densities/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/data/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/mapping.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/mapping_exc_only.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/data/mtypes/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/BP.dat
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/mtype-taxonomy.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25290 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_optimization_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_refined_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/markers_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/mocking_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.700736 atlas-densities-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.664736 atlas-densities-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.668736 atlas-densities-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-05-15 14:27:56.700736 atlas-densities-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22025 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.668736 atlas-densities-0.2.5/atlas_densities/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.672736 atlas-densities-0.2.5/atlas_densities/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43635 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.672736 atlas-densities-0.2.5/atlas_densities/app/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.672736 atlas-densities-0.2.5/atlas_densities/app/data/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/markers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/markers/realigned_slices_bbp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.676736 atlas-densities-0.2.5/atlas_densities/app/data/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/gaba_papers.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/homogenous_regions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   839727 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   347207 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/mmc1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   291827 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/mmc3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/non_density_measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   199258 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/measurements/std_cells.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.676736 atlas-densities-0.2.5/atlas_densities/app/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/ca1_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/group_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/isocortex_23_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/isocortex_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/metadata/thalamus_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.676736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.680736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/composition.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.680736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.680736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.684736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.684736 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/probability_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/probability_map/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   930916 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.684736 atlas-densities-0.2.5/atlas_densities/combination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/combination/annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/combination/markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.688736 atlas-densities-0.2.5/atlas_densities/densities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26599 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_composition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.688736 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/refined_inhibitory_neuron_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/atlas_densities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.668736 atlas-densities-0.2.5/atlas_densities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 14:27:56.000000 atlas-densities-0.2.5/atlas_densities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.688736 atlas-densities-0.2.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.692736 atlas-densities-0.2.5/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)   230179 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/bbpp82_628_linear_program.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/cell_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/combination.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/mtype_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.692736 atlas-densities-0.2.5/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    55115 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/doc/source/static/atlas-densities.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:27:56.700736 atlas-densities-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.692736 atlas-densities-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.692736 atlas-densities-0.2.5/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/app/test_cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/app/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/app/test_mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/app/test_refined_inhibitory_neuron_densities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.696736 atlas-densities-0.2.5/tests/combination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/combination/test_annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/combination/test_markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.696736 atlas-densities-0.2.5/tests/densities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.664736 atlas-densities-0.2.5/tests/densities/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.696736 atlas-densities-0.2.5/tests/densities/data/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/meta/mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/meta/mapping_exc_only.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:27:56.700736 atlas-densities-0.2.5/tests/densities/data/mtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/data/mtypes/mtype-taxonomy.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_density_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25290 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_optimization_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_refined_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/densities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/markers_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/mocking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 14:27:53.000000 atlas-densities-0.2.5/tox.ini
```

### Comparing `atlas-densities-0.2.4/.github/workflows/publish-sdist.yml` & `atlas-densities-0.2.5/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/.github/workflows/run-tox.yml` & `atlas-densities-0.2.5/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/.pylintrc` & `atlas-densities-0.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/CHANGELOG.rst` & `atlas-densities-0.2.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/CONTRIBUTING.rst` & `atlas-densities-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/LICENSE.txt` & `atlas-densities-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/PKG-INFO` & `atlas-densities-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: |banner|
```

### Comparing `atlas-densities-0.2.4/README.rst` & `atlas-densities-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/cell_densities.py` & `atlas-densities-0.2.5/atlas_densities/app/cell_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/cli.py` & `atlas-densities-0.2.5/atlas_densities/app/cli.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/combination.py` & `atlas-densities-0.2.5/atlas_densities/app/combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/1.json` & `atlas-densities-0.2.5/atlas_densities/app/data/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/markers/README.rst` & `atlas-densities-0.2.5/atlas_densities/app/data/markers/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml` & `atlas-densities-0.2.5/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_bbp.json` & `atlas-densities-0.2.5/atlas_densities/app/data/markers/realigned_slices_bbp.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json` & `atlas-densities-0.2.5/atlas_densities/app/data/markers/realigned_slices_ccfv2.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/README.rst` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/gaba_papers.xlsx` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/gaba_papers.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/homogenous_regions.csv` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/homogenous_regions.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/measurements.csv` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc1.xlsx` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/mmc1.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc3.xlsx` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/mmc3.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/non_density_measurements.csv` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/non_density_measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/measurements/std_cells.json` & `atlas-densities-0.2.5/atlas_densities/app/data/measurements/std_cells.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/metadata/README.txt` & `atlas-densities-0.2.5/atlas_densities/app/data/metadata/README.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/metadata/group_ids.json` & `atlas-densities-0.2.5/atlas_densities/app/data/metadata/group_ids.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/metadata/thalamus_metadata.json` & `atlas-densities-0.2.5/atlas_densities/app/data/metadata/thalamus_metadata.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/README.rst` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/composition.yaml` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/composition.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/README.rst` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/README.rst` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/probability_map/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv` & `atlas-densities-0.2.5/atlas_densities/app/data/mtypes/probability_map/probability_map.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/app/mtype_densities.py` & `atlas-densities-0.2.5/atlas_densities/app/mtype_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/combination/annotations_combinator.py` & `atlas-densities-0.2.5/atlas_densities/combination/annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/combination/markers_combinator.py` & `atlas-densities-0.2.5/atlas_densities/combination/markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/cell_counts.py` & `atlas-densities-0.2.5/atlas_densities/densities/cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/cell_density.py` & `atlas-densities-0.2.5/atlas_densities/densities/cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/excel_reader.py` & `atlas-densities-0.2.5/atlas_densities/densities/excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/excitatory_inhibitory_splitting.py` & `atlas-densities-0.2.5/atlas_densities/densities/excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/fitting.py` & `atlas-densities-0.2.5/atlas_densities/densities/fitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/glia_densities.py` & `atlas-densities-0.2.5/atlas_densities/densities/glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py` & `atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py` & `atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_densities_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_density.py` & `atlas-densities-0.2.5/atlas_densities/densities/inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/measurement_to_density.py` & `atlas-densities-0.2.5/atlas_densities/densities/measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_composition.py` & `atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/create.py` & `atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/create.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/utils.py` & `atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_map/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_profiles.py` & `atlas-densities-0.2.5/atlas_densities/densities/mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py` & `atlas-densities-0.2.5/atlas_densities/densities/refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities/densities/utils.py` & `atlas-densities-0.2.5/atlas_densities/densities/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
             "brain_region": hierarchy_info["brain_region"],
             "id_volume": 0.0,
         },
         index=hierarchy_info.index,
     )
 
     ids, counts = np.unique(annotation, return_counts=True)
-    result["id_volume"] = pd.Series(counts * voxel_volume, index=ids)
+    result["id_volume"].update(pd.Series(counts * voxel_volume, index=ids))
 
     volumes = []
     for id_ in hierarchy_info.index:
         id_set = hierarchy_info.loc[id_, "descendant_ids"]
         volume = result.loc[list(id_set), "id_volume"].sum()
         volumes.append(volume)
     result["volume"] = volumes
```

### Comparing `atlas-densities-0.2.4/atlas_densities/utils.py` & `atlas-densities-0.2.5/atlas_densities/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/atlas_densities.egg-info/PKG-INFO` & `atlas-densities-0.2.5/atlas_densities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: |banner|
```

### Comparing `atlas-densities-0.2.4/atlas_densities.egg-info/SOURCES.txt` & `atlas-densities-0.2.5/atlas_densities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/doc/Makefile` & `atlas-densities-0.2.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/doc/source/bbpp82_628_linear_program.pdf` & `atlas-densities-0.2.5/doc/source/bbpp82_628_linear_program.pdf`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/doc/source/conf.py` & `atlas-densities-0.2.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/doc/source/index.rst` & `atlas-densities-0.2.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/doc/source/static/atlas-densities.jpg` & `atlas-densities-0.2.5/doc/source/static/atlas-densities.jpg`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/setup.py` & `atlas-densities-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/1.json` & `atlas-densities-0.2.5/tests/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/app/test_cell_densities.py` & `atlas-densities-0.2.5/tests/app/test_cell_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/app/test_combination.py` & `atlas-densities-0.2.5/tests/app/test_combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/app/test_mtype_densities.py` & `atlas-densities-0.2.5/tests/app/test_mtype_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/app/test_refined_inhibitory_neuron_densities.py` & `atlas-densities-0.2.5/tests/app/test_refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/combination/test_annotations_combinator.py` & `atlas-densities-0.2.5/tests/combination/test_annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/combination/test_markers_combinator.py` & `atlas-densities-0.2.5/tests/combination/test_markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/data/mtypes/mtype-taxonomy.tsv` & `atlas-densities-0.2.5/tests/densities/data/mtypes/mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_cell_counts.py` & `atlas-densities-0.2.5/tests/densities/test_cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_cell_density.py` & `atlas-densities-0.2.5/tests/densities/test_cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_excel_reader.py` & `atlas-densities-0.2.5/tests/densities/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_excitatory_inhibitory_splitting.py` & `atlas-densities-0.2.5/tests/densities/test_excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_fitting.py` & `atlas-densities-0.2.5/tests/densities/test_fitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_glia_densities.py` & `atlas-densities-0.2.5/tests/densities/test_glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_densities_helper.py` & `atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density.py` & `atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density_optimization.py` & `atlas-densities-0.2.5/tests/densities/test_inhibitory_neuron_density_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_measurement_to_density.py` & `atlas-densities-0.2.5/tests/densities/test_measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_composition.py` & `atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_map.py` & `atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_map.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_profiles.py` & `atlas-densities-0.2.5/tests/densities/test_mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_optimization_initialization.py` & `atlas-densities-0.2.5/tests/densities/test_optimization_initialization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_refined_inhibitory_neuron_density.py` & `atlas-densities-0.2.5/tests/densities/test_refined_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/densities/test_utils.py` & `atlas-densities-0.2.5/tests/densities/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -368,32 +368,24 @@
 def test_get_hierarchy(region_map):
     pdt.assert_frame_equal(
         pd.DataFrame(tested.get_hierarchy_info(region_map, root="Central lobule")),
         get_hierarchy_info(),
     )
 
 
-@pytest.fixture
-def annotation():
-    return np.array([[[920, 10710, 10710], [10709, 10708, 976], [10708, 10710, 10709]]])
-
-
-@pytest.fixture
-def volumes(voxel_volume=2):
+def test_compute_region_volumes():
+    voxel_volume = 2.0
+    annotation = np.array([[[920, 10710, 10710], [10709, 10708, 976], [10708, 10710, 10709]]])
     hierarchy_info = get_hierarchy_info()
-    return pd.DataFrame(
+    hierarchy_info.loc[42] = ("VolumeLess", set())
+    expected = pd.DataFrame(
         {
             "brain_region": hierarchy_info["brain_region"],
-            "id_volume": voxel_volume * np.array([1.0, 1.0, 2.0, 2.0, 3.0], dtype=float),
-            "volume": voxel_volume * np.array([9.0, 8.0, 2.0, 2.0, 3.0], dtype=float),
+            "id_volume": voxel_volume * np.array([1.0, 1.0, 2.0, 2.0, 3.0, 0.0], dtype=float),
+            "volume": voxel_volume * np.array([9.0, 8.0, 2.0, 2.0, 3.0, 0.0], dtype=float),
         },
         index=hierarchy_info.index,
     )
-
-
-def test_compute_region_volumes(volumes, annotation):
-    pdt.assert_frame_equal(
-        volumes,  # expected
-        tested.compute_region_volumes(
-            annotation, voxel_volume=2.0, hierarchy_info=get_hierarchy_info()
-        ),
+    res = tested.compute_region_volumes(
+        annotation, voxel_volume=voxel_volume, hierarchy_info=hierarchy_info
     )
+    pdt.assert_frame_equal(expected, res)
```

### Comparing `atlas-densities-0.2.4/tests/markers_config.yaml` & `atlas-densities-0.2.5/tests/markers_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/mocking_tools.py` & `atlas-densities-0.2.5/tests/mocking_tools.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tests/test_utils.py` & `atlas-densities-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.4/tox.ini` & `atlas-densities-0.2.5/tox.ini`

 * *Files identical despite different names*

