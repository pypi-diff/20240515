# Comparing `tmp/diameter-synthesis-0.5.4.tar.gz` & `tmp/diameter_synthesis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diameter-synthesis-0.5.4.tar", last modified: Thu May  4 10:07:33 2023, max compression
+gzip compressed data, was "diameter_synthesis-0.6.0.tar", last modified: Wed May 15 13:58:33 2024, max compression
```

## Comparing `diameter-synthesis-0.5.4.tar` & `diameter_synthesis-0.6.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.801376 diameter-synthesis-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/how_to_use.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.805376 diameter-synthesis-0.5.4/diameter_synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/build_diameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/build_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/distribution_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/morph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23272 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/diameter_synthesis/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/schemas/model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/simpler_diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/diameter_synthesis/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 10:07:33.000000 diameter-synthesis-0.5.4/diameter_synthesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/docs/source/params_and_distrs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.809376 diameter-synthesis-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/diametrizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/get_morphologies.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/rediametrize_single_neuron.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:07:33.821376 diameter-synthesis-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.813376 diameter-synthesis-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3.h5
--rw-r--r--   0 runner    (1001) docker     (123)    90432 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_diametrized.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_1_sample.h5
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/astro_model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/astro_model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/neurondb.dat
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_model_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_model_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/simpler_morph_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_apical_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_diametrized.asc
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/data/small_morph_several_apical_diametrized.asc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.797376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    16095 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:07:33.817376 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_cumulative_distribution.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_div.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_mult.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_plot_distribution_fit.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    34588 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/expected_images/test_violin_analysis.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_build_diameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_build_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_distribution_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_morph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_simpler_diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tests/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-04 10:07:20.000000 diameter-synthesis-0.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.112666 diameter_synthesis-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.096666 diameter_synthesis-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.096666 diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/how_to_use.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.096666 diameter_synthesis-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    28019 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-15 13:58:33.112666 diameter_synthesis-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.096666 diameter_synthesis-0.6.0/diameter_synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19156 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/build_diameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/build_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/distribution_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/morph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.100667 diameter_synthesis-0.6.0/diameter_synthesis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/schemas/model_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/simpler_diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/diameter_synthesis/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 13:58:33.000000 diameter_synthesis-0.6.0/diameter_synthesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.100667 diameter_synthesis-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.100667 diameter_synthesis-0.6.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/docs/source/params_and_distrs.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.100667 diameter_synthesis-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/examples/diametrizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/examples/get_morphologies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/examples/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/examples/rediametrize_single_neuron.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:58:33.112666 diameter_synthesis-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.104667 diameter_synthesis-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.104667 diameter_synthesis-0.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    90432 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    90432 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3_diametrized.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    21120 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized_1_sample.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/astro_model_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/astro_model_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/model_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/model_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/neurondb.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/simpler_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/simpler_model_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/simpler_model_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/simpler_morph_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/small_morph_apical_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/small_morph_diametrized.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/data/small_morph_several_apical_diametrized.asc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.088667 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/
+-rw-r--r--   0 runner    (1001) docker     (127)    15483 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:58:33.108667 diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_plot_cumulative_distribution.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    56388 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_plot_diameter_diff_div.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    56388 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_plot_diameter_diff_mult.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_plot_distribution_fit.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    34449 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/expected_images/test_violin_analysis.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_build_diameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_build_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_distribution_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_morph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_simpler_diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tests/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-15 13:58:27.000000 diameter_synthesis-0.6.0/tox.ini
```

### Comparing `diameter-synthesis-0.5.4/.auto-changelog` & `diameter_synthesis-0.6.0/.auto-changelog`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'ignoreCommitPattern'": "'^Release:? [0-9]+\\\\.[0-9]+\\\\.[0-9]+( ?\\\\(#[0-9]+\\\\))?$|^Update "*

 * *                          'CHANGELOG.*|.*\\\\[skip-changelog\\\\].*|^\\\\[pre-commit.ci\\\\]|^\\\\(dependabot\\\\) '*

 * *                          ".*'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "backfillLimit": false,
     "commitLimit": false,
     "commitUrl": "https://github.com/BlueBrain/diameter-synthesis/commit/{id}",
     "compareUrl": "https://github.com/BlueBrain/diameter-synthesis/compare/{from}..{to}",
-    "ignoreCommitPattern": "Release:? [0-9]+\\.[0-9]+\\.[0-9]+|Update CHANGELOG.*|.*\\[skip-changelog\\].*|\\[pre-commit.ci\\]",
+    "ignoreCommitPattern": "^Release:? [0-9]+\\.[0-9]+\\.[0-9]+( ?\\(#[0-9]+\\))?$|^Update CHANGELOG.*|.*\\[skip-changelog\\].*|^\\[pre-commit.ci\\]|^\\(dependabot\\) .*",
     "issueUrl": "https://github.com/BlueBrain/diameter-synthesis/issues/{id}",
     "mergeUrl": "https://github.com/BlueBrain/diameter-synthesis/pull/{id}",
     "output": "CHANGELOG.md",
     "startingVersion": "0.4.2",
     "template": ".auto-changelog-template.hbs"
 }
```

