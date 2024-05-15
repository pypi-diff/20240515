# Comparing `tmp/sxs-2022.5.6.tar.gz` & `tmp/sxs-2023.0.0.tar.gz`

## Comparing `sxs-2022.5.6.tar` & `sxs-2023.0.0.tar`

### file list

```diff
@@ -1,110 +1,115 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2022.5.6/.codecov.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2022.5.6/.readthedocs.yaml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2022.5.6/CITATION.cff
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 sxs-2022.5.6/mkdocs.yml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2022.5.6/.github/scripts/parse_bump_rule.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 sxs-2022.5.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2022.5.6/.github/workflows/pr_rtd_link.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/index.md -> ../README.md
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/mathematica.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/api/catalog.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/api/horizons.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/api/metadata.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/api/time_series.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/api/waveforms.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/html/main.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/images/favicon.ico
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/javascript/mathjax.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/stylesheets/extra.css
--rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/tutorials/00-Introduction.ipynb
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/tutorials/01-Metadata.ipynb
--rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/tutorials/02-Catalog.ipynb
--rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/tutorials/03-Horizons.ipynb
--rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2022.5.6/docs/tutorials/04-Waveforms.ipynb
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/__version__.py
--rw-r--r--   0        0        0    11405 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/handlers.py
--rw-r--r--   0        0        0    26032 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/time_series.py
--rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/caltechdata/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/caltechdata/catalog.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/caltechdata/login.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/catalog/__init__.py
--rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/catalog/catalog.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/catalog/create.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/catalog/description.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/horizons/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/horizons/spec_horizons_h5.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/horizons/xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/metadata/__init__.py
--rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/metadata/metadata.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/__init__.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/bitwise.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/dicts.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/downloads.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/files.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/formats.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/inspire.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/monotonicity.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/pretty_print.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/select.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/sxs_directories.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/sxs_identifiers.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/url.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/decimation/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/decimation/greedy_spline.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/decimation/linear_bisection.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/decimation/peak_greed.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/decimation/suppression.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/__init__.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/comparisons.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/conversion.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/dataset.py
--rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/horizons.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/metadata.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/waveform_amp_phase.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/lvcnr/waveforms.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/ads.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/arxiv.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/fairchild_report.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/inspire.py
--rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/journal_abbreviations.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/utilities/references/references.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/__init__.py
--rw-r--r--   0        0        0    12399 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/alignment.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/corotating_paired_xor.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/memory.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/mode_utilities.py
--rw-r--r--   0        0        0    20427 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/nrar.py
--rw-r--r--   0        0        0    24896 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/transformations.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/waveform_grid.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/waveform_mixin.py
--rw-r--r--   0        0        0    44751 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/waveform_modes.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/waveforms/waveform_signal.py
--rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/__init__.py
--rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/catalog.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/creators.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/simannex.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/surrogatemodeling.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/api/__init__.py
--rw-r--r--   0        0        0    36876 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/api/deposit.py
--rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/api/login.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2022.5.6/sxs/zenodo/api/records.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/__init__.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/conftest.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_catalog.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_horizons.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_loader.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_metadata.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_time_series.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_transformations.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_utilities.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_waveform_rotations.py
--rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 sxs-2022.5.6/tests/test_waveforms.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 sxs-2022.5.6/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2022.5.6/LICENSE
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 sxs-2022.5.6/README.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 sxs-2022.5.6/pyproject.toml
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 sxs-2022.5.6/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.0.0/.codecov.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.0.0/CITATION.cff
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 sxs-2023.0.0/mkdocs.yml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.0.0/.github/workflows/pr_rtd_link.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/mathematica.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/catalog.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/horizons.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/load.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/metadata.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/time_series.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/api/waveforms.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/html/main.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/javascript/mathjax.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/00-Introduction.ipynb
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/01-Metadata.ipynb
+-rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/02-Catalog.ipynb
+-rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/03-Horizons.ipynb
+-rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.0.0/docs/tutorials/04-Waveforms.ipynb
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/__version__.py
+-rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/handlers.py
+-rw-r--r--   0        0        0    27524 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/time_series.py
+-rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/catalog.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/caltechdata/login.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/__init__.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/catalog.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/create.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/catalog/description.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/spec_horizons_h5.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/horizons/xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/metadata/__init__.py
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/metadata/metadata.py
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/__init__.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/bitwise.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/dicts.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/downloads.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/files.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/formats.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/inspire.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/monotonicity.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/pretty_print.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/select.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/smooth_functions.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/sxs_directories.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/sxs_identifiers.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/url.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/greedy_spline.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/linear_bisection.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/peak_greed.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/decimation/suppression.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/__init__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/comparisons.py
+-rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/conversion.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/dataset.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/horizons.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/metadata.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/waveform_amp_phase.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/lvcnr/waveforms.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/ads.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/arxiv.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/fairchild_report.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/inspire.py
+-rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/journal_abbreviations.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/utilities/references/references.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/__init__.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/alignment.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/memory.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/mode_utilities.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/transformations.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_grid.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_mixin.py
+-rw-r--r--   0        0        0    53506 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_modes.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/waveform_signal.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/__init__.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/lvc.py
+-rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/nrar.py
+-rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/waveforms/format_handlers/spectre_cce_v1.py
+-rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/__init__.py
+-rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/catalog.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/creators.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/simannex.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/surrogatemodeling.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/__init__.py
+-rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/deposit.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/login.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.0.0/sxs/zenodo/api/records.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_catalog.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_horizons.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_loader.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_metadata.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_time_series.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_transformations.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_utilities.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_waveform_rotations.py
+-rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.0.0/tests/test_waveforms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.0.0/LICENSE
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 sxs-2023.0.0/README.md
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 sxs-2023.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 sxs-2023.0.0/PKG-INFO
```

### Comparing `sxs-2022.5.6/mkdocs.yml` & `sxs-2023.0.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   - Tutorials:
     - "tutorials/00-Introduction.ipynb"
     - "tutorials/02-Catalog.ipynb"
     - "tutorials/01-Metadata.ipynb"
     - "tutorials/03-Horizons.ipynb"
     - "tutorials/04-Waveforms.ipynb"
   - API:
+    - "Load": "api/load.md"
     - "Catalog": "api/catalog.md"
     - "Metadata": "api/metadata.md"
     - "Time Series": "api/time_series.md"
     - "Horizons": "api/horizons.md"
     - "Waveforms": "api/waveforms.md"
   - "Calling from Mathematica": "mathematica.md"
```

### Comparing `sxs-2022.5.6/.github/workflows/build.yml` & `sxs-2023.0.0/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,62 +26,65 @@
         !contains(github.event.head_commit.message, '[skip ci]')
         && !contains(github.event.head_commit.message, '[skip tests]')
 
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.8', '3.11']
+        python-version: ['3.8', '3.12']
 
     steps:
       - name: Skip replicates on main branch
         env:
-          skip_replicates: ${{ github.ref == 'refs/heads/main' && (matrix.os != 'ubuntu-latest' || matrix.python-version != '3.11') }}
+          skip_replicates: ${{ github.ref == 'refs/heads/main' && (matrix.os != 'ubuntu-latest' || matrix.python-version != '3.12') }}
         shell: bash
         run: |
           echo "skipping_build_and_test_replicate=${skip_replicates}" >> $GITHUB_ENV
 
       - name: Check out code
         if: ${{ env.skipping_build_and_test_replicate != 'true' }}
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         if: ${{ env.skipping_build_and_test_replicate != 'true' }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install Hatch
         if: ${{ env.skipping_build_and_test_replicate != 'true' }}
         run: pip install --upgrade hatch
 
       - name: Run tests
         if: ${{ env.skipping_build_and_test_replicate != 'true' }}
         run: hatch run test
 
       - name: Upload coverage
-        if: "matrix.python-version == '3.11' && matrix.os == 'ubuntu-latest'"
-        uses: codecov/codecov-action@v3
+        if: "matrix.python-version == '3.12' && matrix.os == 'ubuntu-latest'"
+        uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
 
 
   release:
     name: Create release and send to PyPI
     needs: build
     runs-on: ubuntu-latest
     if: >-
         github.ref == 'refs/heads/main'
+        && github.repository_owner == 'sxs-collaboration'
         && !contains(github.event.head_commit.message, '[no release]')
         && (success() || contains(github.event.head_commit.message, '[skip tests]'))
 
     steps:
       - name: Check out code
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install Hatch
         run: pip install --upgrade hatch
 
       - name: Bump version
@@ -122,20 +125,20 @@
           git tag -a "v${new_version}" -m "Version ${new_version}"
           git status
           git push --follow-tags  # Will not trigger new workflow because it uses GITHUB_TOKEN
 
       - name: Create release
         if: "!contains(github.event.head_commit.message, '[no release]')"
         id: create_release
-        uses: actions/create-release@latest
+        uses: softprops/action-gh-release@v2
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           tag_name: v${{ env.new_version }}
-          release_name: Release v${{ env.new_version }}
+          name: Release v${{ env.new_version }}
           draft: false
           prerelease: false
 
       - name: Publish to PyPI
         if: "!contains(github.event.head_commit.message, '[no pypi]')"
         env:
           # 1) Get key from https://pypi.org/manage/account/token/
```

### Comparing `sxs-2022.5.6/docs/mathematica.md` & `sxs-2023.0.0/docs/mathematica.md`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/images/favicon.ico` & `sxs-2023.0.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/tutorials/00-Introduction.ipynb` & `sxs-2023.0.0/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/tutorials/01-Metadata.ipynb` & `sxs-2023.0.0/docs/tutorials/01-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/tutorials/02-Catalog.ipynb` & `sxs-2023.0.0/docs/tutorials/02-Catalog.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/tutorials/03-Horizons.ipynb` & `sxs-2023.0.0/docs/tutorials/03-Horizons.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/docs/tutorials/04-Waveforms.ipynb` & `sxs-2023.0.0/docs/tutorials/04-Waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/__init__.py` & `sxs-2023.0.0/sxs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 except ModuleNotFoundError:  # pragma: no cover
     import importlib_metadata
 
 __version__ = importlib_metadata.version(__name__)
 
 from . import utilities
 from .utilities import (
-    file_format, sxs_directory, read_config, write_config, sxs_id, lev_number,
+    file_format, sxs_directory, read_config, write_config,
+    sxs_id, lev_number, sxs_id_to_url,
     jit, vectorize, guvectorize, version_info
 )
 from .time_series import TimeSeries
 from .metadata import Metadata
 from .catalog import Catalog
 from .horizons import Horizons, HorizonQuantities
-from .waveforms import WaveformModes #, WaveformGrid, WaveformSignal
+from .waveforms import WaveformModes, WaveformModesDict, to_lvc_conventions #, WaveformGrid, WaveformSignal
 from .waveforms import rotating_paired_xor_multishuffle_bzip2 as rpxmb
 from .waveforms import rotating_paired_diff_multishuffle_bzip2 as rpdmb
+from .waveforms import spectre_cce_v1
 from . import catalog, metadata, horizons, waveforms, zenodo, caltechdata
-from .handlers import load, loadcontext
+from .handlers import load, loadcontext, load_lvc
 
 # The speed of light is, of course, defined to be exactly
 speed_of_light = 299_792_458.0  # m/s
 
 # By "IAU 2012 Resolution B2", the astronomical unit is defined to be exactly
 astronomical_unit = 149_597_870_700.0  # m
 
@@ -44,7 +46,11 @@
 solar_mass_parameter = 1.32712440041e20  # m^3/s^2
 
 # Dividing by the speed of light squared, we get the mass of the sun in meters; dividing again, we
 # get the mass of the sun in seconds. For consistency with the nominal value above, we retain more
 # precision than is warranted by the measurement.
 m_sun_in_meters = 1476.6250385063112526099633973363  # m
 m_sun_in_seconds = 4.925490949162941425997992909269e-06  # s
+
+
+doi_prefix = "10.26138"
+doi_url = f"https://doi.org/{doi_prefix}/"
```

### Comparing `sxs-2022.5.6/sxs/time_series.py` & `sxs-2023.0.0/sxs/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,79 +395,115 @@
     def __repr__(self):
         r = repr(self.ndarray)
         return f"{type(self).__name__}{r[max(0, r.find('(')):-1]}, time={self.time!r}, time_axis={self.time_axis})"
 
     def __str__(self):
         return repr(self)
 
-    def interpolate(self, new_time, derivative_order=0, out=None):
+    def interpolate(self, new_time, derivative_order=0, out=None, padding_points=10):
         """Interpolate this object to a new set of times
 
         Parameters
         ----------
         new_time : array_like
             Points to evaluate the interpolant at
         derivative_order : int, optional
-            Order of derivative to evaluate.  If negative, the antiderivative is
-            returned.  Default value of 0 returns the interpolated data without
-            derivatives or antiderivatives.  Must be between -3 and 3, inclusive.
+            Order of derivative to evaluate.  If negative, the
+            antiderivative is returned.  Default value of 0 returns
+            the interpolated data without derivatives or
+            antiderivatives.  Must be between -3 and 3, inclusive.
+        out : array_like, optional
+            If provided, the result will be placed into this array.
+            It must have the same shape as the result would have been
+            if it was not provided.
+        padding_points : int, optional
+            Number of points to include on either side of `new_time`
+            when constructing interpolating spline, to ensure that the
+            interpolant has enough data to interpolate the whole
+            range.  Default value is 10.  If there are not enough
+            points in the input data to supply all of these padding
+            points, the function will just come as close as possible.
 
         See Also
         --------
         scipy.interpolate.CubicSpline :
             The function that this function is based on.
         antiderivative :
-            Calls this funtion with `new_time=self.time` and
-            `derivative_order=-antiderivative_order` (defaulting to a single
-            antiderivative).
+            Calls this function with `new_time=self.time` and
+            `derivative_order=-antiderivative_order` (defaulting to a
+            single antiderivative).
         derivative :
             Calls this function `new_time=self.time` and
-            `derivative_order=derivative_order` (defaulting to a single derivative).
+            `derivative_order=derivative_order` (defaulting to a
+            single derivative).
         dot :
             Property calling `self.derivative(1)`.
         ddot :
             Property calling `self.derivative(2)`.
         int :
             Property calling `self.antiderivative(1)`.
         iint :
             Property calling `self.antiderivative(2)`.
 
         Notes
         -----
-        This function is essentially a wrapper around `scipy.interpolate.CubicSpline`
+        This function is essentially a wrapper around
+        `scipy.interpolate.CubicSpline`
 
         """
         from scipy.interpolate import CubicSpline
+
         if derivative_order > 3:
             raise ValueError(
                 f"{type(self).__name__} interpolation uses CubicSpline, which cannot take a derivative "
                 f"of order {derivative_order}."
             )
+
+        # Sort out shapes and storage for output
         new_time = np.asarray(new_time)
         if new_time.ndim != 1:
             raise ValueError(f"New time array must have exactly 1 dimension; it has {new_time.ndim}.")
         new_shape = list(self.shape)
         new_shape[self.time_axis] = new_time.size
         if out is not None:
             out = np.asarray(out)
             if out.shape != new_shape:
                 raise ValueError(
-                    f"Output array should have shape {new_shape} for consistency with new time array and modes array"
+                    f"Output array should have shape {new_shape} for consistency with new time "
+                    "array and modes array"
                 )
             if out.dtype != self.dtype:
                 raise ValueError(
-                    f"Output array should have same dtype as this array {self.dtype}; it has dtype {out.dtype}"
+                    f"Output array should have same dtype as this array {self.dtype}; "
+                    f"it has dtype {out.dtype}"
                 )
         result = out or np.empty(new_shape, dtype=self.dtype)
-        spline = CubicSpline(self.time, self.ndarray, axis=self.time_axis)
+
+        # Find a range of indices that includes `new_time`, plus
+        # `padding_points` points in either direction, to ensure that
+        # the spline has enough data to interpolate the whole range.
+        idx_min = max(0, self.index_closest_to(new_time.min()) - padding_points)
+        idx_max = min(self.n_times, self.index_closest_to(new_time.max()) + padding_points)
+        idx = range(idx_min, idx_max)
+
+        # Construct the spline — possibly including derivatives or antiderivatives
+        spline = CubicSpline(
+            self.time[idx],
+            self.ndarray.take(idx, axis=self.time_axis),
+            axis=self.time_axis
+        )
         if derivative_order < 0:
             spline = spline.antiderivative(-derivative_order)
         elif 0 < derivative_order <= 3:
             spline = spline.derivative(derivative_order)
+
+        # Evaluate the spline at the new time points
         result[:] = spline(new_time)
+
+        # Copy metadata and return the result
         metadata = self._metadata.copy()
         metadata["time"] = new_time
         metadata["time_axis"] = self.time_axis
         return type(self)(result, **metadata)
 
     def antiderivative(self, antiderivative_order=1):
         """Integrate modes with respect to time
```

### Comparing `sxs-2022.5.6/sxs/caltechdata/__init__.py` & `sxs-2023.0.0/sxs/caltechdata/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/caltechdata/catalog.py` & `sxs-2023.0.0/sxs/caltechdata/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/caltechdata/login.py` & `sxs-2023.0.0/sxs/caltechdata/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/catalog/catalog.py` & `sxs-2023.0.0/sxs/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/catalog/create.py` & `sxs-2023.0.0/sxs/catalog/create.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/catalog/description.py` & `sxs-2023.0.0/sxs/catalog/description.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/horizons/__init__.py` & `sxs-2023.0.0/sxs/horizons/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/horizons/spec_horizons_h5.py` & `sxs-2023.0.0/sxs/horizons/spec_horizons_h5.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/horizons/xor_multishuffle_bzip2.py` & `sxs-2023.0.0/sxs/horizons/xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/metadata/metadata.py` & `sxs-2023.0.0/sxs/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/__init__.py` & `sxs-2023.0.0/sxs/utilities/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 default_shuffle_widths = (16, 4, 2, 2, 2) + (1,) * 22 + (4,) * 4
 default_shuffle_widths_old = (8, 8, 4, 4, 4, 2,) + (1,) * 34
 
 from . import url, inspire, monotonicity, decimation, lvcnr, references
 from .downloads import download_file
 from .bitwise import diff, xor, multishuffle
 from .sxs_identifiers import (
-    sxs_identifier_regex, sxs_identifier_re, lev_regex, lev_re, sxs_id, lev_number, simulation_title
+    sxs_identifier_regex, sxs_identifier_re, lev_regex, lev_re, sxs_id,
+    lev_number, simulation_title, sxs_id_to_url
+)
+from .sxs_directories import (
+    sxs_directory, read_config, write_config, sxs_path_to_system_path, cached_path
 )
-from .sxs_directories import sxs_directory, read_config, write_config, sxs_path_to_system_path, cached_path
 from .select import select_by_path_component
 from .formats import file_format
 from .pretty_print import fit_to_console
-from .files import md5checksum, lock_file_manager, find_simulation_directories, find_files
+from .files import (
+    md5checksum, lock_file_manager, find_simulation_directories, find_files
+)
 from .dicts import KeyPassingDict
 
 
 def version_info():
     """Find all relevant package versions
 
     This function attempts to import each of the various packages relevant to this
```

### Comparing `sxs-2022.5.6/sxs/utilities/bitwise.py` & `sxs-2023.0.0/sxs/utilities/bitwise.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/dicts.py` & `sxs-2023.0.0/sxs/utilities/dicts.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/downloads.py` & `sxs-2023.0.0/sxs/utilities/downloads.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/files.py` & `sxs-2023.0.0/sxs/utilities/files.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/inspire.py` & `sxs-2023.0.0/sxs/utilities/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/monotonicity.py` & `sxs-2023.0.0/sxs/utilities/monotonicity.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/pretty_print.py` & `sxs-2023.0.0/sxs/utilities/pretty_print.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/select.py` & `sxs-2023.0.0/sxs/utilities/select.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/sxs_directories.py` & `sxs-2023.0.0/sxs/utilities/sxs_directories.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/sxs_identifiers.py` & `sxs-2023.0.0/sxs/utilities/sxs_identifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Simple regexes to understand SXS IDs"""
 
 import re
 
-sxs_identifier_regex = r"(?P<sxs_identifier>SXS:(?P<simulation_type>BBH|BHNS|NSNS):(?P<sxs_number>[0-9]+))(?:v(?P<version>[0-9]+))?"
-lev_regex = r"Lev(?P<lev>[-0-9]*)"
+sxs_identifier_regex = (
+    r"(?P<sxs_identifier>SXS:(?P<simulation_type>BBH|BHNS|NSNS)(?:_ExtCCE)?:"
+    r"(?P<sxs_number>[0-9]+))(?:(v|V)(?P<version>[0-9.]+))?"
+)
+lev_regex = r"Lev(?P<lev>-?[0-9]+)"
 sxs_identifier_re = re.compile(sxs_identifier_regex)
 lev_re = re.compile(lev_regex)
 
 
-def sxs_id(s, default=""):
+def sxs_id(s, default="", include_version=False):
     """Return the SXS ID contained in the input string
 
     An SXS ID is anything that matches the following regular expression:
 
-        SXS:(BBH|BHNS|NSNS):[0-9]*
+        SXS:(BBH|BHNS|NSNS)(_ExtCCE)?:[0-9]+(v[0-9.]+)?
 
     If no match is found, the empty string is returned.  If multiple matches are
     found, only the first is returned.
 
     The input parameter may be:
     1) A string believed to contain the SXS ID
     2) The path to a file (like common-metadata.txt) containing such a string