### Comparing `diameter-synthesis-0.5.4/.auto-changelog-template.hbs` & `diameter_synthesis-0.6.0/.auto-changelog-template.hbs`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list merges heading='### CI Improvements' message='^[cC][iI]:|^[cC][iI]\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
-      {{#commit-list merges heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild\(|^[dD]eprecate:|^[dD]eprecate\(|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
+      {{#commit-list merges heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild ?\(|^[dD]eprecate:|^[dD]eprecate ?\(|^[fF]eat:|^[fF]eat ?\(|^[fF]ix:|^[fF]ix ?\(|^[cC]hore:|^[cC]hore ?\(|^[cC][iI]:|^[cC][iI] ?\(|^[dD]ocs:|^[dD]ocs ?\(|^[rR]efactor:|^[rR]efactor ?\(|^[tT]est:|^[tT]est ?\(|^[sS]tyle:|^[sS]tyle ?\(|^[pP]erf:|^[pP]erf ?\(|\[skip-changelog\]'}}
         - {{message}} ({{author}}{{#if href}} - [#{{id}}]({{href}}){{/if}})
       {{/commit-list}}
 
   {{! List commits with 'breaking:' or 'Breaking change:' anywhere in the message under a heading}}
   {{#commit-list commits heading='### Breaking Changes :warning:' message='[bB]reaking [cC]hange:|[bB]reaking:' exclude='\[skip-changelog\]'}}
     - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
   {{/commit-list}}
@@ -186,12 +186,12 @@
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
       {{#commit-list commits heading='### CI Improvements' message='^[cC][iI]:|^[cC][iI]\(' exclude='[bB]reaking [cC]hange:|[bB]reaking:|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
-      {{#commit-list commits heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild\(|^[dD]eprecate:|^[dD]eprecate\(|^[fF]eat:|^[fF]eat\(|^[fF]ix:|^[fF]ix\(|^[cC]hore:|^[cC]hore\(|^[cC][iI]:|^[cC][iI]\(|^[dD]ocs:|^[dD]ocs\(|^[rR]efactor:|^[rR]efactor\(|^[tT]est:|^[tT]est\(|^[sS]tyle:|^[sS]tyle\(|^[pP]erf:|^[pP]erf\(|\[skip-changelog\]'}}
+      {{#commit-list commits heading='### General Changes' exclude='[bB]reaking [cC]hange:|[bB]reaking:|^[bB]uild:|^[bB]uild ?\(|^[dD]eprecate:|^[dD]eprecate ?\(|^[fF]eat:|^[fF]eat ?\(|^[fF]ix:|^[fF]ix ?\(|^[cC]hore:|^[cC]hore ?\(|^[cC][iI]:|^[cC][iI] ?\(|^[dD]ocs:|^[dD]ocs ?\(|^[rR]efactor:|^[rR]efactor ?\(|^[tT]est:|^[tT]est ?\(|^[sS]tyle:|^[sS]tyle ?\(|^[pP]erf:|^[pP]erf ?\(|\[skip-changelog\]'}}
         - {{subject}} ({{author}}{{#if href}} - [{{shorthash}}]({{href}}){{/if}})
       {{/commit-list}}
 
 {{/each}}
```

### Comparing `diameter-synthesis-0.5.4/.copier-answers.yml` & `diameter_synthesis-0.6.0/.copier-answers.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.43
+_commit: 0.1.57
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
-copyright_license: GNU General Public License v3.0
+copyright_license: Apache License 2.0
 copyright_year: '2022'
 distribution_name: diameter-synthesis
-download_url: git@github.com:BlueBrain/diameter-synthesis.git
+download_url: https://github.com/BlueBrain/diameter-synthesis
 init_git: false
 maintainer: Alexis Arnaudon (@arnaudon)
 package_name: diameter_synthesis
 project_description: Diametrize cells.
 project_name: diameter-synthesis
 project_url: https://diameter-synthesis.readthedocs.io
 repository_name: diameter-synthesis
 repository_namespace: BlueBrain
 repository_provider: github
+setup_codeql: false
 ssh_url: git@github.com:BlueBrain/diameter-synthesis.git
-support_py37: false
 team_name: ''
 tracker_url: https://github.com/BlueBrain/diameter-synthesis/issues
 use_pyproject_toml: false
 version: 0.5.1
 
 # End of Copier answers
```

### Comparing `diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/feature_request.yaml` & `diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/.github/ISSUE_TEMPLATE/how_to_use.yaml` & `diameter_synthesis-0.6.0/.github/ISSUE_TEMPLATE/how_to_use.yaml`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/.github/dependabot.yml` & `diameter_synthesis-0.6.0/.github/dependabot.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,7 +7,10 @@
 updates:
   # Configure check for outdated GitHub Actions actions in workflows.
   # See: https://docs.github.com/code-security/dependabot/working-with-dependabot/keeping-your-actions-up-to-date-with-dependabot
   - package-ecosystem: "github-actions"
     directory: "/" # Check the repository's workflows under /.github/workflows/
     schedule:
       interval: "weekly"
+    commit-message:
+      # Prefix all commit messages with "CI(dependabot): "
+      prefix: "CI(dependabot): "
```

### Comparing `diameter-synthesis-0.5.4/.github/pull_request_template.md` & `diameter_synthesis-0.6.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/.github/workflows/commitlint.yml` & `diameter_synthesis-0.6.0/.github/workflows/commitlint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     types: [edited, opened, reopened, synchronize]
 
 jobs:
   check-pr-title:
     name: Check PR title
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-node@v3
+      - uses: actions/checkout@v4
+      - uses: actions/setup-node@v4
         with:
-          node-version: '16'
+          node-version: '20'
       - run: npm install -g --force commitlint @commitlint/cli commitlint-plugin-cleanfeet
       - run: npm install conventional-changelog-conventionalcommits
       - run: touch .git/COMMIT_EDITMSG
       - run: echo "${{ github.event.pull_request.title }}" | commitlint
```

### Comparing `diameter-synthesis-0.5.4/.github/workflows/publish-sdist.yml` & `diameter_synthesis-0.6.0/.github/workflows/publish-sdist.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
       - '[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python 3.8
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.8
       - name: Build a wheel and a source tarball
         run: |
           pip install setuptools>=42 build setuptools_scm[toml]>=3.4
           python -m build -o dist
       - name: Publish distribution package to PyPI
```

### Comparing `diameter-synthesis-0.5.4/.github/workflows/run-tox.yml` & `diameter_synthesis-0.6.0/.github/workflows/run-tox.yml`

 * *Files 5% similar despite different names*

```diff
@@ -18,32 +18,32 @@
         exclude:
           - min_versions: "min_versions"
         include:
           - python-version: "3.8"
             min_versions: "min_versions"
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Get current month
       id: date
       run: echo "date=$(date +'%Y-%m')" >> $GITHUB_OUTPUT
     - name: Cache APT Packages
       uses: awalsh128/cache-apt-pkgs-action@latest
       with:
         packages:
             poppler-utils
             imagemagick
         version: 1.0
         execute_install_scripts: true
     - name: Cache tox and precommit environments
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: |
           .tox
           ~/.cache/pre-commit
         key: ${{ runner.os }}-${{ matrix.python-version }}-${{ steps.date.outputs.date }}-${{ hashFiles('setup.py') }}-${{ hashFiles('.pre-commit-config.yaml') }}
     - name: Clear results in tox environments
       run: |
@@ -58,28 +58,29 @@
     - name: Run tox with min versions
       if: ${{ matrix.min_versions == 'min_versions' }}
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox
         tox run -e min_versions
     - name: JUnit Report Action
-      uses: mikepenz/action-junit-report@v3
+      uses: mikepenz/action-junit-report@v4
       if: always() # always run even if the previous step fails
       with:
         report_paths: 'reports/pytest-*.xml'
     - name: Upload to codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: false
-        files: ./reports/coverage-*.xml
+        directory: ./reports
         flags: pytest
-        name: "diameter-synthesis-py${{ matrix.python-version }}"
+        name: "diameter-synthesis-py${{ matrix.python-version }}-${{ matrix.min_versions }}"
+        token: ${{ secrets.CODECOV_TOKEN }}
     - name: Upload test artifacts
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       if: always()
       with:
-        name: tests-${{ matrix.python-version }}
+        name: tests-${{ matrix.python-version }}-${{ matrix.min_versions }}
         retention-days: 4
         path: |
           .tox/py*/tmp
           docs/build
           reports
```

### Comparing `diameter-synthesis-0.5.4/.pre-commit-config.yaml` & `diameter_synthesis-0.6.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,24 @@
             - commit-msg
           additional_dependencies: ['conventional-changelog-conventionalcommits']
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.9.1
     hooks:
       - id: black
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         args: ["-x", ".codespellignorelines"]
   - repo: https://github.com/PyCQA/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies: ["tomli"]
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
       - id: flake8
```

### Comparing `diameter-synthesis-0.5.4/.pylintrc` & `diameter_synthesis-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/CHANGELOG.md` & `diameter_synthesis-0.6.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## [0.6.0](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.5..0.6.0)
+
+> 15 May 2024
+
+### Chores And Housekeeping
+
+- Change license from GPLv3 to Apache-v2 (Adrien Berchet - [#50](https://github.com/BlueBrain/diameter-synthesis/pull/50))
+
+## [0.5.5](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.4..0.5.5)
+
+> 28 March 2024
+
+### New Features
+
+- move fit_orders to config (Alexis Arnaudon - [#48](https://github.com/BlueBrain/diameter-synthesis/pull/48))
+
+### General Changes
+
+- Bump mikepenz/action-junit-report from 3 to 4 (dependabot[bot] - [#39](https://github.com/BlueBrain/diameter-synthesis/pull/39))
+- Bump actions/checkout from 3 to 4 (dependabot[bot] - [#40](https://github.com/BlueBrain/diameter-synthesis/pull/40))
+
 ## [0.5.4](https://github.com/BlueBrain/diameter-synthesis/compare/0.5.3..0.5.4)
 
 > 4 May 2023
 
 ### Fixes
 
 - Handle missing neurites in simpler model (Adrien Berchet - [#36](https://github.com/BlueBrain/diameter-synthesis/pull/36))
```

### Comparing `diameter-synthesis-0.5.4/CITATION.cff` & `diameter_synthesis-0.6.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/CONTRIBUTING.md` & `diameter_synthesis-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/PKG-INFO` & `diameter_synthesis-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,285 +1,219 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6469 616d  : 2.1.Name: diam
-00000020: 6574 6572 2d73 796e 7468 6573 6973 0a56  eter-synthesis.V
-00000030: 6572 7369 6f6e 3a20 302e 352e 340a 5375  ersion: 0.5.4.Su
-00000040: 6d6d 6172 793a 2044 6961 6d65 7472 697a  mmary: Diametriz
-00000050: 6520 6365 6c6c 732e 0a48 6f6d 652d 7061  e cells..Home-pa
-00000060: 6765 3a20 6874 7470 733a 2f2f 6469 616d  ge: https://diam
-00000070: 6574 6572 2d73 796e 7468 6573 6973 2e72  eter-synthesis.r
-00000080: 6561 6474 6865 646f 6373 2e69 6f0a 4175  eadthedocs.io.Au
-00000090: 7468 6f72 3a20 426c 7565 2042 7261 696e  thor: Blue Brain
-000000a0: 2050 726f 6a65 6374 2c20 4550 464c 0a4c   Project, EPFL.L
-000000b0: 6963 656e 7365 3a20 474e 5520 4765 6e65  icense: GNU Gene
-000000c0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
-000000d0: 7365 2076 332e 300a 5072 6f6a 6563 742d  se v3.0.Project-
-000000e0: 5552 4c3a 2054 7261 636b 6572 2c20 6874  URL: Tracker, ht
-000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000100: 2f42 6c75 6542 7261 696e 2f64 6961 6d65  /BlueBrain/diame
-00000110: 7465 722d 7379 6e74 6865 7369 732f 6973  ter-synthesis/is
-00000120: 7375 6573 0a50 726f 6a65 6374 2d55 524c  sues.Project-URL
-00000130: 3a20 536f 7572 6365 2c20 6874 7470 733a  : Source, https:
-00000140: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
-00000150: 6542 7261 696e 2f64 6961 6d65 7465 722d  eBrain/diameter-
-00000160: 7379 6e74 6865 7369 730a 436c 6173 7369  synthesis.Classi
-00000170: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
-00000180: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
-00000190: 4265 7461 0a43 6c61 7373 6966 6965 723a  Beta.Classifier:
-000001a0: 2049 6e74 656e 6465 6420 4175 6469 656e   Intended Audien
-000001b0: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
-000001c0: 7365 6172 6368 0a43 6c61 7373 6966 6965  search.Classifie
-000001d0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-000001e0: 4920 4170 7072 6f76 6564 203a 3a20 474e  I Approved :: GN
-000001f0: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00000200: 204c 6963 656e 7365 2076 3320 2847 504c   License v3 (GPL
-00000210: 7633 290a 436c 6173 7369 6669 6572 3a20  v3).Classifier: 
-00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000230: 7561 6765 203a 3a20 5079 7468 6f6e 0a43  uage :: Python.C
-00000240: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000250: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000260: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
-00000270: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000280: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000290: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000002a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002d0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000002e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000300: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-00000310: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000320: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000330: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000340: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-00000350: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000360: 7269 6e67 203a 3a20 4269 6f2d 496e 666f  ring :: Bio-Info
-00000370: 726d 6174 6963 730a 5265 7175 6972 6573  rmatics.Requires
-00000380: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
-00000390: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000003a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000003b0: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-000003c0: 4578 7472 613a 2064 6f63 730a 5072 6f76  Extra: docs.Prov
-000003d0: 6964 6573 2d45 7874 7261 3a20 706c 6f74  ides-Extra: plot
-000003e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000003f0: 2074 6573 740a 4c69 6365 6e73 652d 4669   test.License-Fi
-00000400: 6c65 3a20 4c49 4345 4e53 452e 7478 740a  le: LICENSE.txt.
-00000410: 4c69 6365 6e73 652d 4669 6c65 3a20 4155  License-File: AU
-00000420: 5448 4f52 532e 6d64 0a0a 5b21 5b56 6572  THORS.md..[![Ver
-00000430: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-00000440: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000450: 692f 762f 6469 616d 6574 6572 2d73 796e  i/v/diameter-syn
-00000460: 7468 6573 6973 295d 2868 7474 7073 3a2f  thesis)](https:/
-00000470: 2f67 6974 6875 622e 636f 6d2f 426c 7565  /github.com/Blue
-00000480: 4272 6169 6e2f 6469 616d 6574 6572 2d73  Brain/diameter-s
-00000490: 796e 7468 6573 6973 2f72 656c 6561 7365  ynthesis/release
-000004a0: 7329 0a5b 215b 4275 696c 6420 7374 6174  s).[![Build stat
-000004b0: 7573 5d28 6874 7470 733a 2f2f 6769 7468  us](https://gith
-000004c0: 7562 2e63 6f6d 2f42 6c75 6542 7261 696e  ub.com/BlueBrain
-000004d0: 2f64 6961 6d65 7465 722d 7379 6e74 6865  /diameter-synthe
-000004e0: 7369 732f 6163 7469 6f6e 732f 776f 726b  sis/actions/work
-000004f0: 666c 6f77 732f 7275 6e2d 746f 782e 796d  flows/run-tox.ym
-00000500: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-00000510: 6368 3d6d 6169 6e29 5d28 6874 7470 733a  ch=main)](https:
-00000520: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
-00000530: 6542 7261 696e 2f64 6961 6d65 7465 722d  eBrain/diameter-
-00000540: 7379 6e74 6865 7369 732f 6163 7469 6f6e  synthesis/action
-00000550: 7329 0a5b 215b 436f 6465 636f 762e 696f  s).[![Codecov.io
-00000560: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
-00000570: 762e 696f 2f67 6974 6875 622f 426c 7565  v.io/github/Blue
-00000580: 4272 6169 6e2f 6469 616d 6574 6572 2d73  Brain/diameter-s
-00000590: 796e 7468 6573 6973 2f63 6f76 6572 6167  ynthesis/coverag
-000005a0: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-000005b0: 6e29 5d28 6874 7470 733a 2f2f 636f 6465  n)](https://code
-000005c0: 636f 762e 696f 2f67 6974 6875 622f 426c  cov.io/github/Bl
-000005d0: 7565 4272 6169 6e2f 6469 616d 6574 6572  ueBrain/diameter
-000005e0: 2d73 796e 7468 6573 6973 3f62 7261 6e63  -synthesis?branc
-000005f0: 683d 6d61 696e 290a 5b21 5b4c 6963 656e  h=main).[![Licen
-00000600: 7365 5d28 6874 7470 733a 2f2f 696d 672e  se](https://img.
-00000610: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000620: 2f4c 6963 656e 7365 2d47 504c 7633 2d62  /License-GPLv3-b
-00000630: 6c75 6529 5d28 6874 7470 733a 2f2f 6769  lue)](https://gi
-00000640: 7468 7562 2e63 6f6d 2f42 6c75 6542 7261  thub.com/BlueBra
-00000650: 696e 2f64 6961 6d65 7465 722d 7379 6e74  in/diameter-synt
-00000660: 6865 7369 732f 626c 6f62 2f6d 6169 6e2f  hesis/blob/main/
-00000670: 4c49 4345 4e53 452e 7478 7429 0a5b 215b  LICENSE.txt).[![
-00000680: 446f 6375 6d65 6e74 6174 696f 6e20 7374  Documentation st
-00000690: 6174 7573 5d28 6874 7470 733a 2f2f 7265  atus](https://re
-000006a0: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
-000006b0: 6f6a 6563 7473 2f64 6961 6d65 7465 722d  ojects/diameter-
-000006c0: 7379 6e74 6865 7369 732f 6261 6467 652f  synthesis/badge/
-000006d0: 3f76 6572 7369 6f6e 3d6c 6174 6573 7429  ?version=latest)
-000006e0: 5d28 6874 7470 733a 2f2f 6469 616d 6574  ](https://diamet
-000006f0: 6572 2d73 796e 7468 6573 6973 2e72 6561  er-synthesis.rea
-00000700: 6474 6865 646f 6373 2e69 6f2f 290a 5b21  dthedocs.io/).[!
-00000710: 5b44 4f49 5d28 6874 7470 733a 2f2f 696d  [DOI](https://im
-00000720: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000730: 6765 2f44 4f49 2d31 302e 3130 3136 2f6a  ge/DOI-10.1016/j
-00000740: 2e63 656c 7265 702e 3230 3232 2e31 3130  .celrep.2022.110
-00000750: 3538 362d 626c 7565 295d 2868 7474 7073  586-blue)](https
-00000760: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-00000770: 3136 2f6a 2e63 656c 7265 702e 3230 3232  16/j.celrep.2022
-00000780: 2e31 3130 3538 3629 0a0a 0a23 2044 6961  .110586)...# Dia
-00000790: 6d65 7465 7220 7379 6e74 6865 7369 730a  meter synthesis.
-000007a0: 0a54 6869 7320 636f 6465 2061 696d 7320  .This code aims 
-000007b0: 6174 2067 656e 6572 6174 696e 6720 7379  at generating sy
-000007c0: 6e74 6865 7469 6320 6469 616d 6574 6572  nthetic diameter
-000007d0: 7320 666f 7220 6e65 7572 6f6e 732c 2077  s for neurons, w
-000007e0: 6974 6820 7061 7261 6d65 7465 7273 206c  ith parameters l
-000007f0: 6561 726e 6564 2066 726f 6d20 6120 7365  earned from a se
-00000800: 7420 6f66 2062 696f 6c6f 6769 6361 6c20  t of biological 
-00000810: 6e65 7572 6f6e 732e 0a0a 0a23 2320 496e  neurons....## In
-00000820: 7374 616c 6c61 7469 6f6e 0a0a 5573 6520  stallation..Use 
-00000830: 7069 703a 0a0a 6060 6062 6173 680a 7069  pip:..```bash.pi
-00000840: 7020 696e 7374 616c 6c20 6469 616d 6574  p install diamet
-00000850: 6572 2d73 796e 7468 6573 6973 0a60 6060  er-synthesis.```
-00000860: 0a0a 2323 204d 6169 6e20 7573 6167 650a  ..## Main usage.
-00000870: 0a23 2323 2053 7465 7020 313a 2042 7569  .### Step 1: Bui
-00000880: 6c64 696e 6720 6d6f 6465 6c73 0a0a 496e  lding models..In
-00000890: 2066 6f6c 6465 7220 6065 7861 6d70 6c65   folder `example
-000008a0: 602c 2079 6f75 2066 6972 7374 2068 6176  `, you first hav
-000008b0: 6520 746f 206d 6f64 6966 7920 6063 7265  e to modify `cre
-000008c0: 6174 655f 6a73 6f6e 732e 7079 6020 746f  ate_jsons.py` to
-000008d0: 2073 7569 7420 796f 7572 206e 6565 6473   suit your needs
-000008e0: 2e0a 0a59 6f75 2068 6176 6520 7468 6520  ...You have the 
-000008f0: 666f 6c6c 6f77 696e 6720 696d 706f 7274  following import
-00000900: 616e 7420 7061 7261 6d65 7465 7273 2066  ant parameters f
-00000910: 6f72 2074 6865 2064 6963 7420 6065 7874  or the dict `ext
-00000920: 7261 6374 5f6d 6f64 656c 735f 7061 7261  ract_models_para
-00000930: 6d73 603a 0a0a 2d20 606d 6f72 7068 5f70  ms`:..- `morph_p
-00000940: 6174 6860 3a20 7061 7468 2074 6f20 6d6f  ath`: path to mo
-00000950: 7270 686f 6c6f 6779 2066 696c 6573 0a2d  rphology files.-
-00000960: 2060 6d74 7970 6573 5f73 6f72 7460 3a20   `mtypes_sort`: 
-00000970: 686f 7720 746f 206c 6561 726e 2064 6973  how to learn dis
-00000980: 7472 6962 7574 696f 6e73 3a20 6061 6c6c  tributions: `all
-00000990: 6020 746f 2075 7365 2061 6c6c 2074 6f67  ` to use all tog
-000009a0: 6574 6865 722c 2060 6d74 7970 6573 6020  ether, `mtypes` 
-000009b0: 746f 2075 7365 2062 7920 6d74 7970 6573  to use by mtypes
-000009c0: 202c 2060 7375 7065 725f 6d74 7970 6573   , `super_mtypes
-000009d0: 6020 746f 2075 7365 2068 6f6d 6520 6d61  ` to use home ma
-000009e0: 6465 2063 656c 6c73 2074 7970 6573 2028  de cells types (
-000009f0: 7365 6520 6064 6961 6d65 7465 725f 7479  see `diameter_ty
-00000a00: 7065 7360 2062 656c 6f77 290a 2d20 606d  pes` below).- `m
-00000a10: 6f64 656c 7360 3a20 746f 2063 7265 6174  odels`: to creat
-00000a20: 6520 7365 7665 7261 6c20 6d6f 6465 6c73  e several models
-00000a30: 2028 666f 7220 6e6f 7720 7468 6579 2061   (for now they a
-00000a40: 7265 2061 6c6c 2074 6865 2073 616d 652c  re all the same,
-00000a50: 206a 7573 7420 6469 6666 6572 656e 7420   just different 
-00000a60: 7265 616c 6973 6174 696f 6e20 6f66 2072  realisation of r
-00000a70: 616e 646f 6d20 6e75 6d62 6572 7329 0a2d  andom numbers).-
-00000a80: 2060 6e65 7572 6974 655f 7479 7065 7360   `neurite_types`
-00000a90: 3a20 7479 7065 7320 6f66 206e 6575 7269  : types of neuri
-00000aa0: 7465 2074 6f20 6c65 6172 6e20 7061 7261  te to learn para
-00000ab0: 6d65 7465 7273 2066 6f72 0a2d 2060 6578  meters for.- `ex
-00000ac0: 7472 615f 7061 7261 6d73 603a 2064 6963  tra_params`: dic
-00000ad0: 7420 6f66 2061 6464 6974 696f 6e61 6c20  t of additional 
-00000ae0: 6d6f 6465 6c20 7061 7261 6d65 7465 7273  model parameters
-00000af0: 0a0a 2323 2320 5374 6570 2032 3a20 4275  ..### Step 2: Bu
-00000b00: 696c 6469 6e67 2064 6961 6d65 7465 7273  ilding diameters
-00000b10: 0a0a 5468 656e 2073 696d 706c 7920 7275  ..Then simply ru
-00000b20: 6e20 602e 2f72 756e 5f6d 6f64 656c 732e  n `./run_models.
-00000b30: 7368 6020 746f 2063 7265 6174 6520 7468  sh` to create th
-00000b40: 6520 6d6f 6465 6c73 2028 7361 7665 6420  e models (saved 
-00000b50: 696e 2061 206a 736f 6e20 6669 6c65 292e  in a json file).
-00000b60: 0a0a 496e 2060 6372 6561 7465 5f6a 736f  ..In `create_jso
-00000b70: 6e73 2e70 7960 2c20 7468 6520 6469 6374  ns.py`, the dict
-00000b80: 2060 6765 6e65 7261 7465 5f64 6961 6d65   `generate_diame
-00000b90: 7465 7273 5f70 6172 616d 7360 206e 6565  ters_params` nee
-00000ba0: 6473 2074 6f20 6265 2075 7064 6174 6564  ds to be updated
-00000bb0: 2c20 746f 6f2c 2077 6974 6820 656e 7472  , too, with entr
-00000bc0: 6965 7320 6d61 7463 6869 6e67 2074 6865  ies matching the
-00000bd0: 2070 7265 7669 6f75 7320 6469 6374 2e0a   previous dict..
-00000be0: 5468 6520 7061 7468 2069 6e20 606e 6577  The path in `new
-00000bf0: 5f6d 6f72 7068 5f70 6174 6860 2077 696c  _morph_path` wil
-00000c00: 6c20 6265 2077 6865 7265 2074 6865 206e  l be where the n
-00000c10: 6577 206d 6f72 7068 6f6c 6f67 6965 7320  ew morphologies 
-00000c20: 7769 6c6c 2062 6520 7361 7665 642e 0a0a  will be saved...
-00000c30: 5468 656e 2072 756e 2060 2e2f 7275 6e5f  Then run `./run_
-00000c40: 6469 616d 7465 7273 2e73 6860 2074 6f20  diamters.sh` to 
-00000c50: 6765 6e65 7261 7465 2064 6961 6d65 7465  generate diamete
-00000c60: 7273 2e0a 0a0a 2323 2041 6464 6974 696f  rs....## Additio
-00000c70: 6e61 6c20 7363 7269 7074 730a 0a53 6576  nal scripts..Sev
-00000c80: 6572 616c 2061 6464 6974 696f 6e61 6c20  eral additional 
-00000c90: 7363 7269 7074 7320 696e 2066 6f6c 6465  scripts in folde
-00000ca0: 7220 6073 6372 6970 7473 603a 0a0a 2d20  r `scripts`:..- 
-00000cb0: 6064 6961 6d65 7465 722d 6368 6563 6b73  `diameter-checks
-00000cc0: 603a 2072 756e 2074 6865 2064 6961 6d65  `: run the diame
-00000cd0: 7465 722d 6368 6563 6b20 636f 6465 2028  ter-check code (
-00000ce0: 626c 7565 7079 6d6d 2920 6f6e 2074 6865  bluepymm) on the
-00000cf0: 2062 696f 6c6f 6769 6361 6c20 616e 6420   biological and 
-00000d00: 7361 6d70 6c65 6420 6365 6c6c 730a 2d20  sampled cells.- 
-00000d10: 6064 6961 6d65 7465 725f 7479 7065 7360  `diameter_types`
-00000d20: 3a20 636c 7573 7465 7220 6d74 7970 6573  : cluster mtypes
-00000d30: 2075 7369 6e67 2064 6973 7472 6962 7574   using distribut
-00000d40: 696f 6e73 206f 6620 7375 7266 6163 6520  ions of surface 
-00000d50: 6172 6561 7320 2875 7365 7320 7477 6f20  areas (uses two 
-00000d60: 7072 6976 6174 6573 2072 6570 6f73 6974  privates reposit
-00000d70: 6f72 6965 7320 6120 7468 6520 6d6f 6d65  ories a the mome
-00000d80: 6e74 290a 2d20 6065 7874 7261 6374 5f6d  nt).- `extract_m
-00000d90: 6f72 7068 6f6d 6574 7269 6373 603a 2066  orphometrics`: f
-00000da0: 726f 6d20 6269 6f20 616e 6420 7361 6d70  rom bio and samp
-00000db0: 6c65 2063 656c 6c73 2c20 6578 7472 6163  le cells, extrac
-00000dc0: 7473 2061 6e64 2070 6c6f 7420 6469 7374  ts and plot dist
-00000dd0: 7269 6275 7469 6f6e 206f 6620 7375 7266  ribution of surf
-00000de0: 6163 6520 6172 6561 2061 6e64 2064 6961  ace area and dia
-00000df0: 6d65 7465 7220 6173 2061 2066 756e 6374  meter as a funct
-00000e00: 696f 6e20 6f66 2062 7261 6e63 6820 6f72  ion of branch or
-00000e10: 6465 7220 616e 6420 7061 7468 206c 656e  der and path len
-00000e20: 6774 6873 0a2d 2060 6578 7472 6163 745f  gths.- `extract_
-00000e30: 6d6f 7270 686f 6c6f 6769 6573 603a 2066  morphologies`: f
-00000e40: 726f 6d20 6120 6365 6c6c 2072 656c 6561  rom a cell relea
-00000e50: 7365 2c20 6669 6e64 2074 6865 206f 6e65  se, find the one
-00000e60: 7320 7468 6174 2063 616e 2062 6520 7275  s that can be ru
-00000e70: 6e20 7468 726f 7567 6820 6469 616d 6574  n through diamet
-00000e80: 6572 2d63 6865 636b 0a2d 2060 706c 6f74  er-check.- `plot
-00000e90: 5f6d 6f72 7068 6f6c 6f67 6965 7360 3a20  _morphologies`: 
-00000ea0: 706c 6f74 2061 6c6c 206d 6f72 7068 6f6c  plot all morphol
-00000eb0: 6f67 6965 7320 696e 206d 7479 7065 2066  ogies in mtype f
-00000ec0: 6f6c 6465 7273 0a0a 0a23 2320 4578 616d  olders...## Exam
-00000ed0: 706c 6573 0a0a 5468 6520 6065 7861 6d70  ples..The `examp
-00000ee0: 6c65 7360 2066 6f6c 6465 7220 636f 6e74  les` folder cont
-00000ef0: 6169 6e73 2061 2073 696d 706c 6520 6578  ains a simple ex
-00000f00: 616d 706c 6520 7468 6174 2077 696c 6c20  ample that will 
-00000f10: 6665 7463 6820 6d6f 7270 686f 6c6f 6769  fetch morphologi
-00000f20: 6573 2066 726f 6d20 5b6e 6575 726f 6d6f  es from [neuromo
-00000f30: 7270 686f 2e6f 7267 5d28 6874 7470 3a2f  rpho.org](http:/
-00000f40: 2f6e 6575 726f 6d6f 7270 686f 2e6f 7267  /neuromorpho.org
-00000f50: 292c 206c 6561 726e 2061 2064 6961 6d65  ), learn a diame
-00000f60: 7465 7220 6d6f 6465 6c2c 2072 6564 6961  ter model, redia
-00000f70: 6d65 7472 697a 6520 7468 6573 6520 6d6f  metrize these mo
-00000f80: 7270 686f 6c6f 6769 6573 2c20 616e 6420  rphologies, and 
-00000f90: 7065 7266 6f72 6d20 736f 6d65 2061 6e61  perform some ana
-00000fa0: 6c79 7369 7320 6f66 2074 6865 2072 6573  lysis of the res
-00000fb0: 756c 7473 2074 6f20 636f 6d70 6172 6520  ults to compare 
-00000fc0: 6f72 6967 696e 616c 2061 6e64 2064 6961  original and dia
-00000fd0: 6d65 7472 697a 6564 206d 6f72 7068 6f6c  metrized morphol
-00000fe0: 6f67 6965 732e 0a54 6869 7320 6578 616d  ogies..This exam
-00000ff0: 706c 6520 6361 6e20 7369 6d70 6c79 2062  ple can simply b
-00001000: 6520 7275 6e20 7573 696e 6720 7468 6520  e run using the 
-00001010: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00001020: 643a 0a60 6060 6261 7368 0a2e 2f72 756e  d:.```bash../run
-00001030: 2e73 680a 6060 600a 0a0a 2323 2046 756e  .sh.```...## Fun
-00001040: 6469 6e67 2026 2041 636b 6e6f 776c 6564  ding & Acknowled
-00001050: 676d 656e 740a 0a54 6865 2064 6576 656c  gment..The devel
-00001060: 6f70 6d65 6e74 206f 6620 7468 6973 2073  opment of this s
-00001070: 6f66 7477 6172 6520 7761 7320 7375 7070  oftware was supp
-00001080: 6f72 7465 6420 6279 2066 756e 6469 6e67  orted by funding
-00001090: 2074 6f20 7468 6520 426c 7565 2042 7261   to the Blue Bra
-000010a0: 696e 2050 726f 6a65 6374 2c20 6120 7265  in Project, a re
-000010b0: 7365 6172 6368 2063 656e 7465 7220 6f66  search center of
-000010c0: 2074 6865 20c3 8963 6f6c 6520 706f 6c79   the ..cole poly
-000010d0: 7465 6368 6e69 7175 6520 66c3 a964 c3a9  technique f..d..
-000010e0: 7261 6c65 2064 6520 4c61 7573 616e 6e65  rale de Lausanne
-000010f0: 2028 4550 464c 292c 2066 726f 6d20 7468   (EPFL), from th
-00001100: 6520 5377 6973 7320 676f 7665 726e 6d65  e Swiss governme
-00001110: 6e74 e280 9973 2045 5448 2042 6f61 7264  nt...s ETH Board
-00001120: 206f 6620 7468 6520 5377 6973 7320 4665   of the Swiss Fe
-00001130: 6465 7261 6c20 496e 7374 6974 7574 6573  deral Institutes
-00001140: 206f 6620 5465 6368 6e6f 6c6f 6779 2e0a   of Technology..
-00001150: 0a46 6f72 206c 6963 656e 7365 2061 6e64  .For license and
-00001160: 2061 7574 686f 7273 2c20 7365 6520 604c   authors, see `L
-00001170: 4943 454e 5345 2e74 7874 6020 616e 6420  ICENSE.txt` and 
-00001180: 6041 5554 484f 5253 2e6d 6460 2072 6573  `AUTHORS.md` res
-00001190: 7065 6374 6976 656c 792e 0a0a 436f 7079  pectively...Copy
-000011a0: 7269 6768 7420 c2a9 2032 3032 312d 3230  right .. 2021-20
-000011b0: 3232 2042 6c75 6520 4272 6169 6e20 5072  22 Blue Brain Pr
-000011c0: 6f6a 6563 742f 4550 464c 0a              oject/EPFL.
+00000000: 5b21 5b56 6572 7369 6f6e 5d28 6874 7470  [![Version](http
+00000010: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000020: 696f 2f70 7970 692f 762f 6469 616d 6574  io/pypi/v/diamet
+00000030: 6572 2d73 796e 7468 6573 6973 295d 2868  er-synthesis)](h
+00000040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000050: 6d2f 426c 7565 4272 6169 6e2f 6469 616d  m/BlueBrain/diam
+00000060: 6574 6572 2d73 796e 7468 6573 6973 2f72  eter-synthesis/r
+00000070: 656c 6561 7365 7329 0a5b 215b 4275 696c  eleases).[![Buil
+00000080: 6420 7374 6174 7573 5d28 6874 7470 733a  d status](https:
+00000090: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
+000000a0: 6542 7261 696e 2f64 6961 6d65 7465 722d  eBrain/diameter-
+000000b0: 7379 6e74 6865 7369 732f 6163 7469 6f6e  synthesis/action
+000000c0: 732f 776f 726b 666c 6f77 732f 7275 6e2d  s/workflows/run-
+000000d0: 746f 782e 796d 6c2f 6261 6467 652e 7376  tox.yml/badge.sv
+000000e0: 673f 6272 616e 6368 3d6d 6169 6e29 5d28  g?branch=main)](
+000000f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000100: 6f6d 2f42 6c75 6542 7261 696e 2f64 6961  om/BlueBrain/dia
+00000110: 6d65 7465 722d 7379 6e74 6865 7369 732f  meter-synthesis/
+00000120: 6163 7469 6f6e 7329 0a5b 215b 436f 6465  actions).[![Code
+00000130: 636f 762e 696f 5d28 6874 7470 733a 2f2f  cov.io](https://
+00000140: 636f 6465 636f 762e 696f 2f67 6974 6875  codecov.io/githu
+00000150: 622f 426c 7565 4272 6169 6e2f 6469 616d  b/BlueBrain/diam
+00000160: 6574 6572 2d73 796e 7468 6573 6973 2f63  eter-synthesis/c
+00000170: 6f76 6572 6167 652e 7376 673f 6272 616e  overage.svg?bran
+00000180: 6368 3d6d 6169 6e29 5d28 6874 7470 733a  ch=main)](https:
+00000190: 2f2f 636f 6465 636f 762e 696f 2f67 6974  //codecov.io/git
+000001a0: 6875 622f 426c 7565 4272 6169 6e2f 6469  hub/BlueBrain/di
+000001b0: 616d 6574 6572 2d73 796e 7468 6573 6973  ameter-synthesis
+000001c0: 3f62 7261 6e63 683d 6d61 696e 290a 5b21  ?branch=main).[!
+000001d0: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
+000001e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000001f0: 2f62 6164 6765 2f4c 6963 656e 7365 2d47  /badge/License-G
+00000200: 504c 7633 2d62 6c75 6529 5d28 6874 7470  PLv3-blue)](http
+00000210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
+00000220: 6c75 6542 7261 696e 2f64 6961 6d65 7465  lueBrain/diamete
+00000230: 722d 7379 6e74 6865 7369 732f 626c 6f62  r-synthesis/blob
+00000240: 2f6d 6169 6e2f 4c49 4345 4e53 452e 7478  /main/LICENSE.tx
+00000250: 7429 0a5b 215b 446f 6375 6d65 6e74 6174  t).[![Documentat
+00000260: 696f 6e20 7374 6174 7573 5d28 6874 7470  ion status](http
+00000270: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
+00000280: 6f72 672f 7072 6f6a 6563 7473 2f64 6961  org/projects/dia
+00000290: 6d65 7465 722d 7379 6e74 6865 7369 732f  meter-synthesis/
+000002a0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+000002b0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+000002c0: 6469 616d 6574 6572 2d73 796e 7468 6573  diameter-synthes
+000002d0: 6973 2e72 6561 6474 6865 646f 6373 2e69  is.readthedocs.i
+000002e0: 6f2f 290a 5b21 5b44 4f49 5d28 6874 7470  o/).[![DOI](http
+000002f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000300: 696f 2f62 6164 6765 2f44 4f49 2d31 302e  io/badge/DOI-10.
+00000310: 3130 3136 2f6a 2e63 656c 7265 702e 3230  1016/j.celrep.20
+00000320: 3232 2e31 3130 3538 362d 626c 7565 295d  22.110586-blue)]
+00000330: 2868 7474 7073 3a2f 2f64 6f69 2e6f 7267  (https://doi.org
+00000340: 2f31 302e 3130 3136 2f6a 2e63 656c 7265  /10.1016/j.celre
+00000350: 702e 3230 3232 2e31 3130 3538 3629 0a0a  p.2022.110586)..
+00000360: 0a23 2044 6961 6d65 7465 7220 7379 6e74  .# Diameter synt
+00000370: 6865 7369 730a 0a54 6869 7320 636f 6465  hesis..This code
+00000380: 2061 696d 7320 6174 2067 656e 6572 6174   aims at generat
+00000390: 696e 6720 7379 6e74 6865 7469 6320 6469  ing synthetic di
+000003a0: 616d 6574 6572 7320 666f 7220 6e65 7572  ameters for neur
+000003b0: 6f6e 732c 2077 6974 6820 7061 7261 6d65  ons, with parame
+000003c0: 7465 7273 206c 6561 726e 6564 2066 726f  ters learned fro
+000003d0: 6d20 6120 7365 7420 6f66 2062 696f 6c6f  m a set of biolo
+000003e0: 6769 6361 6c20 6e65 7572 6f6e 732e 0a0a  gical neurons...
+000003f0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000400: 0a0a 5573 6520 7069 703a 0a0a 6060 6062  ..Use pip:..```b
+00000410: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00000420: 6469 616d 6574 6572 2d73 796e 7468 6573  diameter-synthes
+00000430: 6973 0a60 6060 0a0a 2323 204d 6169 6e20  is.```..## Main 
+00000440: 7573 6167 650a 0a23 2323 2053 7465 7020  usage..### Step 
+00000450: 313a 2042 7569 6c64 696e 6720 6d6f 6465  1: Building mode
+00000460: 6c73 0a0a 496e 2066 6f6c 6465 7220 6065  ls..In folder `e
+00000470: 7861 6d70 6c65 602c 2079 6f75 2066 6972  xample`, you fir
+00000480: 7374 2068 6176 6520 746f 206d 6f64 6966  st have to modif
+00000490: 7920 6063 7265 6174 655f 6a73 6f6e 732e  y `create_jsons.
+000004a0: 7079 6020 746f 2073 7569 7420 796f 7572  py` to suit your
+000004b0: 206e 6565 6473 2e0a 0a59 6f75 2068 6176   needs...You hav
+000004c0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+000004d0: 696d 706f 7274 616e 7420 7061 7261 6d65  important parame
+000004e0: 7465 7273 2066 6f72 2074 6865 2064 6963  ters for the dic
+000004f0: 7420 6065 7874 7261 6374 5f6d 6f64 656c  t `extract_model
+00000500: 735f 7061 7261 6d73 603a 0a0a 2d20 606d  s_params`:..- `m
+00000510: 6f72 7068 5f70 6174 6860 3a20 7061 7468  orph_path`: path
+00000520: 2074 6f20 6d6f 7270 686f 6c6f 6779 2066   to morphology f
+00000530: 696c 6573 0a2d 2060 6d74 7970 6573 5f73  iles.- `mtypes_s
+00000540: 6f72 7460 3a20 686f 7720 746f 206c 6561  ort`: how to lea
+00000550: 726e 2064 6973 7472 6962 7574 696f 6e73  rn distributions
+00000560: 3a20 6061 6c6c 6020 746f 2075 7365 2061  : `all` to use a
+00000570: 6c6c 2074 6f67 6574 6865 722c 2060 6d74  ll together, `mt
+00000580: 7970 6573 6020 746f 2075 7365 2062 7920  ypes` to use by 
+00000590: 6d74 7970 6573 202c 2060 7375 7065 725f  mtypes , `super_
+000005a0: 6d74 7970 6573 6020 746f 2075 7365 2068  mtypes` to use h
+000005b0: 6f6d 6520 6d61 6465 2063 656c 6c73 2074  ome made cells t
+000005c0: 7970 6573 2028 7365 6520 6064 6961 6d65  ypes (see `diame
+000005d0: 7465 725f 7479 7065 7360 2062 656c 6f77  ter_types` below
+000005e0: 290a 2d20 606d 6f64 656c 7360 3a20 746f  ).- `models`: to
+000005f0: 2063 7265 6174 6520 7365 7665 7261 6c20   create several 
+00000600: 6d6f 6465 6c73 2028 666f 7220 6e6f 7720  models (for now 
+00000610: 7468 6579 2061 7265 2061 6c6c 2074 6865  they are all the
+00000620: 2073 616d 652c 206a 7573 7420 6469 6666   same, just diff
+00000630: 6572 656e 7420 7265 616c 6973 6174 696f  erent realisatio
+00000640: 6e20 6f66 2072 616e 646f 6d20 6e75 6d62  n of random numb
+00000650: 6572 7329 0a2d 2060 6e65 7572 6974 655f  ers).- `neurite_
+00000660: 7479 7065 7360 3a20 7479 7065 7320 6f66  types`: types of
+00000670: 206e 6575 7269 7465 2074 6f20 6c65 6172   neurite to lear
+00000680: 6e20 7061 7261 6d65 7465 7273 2066 6f72  n parameters for
+00000690: 0a2d 2060 6578 7472 615f 7061 7261 6d73  .- `extra_params
+000006a0: 603a 2064 6963 7420 6f66 2061 6464 6974  `: dict of addit
+000006b0: 696f 6e61 6c20 6d6f 6465 6c20 7061 7261  ional model para
+000006c0: 6d65 7465 7273 0a0a 2323 2320 5374 6570  meters..### Step
+000006d0: 2032 3a20 4275 696c 6469 6e67 2064 6961   2: Building dia
+000006e0: 6d65 7465 7273 0a0a 5468 656e 2073 696d  meters..Then sim
+000006f0: 706c 7920 7275 6e20 602e 2f72 756e 5f6d  ply run `./run_m
+00000700: 6f64 656c 732e 7368 6020 746f 2063 7265  odels.sh` to cre
+00000710: 6174 6520 7468 6520 6d6f 6465 6c73 2028  ate the models (
+00000720: 7361 7665 6420 696e 2061 206a 736f 6e20  saved in a json 
+00000730: 6669 6c65 292e 0a0a 496e 2060 6372 6561  file)...In `crea
+00000740: 7465 5f6a 736f 6e73 2e70 7960 2c20 7468  te_jsons.py`, th
+00000750: 6520 6469 6374 2060 6765 6e65 7261 7465  e dict `generate
+00000760: 5f64 6961 6d65 7465 7273 5f70 6172 616d  _diameters_param
+00000770: 7360 206e 6565 6473 2074 6f20 6265 2075  s` needs to be u
+00000780: 7064 6174 6564 2c20 746f 6f2c 2077 6974  pdated, too, wit
+00000790: 6820 656e 7472 6965 7320 6d61 7463 6869  h entries matchi
+000007a0: 6e67 2074 6865 2070 7265 7669 6f75 7320  ng the previous 
+000007b0: 6469 6374 2e0a 5468 6520 7061 7468 2069  dict..The path i
+000007c0: 6e20 606e 6577 5f6d 6f72 7068 5f70 6174  n `new_morph_pat
+000007d0: 6860 2077 696c 6c20 6265 2077 6865 7265  h` will be where
+000007e0: 2074 6865 206e 6577 206d 6f72 7068 6f6c   the new morphol
+000007f0: 6f67 6965 7320 7769 6c6c 2062 6520 7361  ogies will be sa
+00000800: 7665 642e 0a0a 5468 656e 2072 756e 2060  ved...Then run `
+00000810: 2e2f 7275 6e5f 6469 616d 7465 7273 2e73  ./run_diamters.s
+00000820: 6860 2074 6f20 6765 6e65 7261 7465 2064  h` to generate d
+00000830: 6961 6d65 7465 7273 2e0a 0a0a 2323 2041  iameters....## A
+00000840: 6464 6974 696f 6e61 6c20 7363 7269 7074  dditional script
+00000850: 730a 0a53 6576 6572 616c 2061 6464 6974  s..Several addit
+00000860: 696f 6e61 6c20 7363 7269 7074 7320 696e  ional scripts in
+00000870: 2066 6f6c 6465 7220 6073 6372 6970 7473   folder `scripts
+00000880: 603a 0a0a 2d20 6064 6961 6d65 7465 722d  `:..- `diameter-
+00000890: 6368 6563 6b73 603a 2072 756e 2074 6865  checks`: run the
+000008a0: 2064 6961 6d65 7465 722d 6368 6563 6b20   diameter-check 
+000008b0: 636f 6465 2028 626c 7565 7079 6d6d 2920  code (bluepymm) 
+000008c0: 6f6e 2074 6865 2062 696f 6c6f 6769 6361  on the biologica
+000008d0: 6c20 616e 6420 7361 6d70 6c65 6420 6365  l and sampled ce
+000008e0: 6c6c 730a 2d20 6064 6961 6d65 7465 725f  lls.- `diameter_
+000008f0: 7479 7065 7360 3a20 636c 7573 7465 7220  types`: cluster 
+00000900: 6d74 7970 6573 2075 7369 6e67 2064 6973  mtypes using dis
+00000910: 7472 6962 7574 696f 6e73 206f 6620 7375  tributions of su
+00000920: 7266 6163 6520 6172 6561 7320 2875 7365  rface areas (use
+00000930: 7320 7477 6f20 7072 6976 6174 6573 2072  s two privates r
+00000940: 6570 6f73 6974 6f72 6965 7320 6120 7468  epositories a th
+00000950: 6520 6d6f 6d65 6e74 290a 2d20 6065 7874  e moment).- `ext
+00000960: 7261 6374 5f6d 6f72 7068 6f6d 6574 7269  ract_morphometri
+00000970: 6373 603a 2066 726f 6d20 6269 6f20 616e  cs`: from bio an
+00000980: 6420 7361 6d70 6c65 2063 656c 6c73 2c20  d sample cells, 
+00000990: 6578 7472 6163 7473 2061 6e64 2070 6c6f  extracts and plo
+000009a0: 7420 6469 7374 7269 6275 7469 6f6e 206f  t distribution o
+000009b0: 6620 7375 7266 6163 6520 6172 6561 2061  f surface area a
+000009c0: 6e64 2064 6961 6d65 7465 7220 6173 2061  nd diameter as a
+000009d0: 2066 756e 6374 696f 6e20 6f66 2062 7261   function of bra
+000009e0: 6e63 6820 6f72 6465 7220 616e 6420 7061  nch order and pa
+000009f0: 7468 206c 656e 6774 6873 0a2d 2060 6578  th lengths.- `ex
+00000a00: 7472 6163 745f 6d6f 7270 686f 6c6f 6769  tract_morphologi
+00000a10: 6573 603a 2066 726f 6d20 6120 6365 6c6c  es`: from a cell
+00000a20: 2072 656c 6561 7365 2c20 6669 6e64 2074   release, find t
+00000a30: 6865 206f 6e65 7320 7468 6174 2063 616e  he ones that can
+00000a40: 2062 6520 7275 6e20 7468 726f 7567 6820   be run through 
+00000a50: 6469 616d 6574 6572 2d63 6865 636b 0a2d  diameter-check.-
+00000a60: 2060 706c 6f74 5f6d 6f72 7068 6f6c 6f67   `plot_morpholog
+00000a70: 6965 7360 3a20 706c 6f74 2061 6c6c 206d  ies`: plot all m
+00000a80: 6f72 7068 6f6c 6f67 6965 7320 696e 206d  orphologies in m
+00000a90: 7479 7065 2066 6f6c 6465 7273 0a0a 0a23  type folders...#
+00000aa0: 2320 4578 616d 706c 6573 0a0a 5468 6520  # Examples..The 
+00000ab0: 6065 7861 6d70 6c65 7360 2066 6f6c 6465  `examples` folde
+00000ac0: 7220 636f 6e74 6169 6e73 2061 2073 696d  r contains a sim
+00000ad0: 706c 6520 6578 616d 706c 6520 7468 6174  ple example that
+00000ae0: 2077 696c 6c20 6665 7463 6820 6d6f 7270   will fetch morp
+00000af0: 686f 6c6f 6769 6573 2066 726f 6d20 5b6e  hologies from [n
+00000b00: 6575 726f 6d6f 7270 686f 2e6f 7267 5d28  euromorpho.org](
+00000b10: 6874 7470 3a2f 2f6e 6575 726f 6d6f 7270  http://neuromorp
+00000b20: 686f 2e6f 7267 292c 206c 6561 726e 2061  ho.org), learn a
+00000b30: 2064 6961 6d65 7465 7220 6d6f 6465 6c2c   diameter model,
+00000b40: 2072 6564 6961 6d65 7472 697a 6520 7468   rediametrize th
+00000b50: 6573 6520 6d6f 7270 686f 6c6f 6769 6573  ese morphologies
+00000b60: 2c20 616e 6420 7065 7266 6f72 6d20 736f  , and perform so
+00000b70: 6d65 2061 6e61 6c79 7369 7320 6f66 2074  me analysis of t
+00000b80: 6865 2072 6573 756c 7473 2074 6f20 636f  he results to co
+00000b90: 6d70 6172 6520 6f72 6967 696e 616c 2061  mpare original a
+00000ba0: 6e64 2064 6961 6d65 7472 697a 6564 206d  nd diametrized m
+00000bb0: 6f72 7068 6f6c 6f67 6965 732e 0a54 6869  orphologies..Thi
+00000bc0: 7320 6578 616d 706c 6520 6361 6e20 7369  s example can si
+00000bd0: 6d70 6c79 2062 6520 7275 6e20 7573 696e  mply be run usin
+00000be0: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
+00000bf0: 636f 6d6d 616e 643a 0a60 6060 6261 7368  command:.```bash
+00000c00: 0a2e 2f72 756e 2e73 680a 6060 600a 0a0a  ../run.sh.```...
+00000c10: 2323 2046 756e 6469 6e67 2026 2041 636b  ## Funding & Ack
+00000c20: 6e6f 776c 6564 676d 656e 740a 0a54 6865  nowledgment..The
+00000c30: 2064 6576 656c 6f70 6d65 6e74 206f 6620   development of 
+00000c40: 7468 6973 2073 6f66 7477 6172 6520 7761  this software wa
+00000c50: 7320 7375 7070 6f72 7465 6420 6279 2066  s supported by f
+00000c60: 756e 6469 6e67 2074 6f20 7468 6520 426c  unding to the Bl
+00000c70: 7565 2042 7261 696e 2050 726f 6a65 6374  ue Brain Project
+00000c80: 2c20 6120 7265 7365 6172 6368 2063 656e  , a research cen
+00000c90: 7465 7220 6f66 2074 6865 20c3 8963 6f6c  ter of the ..col
+00000ca0: 6520 706f 6c79 7465 6368 6e69 7175 6520  e polytechnique 
+00000cb0: 66c3 a964 c3a9 7261 6c65 2064 6520 4c61  f..d..rale de La
+00000cc0: 7573 616e 6e65 2028 4550 464c 292c 2066  usanne (EPFL), f
+00000cd0: 726f 6d20 7468 6520 5377 6973 7320 676f  rom the Swiss go
+00000ce0: 7665 726e 6d65 6e74 e280 9973 2045 5448  vernment...s ETH
+00000cf0: 2042 6f61 7264 206f 6620 7468 6520 5377   Board of the Sw
+00000d00: 6973 7320 4665 6465 7261 6c20 496e 7374  iss Federal Inst
+00000d10: 6974 7574 6573 206f 6620 5465 6368 6e6f  itutes of Techno
+00000d20: 6c6f 6779 2e0a 0a46 6f72 206c 6963 656e  logy...For licen
+00000d30: 7365 2061 6e64 2061 7574 686f 7273 2c20  se and authors, 
+00000d40: 7365 6520 604c 4943 454e 5345 2e74 7874  see `LICENSE.txt
+00000d50: 6020 616e 6420 6041 5554 484f 5253 2e6d  ` and `AUTHORS.m
+00000d60: 6460 2072 6573 7065 6374 6976 656c 792e  d` respectively.
+00000d70: 0a0a 436f 7079 7269 6768 7420 c2a9 2032  ..Copyright .. 2
+00000d80: 3032 312d 3230 3232 2042 6c75 6520 4272  021-2022 Blue Br
+00000d90: 6169 6e20 5072 6f6a 6563 742f 4550 464c  ain Project/EPFL
+00000da0: 0a                                       .
```

### Comparing `diameter-synthesis-0.5.4/commitlint.config.js` & `diameter_synthesis-0.6.0/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/build_diameters.py` & `diameter_synthesis-0.6.0/diameter_synthesis/build_diameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Build neurite diameters from a pre-generated model."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 from collections import deque
 from copy import copy
 from copy import deepcopy
 from functools import partial
 
@@ -163,15 +152,15 @@
         params (dict): model parameters.
         params_tree (dict): specific parameters of the current tree.
         rng (numpy.random.Generator): the random number generator to use.
 
     Returns:
        list: list of daughter diameters.
     """
-    # pylint: disable=too-many-locals
+    # pylint: disable=too-many-locals,used-before-assignment
     major_sections = params_tree["major_sections"]
 
     apply_asymmetry = False
     if params_tree.get("with_asymmetry", False):
         child_not_in_major = [child.id not in major_sections for child in section.children]
         # if children are not asymmetrical, don't apply asymmetry
         if False in child_not_in_major:
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/build_models.py` & `diameter_synthesis-0.6.0/diameter_synthesis/build_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Construct diameter models from cells."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 from functools import partial
 
 from neurom import NeuriteType
 
 import diameter_synthesis.morph_functions as morph_funcs
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/cli.py` & `diameter_synthesis-0.6.0/diameter_synthesis/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Command Line Interface for the diameter_synthesis package."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 # pylint: disable=import-outside-toplevel,redefined-outer-name
 import logging
 import os
 from pathlib import Path
 
 import click
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/distribution_fitting.py` & `diameter_synthesis-0.6.0/diameter_synthesis/distribution_fitting.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Functions to fit distributions to parameters of diameter models."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 # pylint: disable=import-outside-toplevel
 import logging
 
 import numpy as np
 
 from diameter_synthesis.exception import DiameterSynthesisError
@@ -156,14 +145,15 @@
     Args:
         model (dict): the model to use.
         rng (numpy.random.Generator): the random number generator.
 
     Returns:
         float: the value of the distribution at the given position.
     """
+    # pylint: disable=possibly-used-before-assignment
     if "a" in model["params"]:
         a_clip = np.clip(model["params"]["a"], A_MIN, A_MAX)
 
     if model["distribution"] == "constant":
         return model["params"]["value"]
 
     if model["distribution"] == "expon_rev":
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/main.py` & `diameter_synthesis-0.6.0/diameter_synthesis/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Main functions to learn and generate diameters."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import json
 import logging
 import multiprocessing
 import os
 from pathlib import Path
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/morph_functions.py` & `diameter_synthesis-0.6.0/diameter_synthesis/morph_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Morphology extraction functions."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 from functools import lru_cache
 
 import neurom as nm
 import numpy as np
 from neurom.core.morphology import Section
@@ -160,14 +149,15 @@
     return add_additional_attributes(
         [max_diam], neurite, attribute_name=attribute_name, bounds=bounds
     )
 
 
 def trunk_diameter(neurite, attribute_name=None, bounds=None, method="last"):
     """Get the trunc diameters (neurom only)."""
+    # pylint: disable=possibly-used-before-assignment
     if method == "mean":
         trunk_diam = _get_mean_diameter(neurite.root_node)
     if method == "first":
         trunk_diam = _get_diameters(neurite.root_node)[0]
     if method == "last":
         trunk_diam = _get_diameters(neurite.root_node)[-1]
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/plotting.py` & `diameter_synthesis-0.6.0/diameter_synthesis/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Plotting functions."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 import multiprocessing
 import os
 import re
 from copy import copy
 from functools import partial
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/schemas/config.json` & `diameter_synthesis-0.6.0/diameter_synthesis/schemas/config.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/schemas/model_params.json` & `diameter_synthesis-0.6.0/diameter_synthesis/schemas/model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/simpler_diametrizer.py` & `diameter_synthesis-0.6.0/diameter_synthesis/simpler_diametrizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Simpler diametrizer."""
+
 from functools import partial
 
 import matplotlib.pyplot as plt
 import numpy as np
 from neurom import NeuriteType
 from neurom import iter_sections
 from neurom.core.morphology import Morphology
@@ -24,21 +25,23 @@
 
 
 def terminal_path_lengths(neurite, cache):
     """Get the path lengths to each terminal point."""
     return _map_sections(partial(section_path_length, cache=cache), neurite, Section.ileaf)
 
 
-def build_simpler_model(morphologies, config, fit_orders=None):
+def build_simpler_model(morphologies, config):
     """Build diameter model."""
     neurite_types = config.get("neurite_types")
     if neurite_types is None:
         neurite_types = ["basal_dendrite", "apical_dendrite"]
-    if fit_orders is None:
-        fit_orders = {"basal_dendrite": 1, "apical_dendrite": 2, "axon": 1}
+
+    fit_orders = {"basal_dendrite": 1, "apical_dendrite": 2, "axon": 1}
+    if config.get("fit_orders") is not None:
+        fit_orders.update(config["fit_orders"])
 
     coeffs = {n_type: [] for n_type in neurite_types}
     residues = {n_type: None for n_type in neurite_types}
     all_diams = {n_type: [] for n_type in neurite_types}
     all_lengths = {n_type: [] for n_type in neurite_types}
 
     for neurite_type in neurite_types:
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis/utils.py` & `diameter_synthesis-0.6.0/diameter_synthesis/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Utils functions."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import json
 import logging
 import os
 from collections import defaultdict
 from pathlib import Path
 from xml.etree import ElementTree as ET
@@ -38,15 +27,15 @@
         morph_path (str): path to morphologies.
         mtype_file (str): path to dat file.
 
     Returns:
         dict: dictionary of morphologies keyed by mtypes.
     """
     # pylint wrongly determines `morph_name` as TextFileReader
-    # pylint: disable=no-member
+    # pylint: disable=no-member,possibly-used-before-assignment
     morph_name = pd.read_csv(mtypes_file, sep=r"\s+", header=None)
     name_dict = defaultdict(list)
     if not morph_name.empty:
         first_name = morph_name.loc[0, 0]  # pylint: disable=no-member
         file_list = Path(morph_path).glob(first_name + "*")
         try:
             ext = next(file_list).suffix
```

### Comparing `diameter-synthesis-0.5.4/diameter_synthesis.egg-info/SOURCES.txt` & `diameter_synthesis-0.6.0/diameter_synthesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/docs/Makefile` & `diameter_synthesis-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/docs/source/conf.py` & `diameter_synthesis-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/examples/get_morphologies.py` & `diameter_synthesis-0.6.0/examples/get_morphologies.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/examples/rediametrize_single_neuron.py` & `diameter_synthesis-0.6.0/examples/rediametrize_single_neuron.py`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/examples/run.sh` & `diameter_synthesis-0.6.0/examples/run.sh`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/package.json` & `diameter_synthesis-0.6.0/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9711538461538461%*

 * *Differences: {"'auto-changelog'": "{'replaceText': {'(^[bB]uild\\\\((.*)\\\\): ?)': '($2) ', "*

 * *                     "'(^[cC]hore\\\\((.*)\\\\): ?)': '($2) ', '(^[cC][iI]\\\\((.*)\\\\): ?)': "*

 * *                     "'($2) ', '(^[dD]eprecate\\\\((.*)\\\\): ?)': '($2) ', "*

 * *                     "'(^[dD]ocs\\\\((.*)\\\\): ?)': '($2) ', '(^[fF]eat\\\\((.*)\\\\): ?)': '($2) "*

 * *                     "', '(^[fF]ix\\\\((.*)\\\\): ?)': '($2) ', '(^[pP]erf\\\\((.*)\\\\): ?)': "*

 * *                     "'($2) ', '(^[rR]efactor\\\\((.*)\\\ […]*

```diff
@@ -1,33 +1,33 @@
 {
     "auto-changelog": {
         "replaceText": {
             "([bB]reaking change: ?)": "",
             "([bB]reaking: ?)": "",
             "(^[bB]uild: ?)": "",
-            "(^[bB]uild\\((.*)\\): ?)": "\\($2\\)",
+            "(^[bB]uild\\((.*)\\): ?)": "($2) ",
             "(^[cC][iI]: ?)": "",
-            "(^[cC][iI]\\((.*)\\): ?)": "\\($2\\)",
+            "(^[cC][iI]\\((.*)\\): ?)": "($2) ",
             "(^[cC]hore: ?)": "",
-            "(^[cC]hore\\((.*)\\): ?)": "\\($2\\)",
+            "(^[cC]hore\\((.*)\\): ?)": "($2) ",
             "(^[dD]eprecate: ?)": "",
-            "(^[dD]eprecate\\((.*)\\): ?)": "\\($2\\)",
+            "(^[dD]eprecate\\((.*)\\): ?)": "($2) ",
             "(^[dD]ocs: ?)": "",
-            "(^[dD]ocs\\((.*)\\): ?)": "\\($2\\)",
+            "(^[dD]ocs\\((.*)\\): ?)": "($2) ",
             "(^[fF]eat: ?)": "",
-            "(^[fF]eat\\((.*)\\): ?)": "\\($2\\)",
+            "(^[fF]eat\\((.*)\\): ?)": "($2) ",
             "(^[fF]ix: ?)": "",
-            "(^[fF]ix\\((.*)\\): ?)": "\\($2\\)",
+            "(^[fF]ix\\((.*)\\): ?)": "($2) ",
             "(^[pP]erf: ?)": "",
-            "(^[pP]erf\\((.*)\\): ?)": "\\($2\\)",
+            "(^[pP]erf\\((.*)\\): ?)": "($2) ",
             "(^[rR]efactor: ?)": "",
-            "(^[rR]efactor\\((.*)\\): ?)": "\\($2\\)",
+            "(^[rR]efactor\\((.*)\\): ?)": "($2) ",
             "(^[rR]evert: ?)": "",
-            "(^[rR]evert\\((.*)\\): ?)": "\\($2\\)",
+            "(^[rR]evert\\((.*)\\): ?)": "($2) ",
             "(^[sS]tyle: ?)": "",
-            "(^[sS]tyle\\((.*)\\): ?)": "\\($2\\)",
+            "(^[sS]tyle\\((.*)\\): ?)": "($2) ",
             "(^[tT]est: ?)": "",
-            "(^[tT]est\\((.*)\\): ?)": "\\($2\\)"
+            "(^[tT]est\\((.*)\\): ?)": "($2) "
         }
     },
     "name": "diameter-synthesis"
 }
```

### Comparing `diameter-synthesis-0.5.4/pyproject.toml` & `diameter_synthesis-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/conftest.py` & `diameter_synthesis-0.6.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Configuration for the pytest test suite."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 # pylint: disable=redefined-outer-name
 import json
 import shutil
 from pathlib import Path
 
 import morphio.mut
```

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3_diametrized.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3_diametrized.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_1_sample.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized_1_sample.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5` & `diameter_synthesis-0.6.0/tests/data/C030796A-P3_lite_diametrized_astrocyte.h5`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/astro_model_data.json` & `diameter_synthesis-0.6.0/tests/data/astro_model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/astro_model_params.json` & `diameter_synthesis-0.6.0/tests/data/astro_model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/model_data.json` & `diameter_synthesis-0.6.0/tests/data/model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/model_params.json` & `diameter_synthesis-0.6.0/tests/data/model_params.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/simpler_model_data.json` & `diameter_synthesis-0.6.0/tests/data/simpler_model_data.json`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/simpler_morph_diametrized.asc` & `diameter_synthesis-0.6.0/tests/data/simpler_morph_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/small_morph_apical_diametrized.asc` & `diameter_synthesis-0.6.0/tests/data/small_morph_apical_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/small_morph_diametrized.asc` & `diameter_synthesis-0.6.0/tests/data/small_morph_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/data/small_morph_several_apical_diametrized.asc` & `diameter_synthesis-0.6.0/tests/data/small_morph_several_apical_diametrized.asc`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_areas_individual/0_L5_TPC_A_cumulative_section_path_distances_areas_C030796A-P3_lite.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_cumulative_analysis/analysis/L5_TPC_A_cumulative_section_path_distances_volumes_individual/0_L5_TPC_A_cumulative_section_path_distances_volumes_C030796A-P3_lite.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_make_cumulative_figures/cumulative_segment_radial_distances_volumes_individual/0_cumulative_segment_radial_distances_volumes.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_plot_cumulative_distribution.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_plot_cumulative_distribution.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_div.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_plot_diameter_diff_div.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_plot_diameter_diff_mult.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_plot_diameter_diff_mult.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_plot_distribution_fit.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_plot_distribution_fit.pdf`

 * *Files identical despite different names*

### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_violin_analysis.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_violin_analysis.pdf`

 * *Files 18% similar despite different names*

#### Comparing `diameter-synthesis-0.5.4/tests/expected_images/test_violin_analysis.pdf` & `diameter_synthesis-0.6.0/tests/expected_images/test_violin_analysis.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20220706093933+02'00'"
-Creator: 'Matplotlib v3.4.2, https://matplotlib.org'
-Producer: 'Matplotlib pdf backend v3.4.2'
+CreationDate: "D:20231031152847+02'00'"
+Creator: 'Matplotlib v3.8.0, https://matplotlib.org'
+Producer: 'Matplotlib pdf backend v3.8.0'
```

### Comparing `diameter-synthesis-0.5.4/tests/test_build_diameters.py` & `diameter_synthesis-0.6.0/tests/test_build_diameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the build_diameters module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 
 import morphio.mut
 import numpy as np
 import pytest
 from morphio import PointLevel
```

### Comparing `diameter-synthesis-0.5.4/tests/test_build_models.py` & `diameter_synthesis-0.6.0/tests/test_build_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the build_models module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import pytest
 
 from diameter_synthesis import build_models
 from diameter_synthesis.exception import DiameterSynthesisError
 
 from .testing_tools import compare_dicts
```

### Comparing `diameter-synthesis-0.5.4/tests/test_cli.py` & `diameter_synthesis-0.6.0/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Tests for the diameter_synthesis.cli module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import json
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 from numpy.testing import assert_almost_equal
```

### Comparing `diameter-synthesis-0.5.4/tests/test_distribution_fitting.py` & `diameter_synthesis-0.6.0/tests/test_distribution_fitting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the distribution_fitting module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 
 import pytest
 
 from diameter_synthesis import distribution_fitting
 from diameter_synthesis.exception import DiameterSynthesisError
```

### Comparing `diameter-synthesis-0.5.4/tests/test_morph_functions.py` & `diameter_synthesis-0.6.0/tests/test_morph_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the morph_functions module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import pytest
 
 from diameter_synthesis import morph_functions
 from diameter_synthesis.exception import DiameterSynthesisError
```

### Comparing `diameter-synthesis-0.5.4/tests/test_plotting.py` & `diameter_synthesis-0.6.0/tests/test_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the plotting module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import neurom as nm
 import pytest
 from diff_pdf_visually import pdf_similar
 from matplotlib import pyplot as plt
 
 from diameter_synthesis import plotting
```

### Comparing `diameter-synthesis-0.5.4/tests/test_simpler_diametrizer.py` & `diameter_synthesis-0.6.0/tests/test_simpler_diametrizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Test the build_models module."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import morphio.mut
 import neurom as nm
 from morphio import SectionType
 
 from diameter_synthesis import build_diameters
 from diameter_synthesis import build_models
```

### Comparing `diameter-synthesis-0.5.4/tests/testing_tools.py` & `diameter_synthesis-0.6.0/tests/testing_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 """Some tools used in tests."""
 
-# Copyright (C) 2021  Blue Brain Project, EPFL
+# Copyright (C) 2021-2024  Blue Brain Project, EPFL
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: Apache-2.0
 
 import json
 
 import neurom as nm
 import numpy as np
 from numpy.testing import assert_allclose
```

### Comparing `diameter-synthesis-0.5.4/tox.ini` & `diameter_synthesis-0.6.0/tox.ini`

 * *Files identical despite different names*