@@ -42,15 +45,18 @@
                 if sxs_id_line:
                     return sxs_id_line
             return default
     except TypeError:
         pass
     m = re.search(sxs_identifier_regex, s)
     if m:
-        return m["sxs_identifier"]
+        if include_version:
+            return m["sxs_identifier"] + (f"v{m['version']}" if m["version"] else "")
+        else:
+            return m["sxs_identifier"]
     else:
         return default
 
 
 def simulation_title(sxs_id):
     """Create simulation title given just the SXS ID
 
@@ -80,20 +86,24 @@
 
 
 def lev_number(s):
     """Return the integer Lev number contained in the input string
 
     The Lev number is anything that matches the following regular expression:
 
-        Lev(?P<lev>[-0-9]*)
+        Lev(?P<lev>-?[0-9]+)
 
     If no match is found, `None` is returned.  If multiple matches are found,
     only the first is returned.
 
     """
-    import os.path
     import re
     m = re.search(lev_regex, s)
     if m:
         return int(m["lev"])
     else:
         return None
+
+
+def sxs_id_to_url(sxs_id):
+    """Return the DOI URL for the SXS ID"""
+    return f"https://doi.org/10.26138/{sxs_id}"
```

### Comparing `sxs-2022.5.6/sxs/utilities/url.py` & `sxs-2023.0.0/sxs/utilities/url.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/decimation/__init__.py` & `sxs-2023.0.0/sxs/utilities/decimation/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/decimation/greedy_spline.py` & `sxs-2023.0.0/sxs/utilities/decimation/greedy_spline.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/decimation/linear_bisection.py` & `sxs-2023.0.0/sxs/utilities/decimation/linear_bisection.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/decimation/peak_greed.py` & `sxs-2023.0.0/sxs/utilities/decimation/peak_greed.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/decimation/suppression.py` & `sxs-2023.0.0/sxs/utilities/decimation/suppression.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/__init__.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/comparisons.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/comparisons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/conversion.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,35 +44,32 @@
         tolerance : float, optional
             Target tolerance used in `sxs.utilities.greedy_spline.minimal_indices`.
         quiet : bool, optional
             If False (the default), echo each line of the log as it is created;
             otherwise just store the final log in the output file.
 
         """
-        import os
-        import time
-        import json
         import platform
         import numpy
         import scipy
         import h5py
-        import sxs
+        from ... import __version__, load, zenodo
 
         self.modes = modes
         self.tolerance = tolerance
         self.quiet = quiet
 
         self.code_versions = (
             f"python=={platform.python_version()}\n"
             f"numpy=={numpy.version.version}\n"
             f"scipy=={scipy.version.full_version}\n"
             f"h5py=={h5py.version.version}\n"
             f"# h5py_api=={h5py.version.api_version}\n"
             f"# h5py_hdf5=={h5py.version.hdf5_version}\n"
-            f"sxs=={sxs.__version__}\n"
+            f"sxs=={__version__}\n"
         )
 
         self.command = (
             f"sxs.utilities.lvcnr.convert_simulation(\n"
             f"    sxs_data_path={{sxs_data_path!r}},\n"
             f"    out_path={{out_path!r}},\n"
             f"    truncation_time={{truncation_time!r}},\n"
@@ -90,21 +87,21 @@
             self.modes = [[2, 2], [2, -2]]
         else:
             l_max = int(modes)
             self.modes = [[l, m] for l in range(2, l_max + 1) for m in range(-l, l + 1)]
         self.ell_max = max(lm[0] for lm in self.modes)
 
         # Load catalog metadata
-        catalog = sxs.load("catalog")
+        catalog = load("catalog")
         self.sxs_catalog = {
             "simulations": catalog.simulations,
             "records": catalog.records,
         }
 
-        self.sxs_catalog_resolutions = sxs.zenodo.catalog.resolutions_for_simulations(self.sxs_catalog)
+        self.sxs_catalog_resolutions = zenodo.catalog.resolutions_for_simulations(self.sxs_catalog)
 
     def convert(
         self,
         sxs_data_path,
         out_path,
         waveform_name=None,
         out_waveform_name=None,
@@ -144,17 +141,16 @@
             that this is not typically a very effective setting — perhaps providing
             another 10% compression; the output file sizes are dominated by fairly
             redundant time data unaffected by this parameter.
 
         """
         import os
         import time
-        import json
         import h5py
-        import sxs
+        from ... import lev_number, Metadata
 
         from .metadata import sxs_id_from_alt_names, write_metadata_from_sxs
         from .horizons import horizon_splines_from_sxs, write_horizon_splines_from_sxs
         from .waveforms import convert_modes
 
         log = self.Log(self.quiet)
         log(
@@ -162,21 +158,21 @@
                 sxs_data_path=sxs_data_path, out_path=out_path, truncation_time=truncation_time, resolution=resolution
             )
         )
         log("Starting at " + time.strftime("%H:%M%p %Z on %b %d, %Y"))
 
         # Load metadata from this simulation
         try:
-            metadata = sxs.Metadata.from_file(os.path.join(sxs_data_path, "metadata"))
+            metadata = Metadata.from_file(os.path.join(sxs_data_path, "metadata"))
         except:
             raise ValueError("Cannot load metadata.")
 
         # Determine the resolution of the input simulation, if needed
         if resolution is None:
-            resolution = sxs.lev_number(sxs_data_path)
+            resolution = lev_number(sxs_data_path)
         if resolution is None:
             raise ValueError("No `resolution` value found in input arguments or data path.")
 
         sxs_id = sxs_id_from_alt_names(metadata["alternative_names"])
         log("Converting " + sxs_id)
 
         extrapolation_order = "Extrapolated_N2"
```

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/dataset.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/dataset.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/horizons.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/metadata.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/waveform_amp_phase.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/waveform_amp_phase.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/lvcnr/waveforms.py` & `sxs-2023.0.0/sxs/utilities/lvcnr/waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/references/ads.py` & `sxs-2023.0.0/sxs/utilities/references/ads.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/references/arxiv.py` & `sxs-2023.0.0/sxs/utilities/references/arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     return reference
 
 
 def get_journal_reference_from_ads(doi):
     import sys
     import difflib
     import ads
-    from sxs.references.journal_abbreviations import journal_abbreviation_pairs
+    from .journal_abbreviations import journal_abbreviation_pairs
     reference = {'title':'', 'pub':'', 'volume':'', 'issue':'', 'year':'', 'page':''}
     try:
         article = ads.SearchQuery(q="doi:{0}".format(doi), fl=list(reference)).next()
         reference['title'] = article.title
         reference['pub'] = article.pub
         reference['volume'] = article.volume
         reference['issue'] = article.issue
```

### Comparing `sxs-2022.5.6/sxs/utilities/references/fairchild_report.py` & `sxs-2023.0.0/sxs/utilities/references/fairchild_report.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/references/inspire.py` & `sxs-2023.0.0/sxs/utilities/references/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/utilities/references/journal_abbreviations.py` & `sxs-2023.0.0/sxs/utilities/references/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/waveforms/__init__.py` & `sxs-2023.0.0/sxs/waveforms/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """Containers for various types of waveforms
 
-Currently, the most interesting object in this submodule is [`WaveformModes`](../sxs.waveforms.waveform_modes/).
+Currently, the most interesting object in this submodule is
+[`WaveformModes`](../sxs.waveforms.waveform_modes/).
 
 """
 
 from .waveform_mixin import WaveformMixin
-from .waveform_modes import WaveformModes
+from .waveform_modes import WaveformModes, WaveformModesDict
 # from .waveform_grid import WaveformGrid
 # from .waveform_signal import WaveformSignal
 
-from . import nrar, rotating_paired_xor_multishuffle_bzip2, rotating_paired_diff_multishuffle_bzip2, memory, transformations, alignment
+from .format_handlers import (
+    nrar,
+    rotating_paired_diff_multishuffle_bzip2,
+    rotating_paired_xor_multishuffle_bzip2,
+    spectre_cce_v1,
+)
+from .format_handlers.lvc import to_lvc_conventions
+from . import memory, transformations, alignment
 
 # Map a format string to the module that should be used to load a waveform with that format
 formats = {
     None: nrar,
     "": nrar,
     "nrar": nrar,
     "rotating_paired_xor_multishuffle_bzip2": rotating_paired_xor_multishuffle_bzip2,
     "rpxm": rotating_paired_xor_multishuffle_bzip2,
     "rpxmb": rotating_paired_xor_multishuffle_bzip2,
     "rotating_paired_diff_multishuffle_bzip2": rotating_paired_diff_multishuffle_bzip2,
     "rpdmb": rotating_paired_diff_multishuffle_bzip2,
+    "SpECTRE_CCE_v1": spectre_cce_v1,
 }
```

### Comparing `sxs-2022.5.6/sxs/waveforms/alignment.py` & `sxs-2023.0.0/sxs/waveforms/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import sxs
 import numpy as np
 
 from scipy.integrate import trapezoid
 
 import multiprocessing as mp
 from functools import partial
 
 
+
 def align1d(wa, wb, t1, t2, n_brute_force=None):
     """Align waveforms by shifting in time
 
     This function determines the optimal time offset to apply to `wb` by minimizing
     the averaged (over time) squared difference in the L² norms (over the sphere)
     of the waveforms:
 
@@ -204,14 +204,15 @@
     always rely on a specific number of orbits, for example.  Also note that
     neither number should be too close to the beginning or end of either waveform,
     to provide some "wiggle room".
 
     """
     from scipy.interpolate import CubicSpline
     from scipy.optimize import least_squares
+    from .. import WaveformModes
 
     wa_orig = wa
     wa = wa.copy()
     wb = wb.copy()
 
     # Check that (t1, t2) makes sense and is actually contained in both waveforms
     if t2 <= t1:
@@ -288,15 +289,15 @@
         δt_δϕ = δt_δϕ_brute_force[np.argmin(cost_brute_force)]
 
         # Optimize explicitly
         optimum = least_squares(cost_wrapper, δt_δϕ, bounds=[(δt_lower, 0), (δt_upper, 2 * np.pi)], max_nfev=50000)
         optimums.append(optimum)
         δt, δϕ = optimum.x
 
-        wa_prime = sxs.WaveformModes(
+        wa_prime = WaveformModes(
             input_array=(
                 wa_orig[:, wa_orig.index(2, -2) : wa_orig.index(ell_max + 1, -(ell_max + 1))].data
                 * np.exp(1j * m * δϕ)
                 * δΨ_factor
             ),
             time=wa_orig.t - δt,
             time_axis=0,
```

### Comparing `sxs-2022.5.6/sxs/waveforms/memory.py` & `sxs-2023.0.0/sxs/waveforms/memory.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/waveforms/mode_utilities.py` & `sxs-2023.0.0/sxs/waveforms/mode_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/waveforms/nrar.py` & `sxs-2023.0.0/sxs/waveforms/format_handlers/nrar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Handlers for waveforms in the old NRAR data format"""
 
 import sys
 import warnings
 import ast
 import numpy as np
-from . import WaveformModes
-from ..metadata import Metadata
-from ..utilities.monotonicity import index_is_monotonic
+from .. import WaveformModes
+from ...metadata import Metadata
+from ...utilities.monotonicity import index_is_monotonic
 
 
 FrameType = [UnknownFrameType, Inertial, Coprecessing, Coorbital, Corotating] = range(5)
 FrameNames = ["UnknownFrameType", "Inertial", "Coprecessing", "Coorbital", "Corotating"]
 
 DataType = [UnknownDataType, psi0, psi1, psi2, psi3, psi4, sigma, h, hdot, news, psin] = range(11)
 DataNames = ["UnknownDataType", "Psi0", "Psi1", "Psi2", "Psi3", "Psi4", "sigma", "h", "hdot", "news", "psin"]
@@ -143,15 +143,15 @@
 
     """
     import pathlib
     import re
     import h5py
     import quaternionic
     import spherical
-    from ..utilities import KeyPassingDict
+    from ...utilities import KeyPassingDict
 
     # This unfortunate concoction is needed to determine the (ell,m) values of the various mode data sets
     pattern_Ylm = re.compile(r"""Y_l(?P<L>[0-9]+)_m(?P<M>[-+0-9]+)\.dat""")
 
     # Initialize an empty object to be filled with goodies
     w_attributes = {}
```

### Comparing `sxs-2022.5.6/sxs/waveforms/rotating_paired_diff_multishuffle_bzip2.py` & `sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,118 +1,138 @@
 """Functions to load and save waveforms in RPDMB format"""
 
-import sys
 import warnings
 import tempfile
 import contextlib
 import pathlib
+import numbers
 import bz2
 import json
 import numpy as np
-import scipy
 import h5py
 import quaternionic
-import spherical
 
-from . import WaveformModes
-from .. import __version__
-from ..utilities import default_shuffle_widths, md5checksum, diff, xor, multishuffle, version_info
+from ...utilities import default_shuffle_widths, md5checksum, diff, xor, multishuffle, version_info
+from ... import Metadata, __version__
+from .. import WaveformModes
 
 
 sxs_formats = ["rotating_paired_diff_multishuffle_bzip2", "rpdmb", "RPDMB"]
 
 
 def save(
         w, file_name=None, file_write_mode="w",
         L2norm_fractional_tolerance=1e-10, log_frame=None,
         shuffle_widths=default_shuffle_widths, convert_to_conjugate_pairs=True,
         compression=bz2, diff=diff, formats=None, verbose=True, allow_existing_group=False,
-        version_info_update=None,
+        version_info_update=None, max_phase_per_timestep=None
 ):
     """Save a waveform in RPDMB format
 
-    This function converts the data to "rotating paired diff multishuffle bzip2"
-    format.  In particular, it uses the corotating frame, and zeroes out bits at
-    high precision to allow for optimal compression while maintaining the requested
-    tolerance.
+    This function converts the data to "rotating paired diff
+    multishuffle bzip2" format.  In particular, it uses the corotating
+    frame, and zeroes out bits at high precision to allow for optimal
+    compression while maintaining the requested tolerance.
 
-    Optionally, with appropriate inputs, can provide different formats.
+    Optionally, with appropriate inputs, can provide different
+    formats.
 
     Parameters
     ----------
     w : WaveformModes
         A waveform in either the inertial or corotating frame
     file_name : str
-        Relative or absolute path to the output HDF5 file.  If this string contains
-        `'.h5'` but does not *end* with that, the remainder of the string is taken
-        to be the group within the HDF5 file in which the data should be stored.
-        Also note that a JSON file is created in the same location, with `.h5`
-        replaced by `.json` (and the corresponding data is stored under the `group`
-        key if relevant).  To retrieve just the return values, or for testing
-        purposes, this argument may be `None`, in which case a temporary directory
-        is used, just to test how large the output will be; it is deleted
-        immediately upon returning.
+        Relative or absolute path to the output HDF5 file.  If this
+        string contains `'.h5'` but does not *end* with that, the
+        remainder of the string is taken to be the group within the
+        HDF5 file in which the data should be stored.  Also note that
+        a JSON file is created in the same location, with `.h5`
+        replaced by `.json` (and the corresponding data is stored
+        under the `group` key if relevant).  To retrieve just the
+        return values, or for testing purposes, this argument may be
+        `None`, in which case a temporary directory is used, just to
+        test how large the output will be; it is deleted immediately
+        upon returning.
     file_write_mode : str, optional
         One of the valid [file modes for
         h5py](https://docs.h5py.org/en/stable/high/file.html#opening-creating-files).
-        Default value is `"w"`, which overwrites any existing file.  If writing
-        into a group, you may prefer `"a"`, which will just ensure the file exists
-        without erasing it first.
+        Default value is `"w"`, which overwrites any existing file.
+        If writing into a group, you may prefer `"a"`, which will just
+        ensure the file exists without erasing it first.
     L2norm_fractional_tolerance : float, optional
-        Tolerance passed to `WaveformModes.truncate`; see that function's docstring
-        for details.  Default value is 1e-10.
+        Tolerance passed to `WaveformModes.truncate`; see that
+        function's docstring for details.  Default value is 1e-10.
     log_frame : array of quaternions, optional
-        If this argument is given the waveform must be in the corotating frame, and
-        the given data will be used as the logarithmic frame data.  If this
-        argument is `None` (the default), this will be calculated when the waveform
-        is transformed to the corotating frame, or simply taken directly from the
-        waveform if it is already corotating.
+        If this argument is given the waveform must be in the
+        corotating frame, and the given data will be used as the
+        logarithmic frame data.  If this argument is `None` (the
+        default), this will be calculated when the waveform is
+        transformed to the corotating frame, or simply taken directly
+        from the waveform if it is already corotating.
     shuffle_widths : iterable of ints, optional
-        See `sxs.utilities.multishuffle` for details.  The default value is
-        `default_shuffle_widths`.  Note that if `L2norm_fractional_tolerance` is
-        0.0, this will be ignored and the standard HDF5 shuffle option will be used
-        instead.
+        See `sxs.utilities.multishuffle` for details.  The default
+        value is `default_shuffle_widths`.  Note that if
+        `L2norm_fractional_tolerance` is 0.0, this will be ignored and
+        the standard HDF5 shuffle option will be used instead.
     convert_to_conjugate_pairs : bool, optional
-        If `True` (the default), the data is converted to conjugate-pair form.
+        If `True` (the default), the data is converted to
+        conjugate-pair form.
     compression : module, optional
-        Compression module (or any other object) with `compress` and `decompress`
-        methods.  Default value is `bz2`, which is part of python's standard
-        library, and performs bzip2 de/compression.  Note that whatever this is
-        must be available to the `load` code, so this should probably be oneof the
+        Compression module (or any other object) with `compress` and
+        `decompress` methods.  Default value is `bz2`, which is part
+        of python's standard library, and performs bzip2
+        de/compression.  Note that whatever this is must be available
+        to the `load` code, so this should probably be oneof the
         built-in packages: `bz2`, `lmza`, `gzip`, or `zlib`.
     diff : function, optional
-        Function to compare successive values.  Defaults to `diff`, which is the
-        floating-point difference.  Other possibilities include `diffInt` (which
-        reinterprets the data as integers before taking the difference) and `xor`
-        (which is the previous default); neither works as well with our data at the
-        time of this writing.
+        Function to compare successive values.  Defaults to `diff`,
+        which is the floating-point difference.  Other possibilities
+        include `diffInt` (which reinterprets the data as integers
+        before taking the difference) and `xor` (which is the previous
+        default); neither works as well with our data at the time of
+        this writing.
     formats : array[str], optional
-        Possible names of the format.  Defaults to variations on `RPDMB`.
+        Possible names of the format.  Defaults to variations on
+        `RPDMB`.
     allow_existing_group : bool, optional
-        If `True`, allow the group being written into to exist already; otherwise
-        (and by default), if the group exists, an error will be raised.
+        If `True`, allow the group being written into to exist
+        already; otherwise (and by default), if the group exists, an
+        error will be raised.
     version_info_update : dict, optional
-        If present, the `version_info` field in the output JSON file will be
-        updated with this information.  Any existing version info that is not found
-        in this input will remain unchanged, but any that are in this input will be
-        either altered or added.
+        If present, the `version_info` field in the output JSON file
+        will be updated with this information.  Any existing version
+        info that is not found in this input will remain unchanged,
+        but any that are in this input will be either altered or
+        added.
+    max_phase_per_timestep : float, optional
+        Maximum phase change per time step.  If given, the approximate
+        phase change per time step is calculated when transforming to
+        the corotating frame.  If it exceeds this value, a ValueError
+        is raised.  A sensible value here is probably 10 or so — high
+        enough that random spikes from junk radiation or late ringdown
+        noise won't trigger it, but low enough that the integration
+        will still proceed reasonably quickly for anything below this
+        threshold.
 
     Returns
     -------
     w_out : WaveformModes
-        The output data, after conversion to the corotating frame, pairing of
-        opposite `m` modes, and differencing (but not shuffling).
+        The output data, after conversion to the corotating frame,
+        pairing of opposite `m` modes, and differencing (but not
+        shuffling).
     log_frame : array of quaternions
-        The actual `log_frame` data stored in the file, and used to transform to
-        the corotating frame if that was done inside this function.
-
-    Note that the returned data are *as stored in the file*.  Specifically, they
-    are presented as various types of `float` data, but have been differenced,
-    which makes them invalid as floats; you will see many NaNs and other
-    nonsensical values unless you reverse the process.
+        The actual `log_frame` data stored in the file, and used to
+        transform to the corotating frame if that was done inside this
+        function.
+
+    Note that the returned data are *as stored in the file*.
+    Specifically, they are presented as various types of `float` data,
+    but have been differenced, which makes them invalid as floats; you
+    will see many NaNs and other nonsensical values unless you reverse
+    the process.
 
     """
     if formats is None:
         formats = sxs_formats
 
     # Make sure that we can understand the file_name and create the directory
     group = None
@@ -147,19 +167,24 @@
             try:
                 initial_time = w.t[0]
                 relaxation_time = w.metadata.relaxation_time
                 max_norm_time = w.max_norm_time()
                 z_alignment_region = ((relaxation_time - initial_time) / (max_norm_time - initial_time), 0.95)
             except Exception:
                 z_alignment_region = (0.1, 0.95)
-            w, log_frame = w.to_corotating_frame(
-                tolerance=L2norm_fractional_tolerance,
-                z_alignment_region=z_alignment_region,
-                truncate_log_frame=True
-            )
+            try:
+                w, log_frame = w.to_corotating_frame(
+                    tolerance=L2norm_fractional_tolerance,
+                    z_alignment_region=z_alignment_region,
+                    truncate_log_frame=True,
+                    max_phase_per_timestep=max_phase_per_timestep
+                )
+            except ValueError as e:
+                print("\nError transforming to corotating frame:")
+                raise e
             log_frame = log_frame.ndarray[:, 1:]
         if w.frame_type != "corotating":
             raise ValueError(
                 f"Frame type of input waveform must be 'corotating' or 'inertial'; it is {w.frame_type}"
             )
 
         # Convert mode structure to conjugate pairs
@@ -301,101 +326,117 @@
         **kwargs
 ):
     """Load a waveform in RPDMB format
 
     Parameters
     ----------
     file_name : str
-        Relative or absolute path to the input HDF5 file.  If this string contains
-        but does not *end* with `'.h5'`, the remainder of the string is taken to be
-        the group within the HDF5 file in which the data is stored.  Also note that
-        a JSON file is expected in the same location, with `.h5` replaced by
-        `.json` (and the corresponding data must be stored under the `group` key if
-        relevant).
+        Relative or absolute path to the input HDF5 file.  If this
+        string contains but does not *end* with `'.h5'`, the remainder
+        of the string is taken to be the group within the HDF5 file in
+        which the data is stored.  Also note that a JSON file is
+        expected in the same location, with `.h5` replaced by `.json`
+        (and the corresponding data must be stored under the `group`
+        key if relevant).
     ignore_validation : bool or None, optional
-        Validation checks the corresponding JSON file for (1) existence, (2) number
-        of time steps, (3) H5 file size, and (4) H5 file MD5 checksum (if
-        `check_md5` is `True`).  If this key is `False`, all of this will be
-        ignored; if `True`, a `ValueError` will be raised if any of these checks
-        fails; if `None`, warnings will be issued, but the function will continue
-        as usual.
+        Validation checks the corresponding JSON file for (1)
+        existence, (2) number of time steps, (3) H5 file size, and (4)
+        H5 file MD5 checksum (if `check_md5` is `True`).  If this key
+        is `False`, all of this will be ignored; if `True`, a
+        `ValueError` will be raised if any of these checks fails; if
+        `None`, warnings will be issued, but the function will
+        continue as usual.
     check_md5 : bool, optional
         Default is `True`.  See `ignore_validation` for explanation.
     transform_to_inertial : bool, optional
-        If `True`, the output waveform is transformed to the inertial frame;
-        otherwise it is left in the frame used in the file.
+        If `True`, the output waveform is transformed to the inertial
+        frame; otherwise it is left in the frame used in the file.
     convert_from_conjugate_pairs : bool, optional
-        If `False`, the data is left in its conjugate-pair form; default is `True`.
+        If `False`, the data is left in its conjugate-pair form;
+        default is `True`.
     compression : module, optional
-        Compression module (or any other object) with `compress` and `decompress`
-        methods.  Default value is `bz2`, which is part of python's standard
-        library, and performs bzip2 de/compression.  Note that whatever this is
-        must be available to the `load` code, so this should probably be oneof the
+        Compression module (or any other object) with `compress` and
+        `decompress` methods.  Default value is `bz2`, which is part
+        of python's standard library, and performs bzip2
+        de/compression.  Note that whatever this is must be available
+        to the `load` code, so this should probably be oneof the
         built-in packages: `bz2`, `lmza`, `gzip`, or `zlib`.
     diff : function, optional
-        Function to compare successive values.  Defaults to `diff`, which is the
-        floating-point difference.  Other possibilities include `diffInt` (which
-        reinterprets the data as integers before taking the difference) and `xor`
-        (which is the previous default); neither works as well with our data at the
-        time of this writing.
+        Function to compare successive values.  Defaults to `diff`,
+        which is the floating-point difference.  Other possibilities
+        include `diffInt` (which reinterprets the data as integers
+        before taking the difference) and `xor` (which is the previous
+        default); neither works as well with our data at the time of
+        this writing.
     formats : array[str], optional
-        Possible names of the format.  Defaults to variations on `RPDMB`.
+        Possible names of the format.  Defaults to variations on
+        `RPDMB`.
 
     Keyword parameters
     ------------------
     data_type : str, optional
-        Describes the type of data — such as "h" or "psi4".  Default is "unknown".
+        Describes the type of data — such as "h" or "psi4".  Default
+        is "unknown".
     m_is_scaled_out : bool, optional
         Default is True
     r_is_scaled_out : bool, optional
         Default is True
     spin_weight : int, optional
         Default is `None`.
-
-    Note that the keyword parameters will be overridden by corresponding entries in
-    the JSON file, if they exist.  If the JSON file does not exist, any keyword
-    parameters not listed above will be passed through as the `json_data` field of
-    the returned waveform.
+    drop_times_before : {float,"begin","reference","merger"}, optional
+        If given, all times before the given time will be dropped.  If
+        a string is given, the corresponding time will be used.  The
+        "begin" option represents the earliest time in the data, so no
+        data will be dropped; "reference" is the `reference_time`
+        reported in the metadata.  If `None`, the default, t=0 will be
+        used if present in the data, and the first time step
+        otherwise.
+
+    Note that the keyword parameters will be overridden by
+    corresponding entries in the JSON file, if they exist.  If the
+    JSON file does not exist, any keyword parameters not listed above
+    will be passed through as the `json_data` field of the returned
+    waveform.
 
     """
     if formats is None:
         formats = sxs_formats
 
     def invalid(message):
         if ignore_validation:
             pass
         elif ignore_validation is None:
             warnings.warn(message)
         else:
             raise ValueError(message)
 
     file_name_str = str(file_name)
-    group = None
+    group = kwargs.get("group", None)
     if ".h5" in file_name_str and not file_name_str.endswith(".h5"):
         file_name_str, group = file_name_str.split(".h5")
     if group == "/":
         group = None
 
     # At this point, file_name_str may or may not have an h5 suffix
     # (because the user may have passed in a file without the suffix,
     # or because there was an .h5 in the middle of the filename.)
     # But that's ok, we will use with_suffix below.
 
-
     # In a common use case, the h5 and json files will be named
     # bla.h5 and bla.json as expected, but they will be git-annex symlinks.
     # This means that the files pointed to will have strange names, like:
     # bla.h5   -> /some/crazy/path/some_crazy_hash.h5
     # bla.json -> /some/different/crazy/path/a_different_crazy_hash.json
     # where the paths are determined by git-annex and the hashes are basically
     # SHA256 hashes of the contents.
     #
     # This means we need to change the suffix *before* the resolve() call.
     h5_path = pathlib.Path(file_name_str).with_suffix(".h5").expanduser().resolve()
     json_path = pathlib.Path(file_name_str).with_suffix(".json").expanduser().resolve()
+    metadata_path = (pathlib.Path(file_name_str).parent / "metadata.json").expanduser().resolve()
 
     # This will be used for validation
     h5_size = h5_path.stat().st_size
 
     data_type = kwargs.pop("data_type", "unknown")
     m_is_scaled_out = kwargs.pop("m_is_scaled_out", True)
     r_is_scaled_out = kwargs.pop("r_is_scaled_out", True)
@@ -495,15 +536,15 @@
     data = np.empty((n_times, n_modes), dtype=complex)
 
     # Un-diff the data
     xor(t, reverse=True, preserve_dtype=True, out=t)
     diff(data_tmp, reverse=True, axis=0, out=data)
     diff(log_frame, reverse=True, preserve_dtype=True, axis=0, out=log_frame)
 
-    frame = np.exp(quaternionic.array(np.insert(log_frame, 0, 0.0, axis=1)))
+    frame = np.exp(quaternionic.array.from_vector_part(log_frame))
 
     if spin_weight is None:
         warning = f"Spin weight has not been provided for {h5_path}.  This may result in errors with some functions."
         warnings.warn(warning)
 
     w = WaveformModes(
         data.view(np.complex128),
@@ -522,16 +563,42 @@
 
     if convert_from_conjugate_pairs:
         w.convert_from_conjugate_pairs()
 
     if transform_to_inertial:
         w = w.to_inertial_frame()
 
+    if not metadata_path.exists():
+        invalid(f'\nMetadata file "{metadata_path}" cannot be found, but is expected for this data format.')
+        metadata = None
+    else:
+        metadata = Metadata.from_file(metadata_path)
+
+    dtb = kwargs.pop("drop_times_before", 0)
+    if dtb=="begin":
+        i0 = 0
+    elif dtb==0:
+        i0 = np.argmin(w.t < 0)
+    elif dtb=="reference":
+        if metadata is None:
+            raise ValueError(f"Metadata is required if `drop_times_before` is set to 'reference'")
+        i0 = np.argmin(w.t < metadata.reference_time)
+    elif isinstance(dtb, numbers.Real):
+        i0 = np.argmin(w.t < dtb)
+    elif dtb=="merger":
+        i0 = w.max_norm_index()
+    else:
+        raise ValueError(f"Invalid value for `drop_times_before`: {dtb}")
+    if i0 != 0:
+        w = w[i0:]
+
     w.json_data = json_data
     w.log_frame = log_frame
+    if metadata is not None:
+        w.metadata = metadata
 
     return w
 
 
 def load_time(
         file_name, ignore_validation=None, check_md5=True,
         transform_to_inertial=True, convert_from_conjugate_pairs=True,
```

### Comparing `sxs-2022.5.6/sxs/waveforms/rotating_paired_xor_multishuffle_bzip2.py` & `sxs-2023.0.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import json
 import numpy as np
 import scipy
 import h5py
 import quaternionic
 import spherical
 
-from . import WaveformModes
+from .. import WaveformModes
 from . import rotating_paired_diff_multishuffle_bzip2 as rpdmb
-from .. import __version__
-from ..utilities import default_shuffle_widths, md5checksum, xor, multishuffle, version_info
+from ... import __version__
+from ...utilities import default_shuffle_widths, md5checksum, xor, multishuffle, version_info
 
 
 sxs_formats = ["rotating_paired_xor_multishuffle_bzip2", "rpxmb", "rpxm", "RPXMB", "RPXM"]
 
 
 def save(w, file_name=None, file_write_mode="w", L2norm_fractional_tolerance=1e-10, log_frame=None, shuffle_widths=default_shuffle_widths):
     """Save a waveform in RPXMB format
```

### Comparing `sxs-2022.5.6/sxs/waveforms/transformations.py` & `sxs-2023.0.0/sxs/waveforms/transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/waveforms/waveform_mixin.py` & `sxs-2023.0.0/sxs/waveforms/waveform_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import abc
 import numpy as np
 import quaternionic
 
 
 class WaveformMixin(abc.ABC):
-    # Note: This is currently a pretty trivial class, but as the code develops
-    # this will be increasingly useful.
-
     @property
     @abc.abstractmethod
     def data(self):  # Handy alias for backwards compatibility
         return self.ndarray
 
     @property
     @abc.abstractmethod
```

### Comparing `sxs-2022.5.6/sxs/waveforms/waveform_modes.py` & `sxs-2023.0.0/sxs/waveforms/waveform_modes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """The main container for waveform objects with mode weights"""
 
 import re
+import numbers
+from collections.abc import MutableMapping
 import numpy as np
+from scipy.interpolate import CubicSpline
+from scipy.optimize import minimize_scalar
 import quaternionic
 import spherical
 from .. import TimeSeries
 from . import WaveformMixin
 from .mode_utilities import _expectation_value_LL, _expectation_value_Ldt
 
 NRAR_mode_regex = re.compile(r"""Y_l(?P<L>[0-9]+)_m(?P<M>[-+0-9]+)\.dat""")
@@ -82,16 +86,14 @@
 
     This code is identical to the equivalent code using `h5py` except that the call
     to `h5py.File` is replaced with the call to `sxs.loadcontext`.  The `.dat`
     datasets are reconstructed on the fly, but should be bitwise-identical to the
     output from the HDF5 file whenever the underlying format is NRAR.
 
     """
-    import functools
-
     def __new__(cls, input_array, *args, **kwargs):
         for requirement in ["modes_axis", "ell_min", "ell_max"]:
             if requirement not in kwargs and requirement not in getattr(input_array, "_metadata", {}):
                 raise ValueError(f"{cls} could not find required argument '{requirement}'")
         self = super().__new__(cls, input_array, *args, **kwargs)
         return self
 
@@ -115,14 +117,39 @@
             return np.hstack((self.time[:, np.newaxis], data))
         obj, time_key = self._slice(key)
         if time_key is None:
             raise ValueError(f"Fancy indexing (with {key}) is not supported")
         obj = obj.view(type(self))
         if "frame" in obj._metadata and obj.frame.shape == (self.n_times, 4):
             obj._metadata["frame"] = obj.frame[time_key, :]
+        if (
+            obj.ndim != self.ndim
+            or obj.shape[obj.modes_axis] != self.shape[self.modes_axis]
+        ):
+            clean_LM_slice = False
+            # Check if the new shape is compatible with specific ell_min and ell_max values
+            if (
+                isinstance(key, tuple)
+                and len(key) > self.modes_axis
+                and isinstance(key[self.modes_axis], slice)
+            ):
+                sl = key[1]
+                if sl.step is None or sl.step==1:
+                    ell1, m1 = self.LM[sl.start or 0]  # in case sl.start is None
+                    ell2, m2 = self.LM[sl.stop-1]
+                    if ell1 <= ell2 and m1 == -ell1 and m2 == ell2:
+                        # The sliced object has valid ell_min and ell_max values,
+                        # so we can interpret it as a WaveformModes object; we
+                        # just need to correct those values
+                        clean_LM_slice = True
+                        obj._metadata["ell_min"] = ell1
+                        obj._metadata["ell_max"] = ell2
+            if not clean_LM_slice:
+                # If not, don't represent this as a WaveformModes object; it's just a TimeSeries
+                obj = TimeSeries(obj)
         return obj
 
     @property
     def modes_axis(self):
         """Axis of the array storing the various modes
 
         See the documentation of this class for an explanation of what this means.
@@ -427,21 +454,41 @@
         """
         if skip_fraction_of_data <= 1:
             return np.argmax(self.norm)
         else:
             i = int(self.n_times // skip_fraction_of_data)
             return np.argmax(self[i:].norm) + i
 
-    def max_norm_time(self, skip_fraction_of_data=4):
+    def max_norm_time(self, skip_fraction_of_data=4, interpolate=False):
         """Return time at which largest norm occurs in data
 
-        See `help(max_norm_index)` for explanation of the optional argument.
+        See `help(max_norm_index)` for explanation of
+        `skip_fraction_of_data`.
 
-        """
-        return self.t[self.max_norm_index(skip_fraction_of_data=skip_fraction_of_data)]
+        If `interpolate` is True, the time is interpolated to a higher
+        precision than the time step of the data.  This is done by
+        fitting a cubic spline to the norm of the data and finding the
+        time at which the norm is maximized.
+
+        """
+        if interpolate:
+            i_max = self.max_norm_index(skip_fraction_of_data)
+
+            # Find a range of indices that includes the discrete time with
+            # largest norm, plus 10 points in either direction, to ensure that
+            # the spline has enough data to interpolate the whole range.
+            idx_min = max(0, i_max - 10)
+            idx_max = min(self.n_times, i_max + 10)
+            idx = slice(idx_min, idx_max)
+
+            # Minimize -norm over the range of indices
+            spline = CubicSpline(self.t[idx], -self[idx, :].norm)
+            return minimize_scalar(spline, bounds=(self.t[idx_min], self.t[idx_max]), method='bounded').x
+        else:
+            return self.t[self.max_norm_index(skip_fraction_of_data)]
 
     def interpolate(self, new_time, derivative_order=0, out=None):
         """Interpolate this object to a new set of times
 
         Note that if this object has "frame" data and the derivative order is nonzero,
         it is not entirely clear what is desired.  In those cases, the frame is just
         interpolated to the new times, but no derivative or antiderivative is taken.
@@ -474,15 +521,15 @@
             Property calling `self.antiderivative(1)`.
         iint :
             Property calling `self.antiderivative(2)`.
 
         """
         result = TimeSeries.interpolate(self, new_time, derivative_order=derivative_order, out=out)
         if self.frame.shape == (self.n_times, 4) and not np.array_equal(self.time, result.time):
-            self._metadata["frame"] = quaternionic.squad(self.frame, self.time, result.time)
+            result._metadata["frame"] = quaternionic.squad(self.frame, self.time, result.time)
         return result
 
     def truncate(self, tol=1e-10):
         """Truncate the precision of this object's data in place
 
         This function sets bits in the data to 0 when they have lower significance than
         will alter the norm of the Waveform by a fraction `tol` at that instant in
@@ -753,25 +800,25 @@
         """
         if rough_direction is None:
             rough_direction = np.array([0, 0, 1.])
 
         # Calculate the LL matrix at each instant
         LL = self.expectation_value_LL
 
-        # This is the eigensystem
-        eigenvals, eigenvecs = np.linalg.eigh(LL)
+        # Compute the eigensystem
+        _, eigenvecs = np.linalg.eigh(LL)
 
-        # `eigh` always returns eigenvals in *increasing* order, so element `2` will be
-        # the dominant principal axis
-        dpa = quaternionic.array.from_vector_part(eigenvecs[..., 2])
+        # Choose the dominant principal axis `dpa`
+        # `eigh` always returns eigenvalues in *increasing* order, so we want the last
+        dpa = quaternionic.array.from_vector_part(eigenvecs[..., -1])
 
         # Make the direction vectors continuous
         dpa = quaternionic.unflip_rotors(dpa, inplace=True).vector
 
-        # Now, just make sure that the result if more parallel than anti-parallel to
+        # Now, just make sure that the result is more parallel than anti-parallel to
         # the `rough_direction`
         if np.dot(dpa[rough_direction_index], rough_direction) < 0:
             dpa *= -1
 
         return dpa
 
     @property
@@ -937,23 +984,30 @@
         new_metadata.pop("frame", None)
         return type(self)(rotated_mode_weights, **new_metadata)
 
     def to_inertial_frame(self):
         """Return a copy of this waveform in the inertial frame"""
         if "frame" not in self._metadata:
             raise ValueError("This waveform has no frame information")
-        if self.frame.shape[0] == 1:
+        if self.frame.shape[0] == 1 and self.n_times > 1:
             raise ValueError("This waveform appears to already be in an inertial frame")
         if self.frame.shape != (self.n_times, 4):
             raise ValueError(f"Frame shape {self.frame.shape} not understood; expected {(self.n_times, 4)}")
         w = self.rotate(~self.frame)
         w._metadata["frame_type"] = "inertial"
         return w
 
-    def corotating_frame(self, R0=quaternionic.one, tolerance=1e-12, z_alignment_region=None, return_omega=False):
+    def corotating_frame(
+            self,
+            R0=quaternionic.one,
+            tolerance=1e-12,
+            z_alignment_region=None,
+            return_omega=False,
+            max_phase_per_timestep=None
+        ):
         """Return rotor taking current mode frame into corotating frame
 
         Parameters
         ----------
         R0 : quaternionic, optional
             Value of the output rotation at the first output instant; defaults to 1
         tolerance : float, optional
@@ -965,14 +1019,18 @@
             begin and end the average.  For example, (0.1, 0.9) would lead to starting
             10% of the time from the first time step to the max norm time, and ending
             at 90% of that time.
         return_omega: bool, optional
             If True, return a 2-tuple consisting of the frame (the usual returned
             object) and the angular-velocity data.  That is frequently also needed, so
             this is just a more efficient way of getting the data.  Default is `False`.
+        max_phase_per_timestep : float, optional
+            Maximum phase change per time step.  If given, the approximate phase change
+            per time step is calculated, and if it exceeds this value, a ValueError is
+            raised.
 
         Notes
         -----
         Essentially, this function evaluates the angular velocity of the waveform, and
         then integrates it to find the corotating frame itself.  This frame is defined
         to be the frame in which the time-dependence of the waveform is minimized — at
         least, to the extent possible with a time-dependent rotation.
@@ -981,14 +1039,26 @@
         specified as the optional `R0` argument to this function.  If it is not
         specified, the z axis of the rotating frame is aligned with the
         `dominant_eigenvector_LL`, and chosen to be more parallel than anti-parallel to
         the angular velocity.
 
         """
         ω = self.angular_velocity
+        if max_phase_per_timestep is not None:
+            dt = np.diff(self.t)
+            dt = np.append(dt, dt[-1])
+            dθ = np.linalg.norm(ω, axis=1) * dt
+            if np.max(dθ) > max_phase_per_timestep:
+                index = np.argmax(dθ)
+                t = self.t[index]
+                raise ValueError(
+                    f"\nMaximum phase change per time step exceeded: "
+                    f"{max(dθ)=:.2g} > {max_phase_per_timestep} at {index=} ({t=:.2f}).\n"
+                    f"This probably means that there is something very wrong in your data."
+                )
         R = quaternionic.array.from_angular_velocity(ω, self.t, R0=R0, tolerance=tolerance)
         if z_alignment_region is None:
             correction_rotor = quaternionic.one
         else:
             initial_time = self.t[0]
             inspiral_time = self.max_norm_time() - initial_time
             t1 = initial_time + z_alignment_region[0] * inspiral_time
@@ -1003,16 +1073,22 @@
         R = (R * correction_rotor).normalized
         if return_omega:
             return (R, ω)
         else:
             return R
 
     def to_corotating_frame(
-        self, R0=None, tolerance=1e-12, z_alignment_region=None, return_omega=False, truncate_log_frame=False
-    ):
+            self,
+            R0=None,
+            tolerance=1e-12,
+            z_alignment_region=None,
+            return_omega=False,
+            truncate_log_frame=False,
+            max_phase_per_timestep=None
+        ):
         """Return a copy of this waveform in the corotating frame
 
         The corotating frame is defined to be a rotating frame for which the (L² norm
         of the) time-dependence of the modes expressed in that frame is minimized.
         This leaves the frame determined only up to an overall rotation.  In this 
 
         Parameters
@@ -1034,18 +1110,26 @@
             frame (the usual returned object) and the angular-velocity data.  That is
             frequently also needed, so this is just a more efficient way of getting the
             data.
         truncate_log_frame : bool, optional
             If True, set bits of log(frame) with lower significance than `tolerance` to
             zero, and use exp(truncated(log(frame))) to rotate the waveform.  Also
             returns `log_frame` along with the waveform (and optionally `omega`)
+        max_phase_per_timestep : float, optional
+            Maximum phase change per time step.  If given, the approximate phase change
+            per time step is calculated, and if it exceeds this value, a ValueError is
+            raised.
 
         """
         frame, omega = self.corotating_frame(
-            R0=R0, tolerance=tolerance, z_alignment_region=z_alignment_region, return_omega=True
+            R0=R0,
+            tolerance=tolerance,
+            z_alignment_region=z_alignment_region,
+            return_omega=True,
+            max_phase_per_timestep=max_phase_per_timestep
         )
         if truncate_log_frame:
             log_frame = np.log(frame)
             TimeSeries.truncate(log_frame, tolerance)
             frame = np.exp(quaternionic.array(log_frame))
         w = self.rotate(frame)
         w._metadata["frame_type"] = "corotating"
@@ -1056,7 +1140,120 @@
             else:
                 return (w, omega)
         else:
             if truncate_log_frame:
                 return (w, log_frame)
             else:
                 return w
+
+    def coprecessing_frame(self, rough_direction=None, rough_direction_index=0):
+        """Return the coprecessing frame of the waveform
+
+        This function returns the minimally rotating coprecessing frame of the
+        waveform, as a `quaternionic.array`.  Specifically, the result rotates
+        the static $(x,y,z)$ frame onto a frame in which the dominant eigenvector
+        of the matrix expectation value ⟨w|LᵃLᵇ|w⟩ is aligned with the $z'$ axis.
+        Furthermore, to fix the rotation *about* the $z'$ axis, the minimal-
+        rotation condition is enforced.
+        
+        The coprecessing frame and the minimal-rotation condition are defined
+        in https://arxiv.org/abs/1110.2965.
+
+        For details about the arguments, see the docstring for the
+        `dominant_eigenvector_LL` method.
+
+        """
+        cpa = quaternionic.array.from_vector_part(
+            self.dominant_eigenvector_LL(rough_direction, rough_direction_index)
+        )
+        R = np.sqrt(-cpa * quaternionic.z)  # R * z * R.conj() ≈ cpa
+        return R.to_minimal_rotation(self.t)
+
+    def to_coprecessing_frame(self, rough_direction=None, rough_direction_index=0):
+        """Transform this waveform to the coprecessing frame
+
+        The coprecessing frame is defined to be a rotating frame for which the
+        dominant eigenvector of the matrix expectation value ⟨w|LᵃLᵇ|w⟩ is aligned
+        with the $z'$ axis, and the minimal-rotation condition is enforced.  This
+        leaves the frame completely determined, except for a single rotation about
+        the $z'$ axis.
+
+        The coprecessing frame and the minimal-rotation condition are defined in
+        https://arxiv.org/abs/1110.2965.
+
+        For details about the arguments, see the docstring for the
+        `dominant_eigenvector_LL` method.
+
+        """
+        frame = self.coprecessing_frame(rough_direction, rough_direction_index)
+        w = self.rotate(frame)
+        w._metadata["frame_type"] = "coprecessing"
+        w._metadata["frame"] = frame
+        return w
+
+
+class WaveformModesDict(MutableMapping, WaveformModes):
+    """A dictionary-like class for storing waveform modes
+
+    This class is a subclass of `MutableMapping`, which is essentially
+    a `dict`.  The only difference is that this class silently passes
+    `__delitem__`, and disables adding keys that aren't within the
+    valid `ell` range or don't have valid `m` values.  Otherwise, it
+    behaves exactly like a dictionary, including the various methods
+    of iteration, and being able to update values.
+    
+    This class is also a subclass of `WaveformModes`, except with
+    dictionary-like access to the modes.  Specifically, indexing like
+    `h[2,1]` will return the mode with `(ell,m) = (2,1)` as a function
+    of time.  The input index is checked to ensure that it is a tuple
+    containing exactly two integers; all other indexing is passed
+    through to the superclass.
+
+    This subclass is necessary because the `WaveformModes` class would
+    consider an index like `h[2,1]` to indicate the second time step
+    and the first mode, rather than the mode with `(ell,m) = (2,1)`,
+    which is preferred by some users.
+    """
+    def __getitem__(self, key):
+        if (
+            isinstance(key, (tuple, list))
+            and len(key) == 2
+            and isinstance(key[0], numbers.Integral)
+            and isinstance(key[1], numbers.Integral)
+        ):
+            ell, m = key
+            if abs(m) > ell:
+                raise KeyError(f"Mode index {(ell,m)=} is not valid")
+            if not self.ell_min <= ell <= self.ell_max:
+                raise KeyError(
+                    f"Mode {ell=} is out of range for this waveform's "
+                    f"ell values {[self.ell_min, self.ell_max]}"
+                )
+            return np.take(self.ndarray, self.index(ell, m), axis=self.modes_axis)
+            # return self.ndarray[:, self.index(ell, m)]
+            # return super().__getitem__((slice(None), self.index(ell, m))).ndarray
+        else:
+            return super().__getitem__(key)
+    def __setitem__(self, key, value):
+        if (
+            isinstance(key, tuple)
+            and len(key) == 2
+            and isinstance(key[0], numbers.Integral)
+            and isinstance(key[1], numbers.Integral)
+        ):
+            ell, m = key
+            if abs(m) > ell:
+                raise KeyError(f"Mode index {(ell,m)=} is not valid")
+            if not self.ell_min <= ell <= self.ell_max:
+                raise KeyError(
+                    f"Mode {ell=} is out of range for this waveform's "
+                    f"ell values {[self.ell_min, self.ell_max]}"
+                )
+            self.ndarray[:, self.index(ell, m)] = value
+        else:
+            return super().__setitem__(key, value)
+    def __delitem__(self, key):
+        pass
+    def __iter__(self):
+        return map(tuple, self.LM)
+    def __len__(self):
+        return self.LM.__len__()
```

### Comparing `sxs-2022.5.6/sxs/zenodo/__init__.py` & `sxs-2023.0.0/sxs/zenodo/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/catalog.py` & `sxs-2023.0.0/sxs/zenodo/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/creators.py` & `sxs-2023.0.0/sxs/zenodo/creators.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/simannex.py` & `sxs-2023.0.0/sxs/zenodo/simannex.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/surrogatemodeling.py` & `sxs-2023.0.0/sxs/zenodo/surrogatemodeling.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/api/deposit.py` & `sxs-2023.0.0/sxs/zenodo/api/deposit.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,16 +569,17 @@
         as for a new deposit.
 
         Only one unpublished new version deposit can be available at any moment, i.e.: calling new
         version action multiple times will have no effect, as long as the resulting new version
         deposit from the first call is not published or deleted.
 
         """
-        self.register_new_version(refresh_information=refresh_information)
-        return self.login.deposit(self.id_latest_draft, ignore_deletion=ignore_deletion)
+        r = self.register_new_version(refresh_information=refresh_information)
+        id_latest_draft = r.json()['links']['latest_draft'].split('/')[-1]
+        return self.login.deposit(id_latest_draft, ignore_deletion=ignore_deletion)
         
     def register_new_version(self, refresh_information=True):
         """Create a new version of a deposit.
 
         To publish the new version, its files must differ from all previous versions.
 
         This action will create a new deposit, which will be a snapshot of the current resouce,
@@ -683,15 +684,15 @@
                 if md5checksum(path) == file_checksums[name]:
                     print('File {0} has already been uploaded.  Skipping this upload.'.format(name))
                     return None
         if name in self.file_ids:
             self.delete_file(name, refresh_information=False)
         url = '{0}/{1}'.format(self.links['bucket'], name)
         r = self._put(url, data=open(path, 'rb'), headers={"Content-Type": "application/octet-stream"})
-        if r.status_code != 200:
+        if r.status_code != 201:
             print('Uploading {0} to deposit {1} failed.'.format(path, self.deposition_id))
             print('Upload url was {0}.'.format(url))
             if r.status_code == 400:
                 if os.stat(path).st_size == 0:
                     print('This file has size zero, which leads to an error response.')
             try:
                 print(r.json())
@@ -707,15 +708,15 @@
         import json
         file_ids = self.file_ids
         if old_file_name not in file_ids:
             print('File name "{0}" not found on Zenodo.'.format(old_file_name))
             raise ValueError(old_file_name)
         file_id = file_ids[old_file_name]
         url = '{0}api/deposit/depositions/{1}/files/{2}'.format(self.base_url, self.id, file_id)
-        rename_data = {'filename': new_file_name}
+        rename_data = {'name': new_file_name}
         r = self._put(url, data=json.dumps(rename_data))
         if r.status_code != 200:
             print('Renaming file "{0}" to "{1}" in deposit "{2}" failed.'.format(old_file_name, new_file_name, self.id))
             if r.status_code == 403:
                 print('Server replied with "Forbidden: Renaming an already published deposition file."')
                 print('Try get_new_version, and then delete the file from that version.')
             if r.status_code == 404:
```

### Comparing `sxs-2022.5.6/sxs/zenodo/api/login.py` & `sxs-2023.0.0/sxs/zenodo/api/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/sxs/zenodo/api/records.py` & `sxs-2023.0.0/sxs/zenodo/api/records.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/conftest.py` & `sxs-2023.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_catalog.py` & `sxs-2023.0.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_horizons.py` & `sxs-2023.0.0/tests/test_horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_loader.py` & `sxs-2023.0.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_metadata.py` & `sxs-2023.0.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_time_series.py` & `sxs-2023.0.0/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_transformations.py` & `sxs-2023.0.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_waveform_rotations.py` & `sxs-2023.0.0/tests/test_waveform_rotations.py`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/tests/test_waveforms.py` & `sxs-2023.0.0/tests/test_waveforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     for L2norm_fractional_tolerance in [1e-6, 1e-10, 1e-14]:
         print(f"# Tolerance {L2norm_fractional_tolerance}")
         with tempfile.TemporaryDirectory() as temp_dir:
             file_name = pathlib.Path(temp_dir) / "Strain_N4"
             h5_file_name = file_name.with_suffix(".h5")
             sxs.rpxmb.save(w, file_name, L2norm_fractional_tolerance=L2norm_fractional_tolerance)
             print(f"File size = {h5_file_name.stat().st_size:_}B")
-            w2 = sxs.rpxmb.load(file_name)
+            w2 = sxs.rpxmb.load(file_name, drop_times_before="begin")
         diff_norm = np.linalg.norm(w.data-w2.data, axis=w.modes_axis)
         print(f"Max difference = {np.max(diff_norm)}")
         assert np.max(diff_norm) < L2norm_fractional_tolerance, (np.max(diff_norm), "\n", diff_norm)
 
 
 def test_rpdmb():
     print()
@@ -277,25 +277,25 @@
         print(f"# Tolerance {L2norm_fractional_tolerance}")
         with tempfile.TemporaryDirectory() as temp_dir:
             file_name = pathlib.Path(temp_dir) / "Strain_N4"
             h5_file_name = file_name.with_suffix(".h5")
             sxs.rpdmb.save(w, file_name, L2norm_fractional_tolerance=L2norm_fractional_tolerance)
             file_size = h5_file_name.stat().st_size
             print(f"RPDMB File size = {file_size:_}B")
-            w2 = sxs.rpdmb.load(file_name)
+            w2 = sxs.rpdmb.load(file_name, drop_times_before="begin")
 
             file_name2 = pathlib.Path(temp_dir) / "Strain2_N4"
             h5_file_name2 = file_name2.with_suffix(".h5")
             sxs.rpxmb.save(
                 w, file_name2, L2norm_fractional_tolerance=L2norm_fractional_tolerance,
                 shuffle_widths=sxs.utilities.default_shuffle_widths_old
             )
             file_size2 = h5_file_name2.stat().st_size
             print(f"RPXMB File size = {file_size2:_}B")
-            w3 = sxs.rpxmb.load(file_name2)
+            w3 = sxs.rpxmb.load(file_name2, drop_times_before="begin")
 
             print(f"RPXMB/RPDMB file size = {file_size2/file_size}")
 
         diff_norm = np.linalg.norm(w.data-w2.data, axis=w.modes_axis)
         diff_norm2 = np.linalg.norm(w2.data-w3.data, axis=w.modes_axis)
         print(f"Max RPDMB difference = {np.max(diff_norm)}")
         print(f"Max RPDMB-RPXMB difference = {np.max(diff_norm2)}")
```

### Comparing `sxs-2022.5.6/.gitignore` & `sxs-2023.0.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -114,7 +114,9 @@
 .envrc
 
 # conda smithy ci-skeleton start
 *.pyc
 
 build_artifacts
 # conda smithy ci-skeleton end
+
+.vscode
```

### Comparing `sxs-2022.5.6/LICENSE` & `sxs-2023.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/README.md` & `sxs-2023.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sxs-2022.5.6/pyproject.toml` & `sxs-2023.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 build = "mkdocs build --clean"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 # This is just a workaround; see https://github.com/danielfrg/mkdocs-jupyter/issues/154
 [tool.hatch.envs.docs.env-vars]
 JUPYTER_PLATFORM_DIRS = "1"
 
+[tool.hatch.envs.notes]
+dependencies = [
+  "ipython",
+  "matplotlib"
+]
+
 
 [tool.black]
 line-length = 120
 target-version = ["py38"]
 
 
 [tool.pytest.ini_options]
```

### Comparing `sxs-2022.5.6/PKG-INFO` & `sxs-2023.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sxs
-Version: 2022.5.6
+Version: 2023.0.0
 Summary: Interface to data produced by the Simulating eXtreme Spacetimes collaboration
 Project-URL: Homepage, https://github.com/sxs-collaboration/sxs
 Project-URL: Documentation, https://sxs.readthedocs.io/
 Author-email: Michael Boyle <michael.oliver.boyle@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Michael Boyle
```

