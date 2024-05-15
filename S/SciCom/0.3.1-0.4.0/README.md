# Comparing `tmp/scicom-0.3.1.tar.gz` & `tmp/scicom-0.4.0.tar.gz`

## Comparing `scicom-0.3.1.tar` & `scicom-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,124 @@
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.3.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scicom-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 scicom-0.3.1/tox.ini
--rw-r--r--   0        0        0   822615 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/HistoricalLetters.png
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/authors.rst
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/conf.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/index.rst
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/license.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/make.bat
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/readme.rst
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/requirements.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/usingmesa.rst
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/_static/bmbf.png
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/_static/logo.png
--rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.3.1/docs/_static/mpiwg.png
--rw-r--r--   0        0        0   189800 2020-02-02 00:00:00.000000 scicom-0.3.1/examples/RunModel.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/__init__.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/interface.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/run.py
--rw-r--r--   0        0        0   389859 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson
--rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/data/pone.0162678.s003.csv
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/data/relPop_plosOne.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/__init__.py
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/agents.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/interface.py
--rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/model.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/server.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/space.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/historicalletters/utils.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/SimpleContinuousModule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/__init__.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/agents.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/interface.py
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/model.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/server.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/simple_continuous_canvas.js
--rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/knowledgespread/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/utilities/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 scicom-0.3.1/src/scicom/utilities/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/.gitignore
--rw-r--r--   0        0        0    19095 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/class_index.html
--rw-r--r--   0        0        0    23058 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/coverage_html.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/favicon_32.png
--rw-r--r--   0        0        0    55562 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/function_index.html
--rw-r--r--   0        0        0    10911 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/keybd_open.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/style.css
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_SimpleContinuousModule_py.html
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79___init___py.html
--rw-r--r--   0        0        0    52034 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_agents_py.html
--rw-r--r--   0        0        0    20652 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_app_py.html
--rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_interface_py.html
--rw-r--r--   0        0        0    53577 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_model_py.html
--rw-r--r--   0        0        0    60439 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_server_py.html
--rw-r--r--   0        0        0    80920 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_utils_py.html
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_22d2582a602e487e___init___py.html
--rw-r--r--   0        0        0    55925 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_22d2582a602e487e_statistics_py.html
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21___init___py.html
--rw-r--r--   0        0        0    82015 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_agents_py.html
--rw-r--r--   0        0        0    40709 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_interface_py.html
--rw-r--r--   0        0        0    85990 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_model_py.html
--rw-r--r--   0        0        0    27174 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_server_py.html
--rw-r--r--   0        0        0    20755 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_space_py.html
--rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_utils_py.html
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3___init___py.html
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3_interface_py.html
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3_run_py.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/historicalletters/__init__.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/historicalletters/test_model.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/historicalletters/test_server.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/historicalletters/test_space.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 scicom-0.3.1/tests/scicom/historicalletters/test_utils.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 scicom-0.3.1/.gitignore
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.3.1/AUTHORS.rst
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 scicom-0.3.1/README.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 scicom-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 scicom-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scicom-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.4.0/MANIFEST.in
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 scicom-0.4.0/tox.ini
+-rw-r--r--   0        0        0   822615 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/HistoricalLetters.png
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/authors.rst
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/license.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/readme.rst
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/usingmesa.rst
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/_static/bmbf.png
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/_static/logo.png
+-rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.4.0/docs/_static/mpiwg.png
+-rw-r--r--   0        0        0   189800 2020-02-02 00:00:00.000000 scicom-0.4.0/examples/RunModel.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/__init__.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/interface.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/run.py
+-rw-r--r--   0        0        0   389859 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson
+-rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/data/pone.0162678.s003.csv
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/data/relPop_plosOne.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/__init__.py
+-rw-r--r--   0        0        0    11634 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/agents.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/interface.py
+-rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/model.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/server.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/space.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/historicalletters/utils.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/SimpleContinuousModule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/__init__.py
+-rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/agents.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/interface.py
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/model.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/server.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/simple_continuous_canvas.js
+-rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/knowledgespread/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/utilities/__init__.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 scicom-0.4.0/src/scicom/utilities/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/coverage_html.js
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_02d42bec932dca30___init___py.html
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_02d42bec932dca30_run_py.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe___init___py.html
+-rw-r--r--   0        0        0    81276 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_agents_py.html
+-rw-r--r--   0        0        0    78861 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_model_py.html
+-rw-r--r--   0        0        0    26866 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_server_py.html
+-rw-r--r--   0        0        0    19668 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_space_py.html
+-rw-r--r--   0        0        0    30811 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_utils_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_6392e7e021769227___init___py.html
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_6392e7e021769227_test_model_py.html
+-rw-r--r--   0        0        0    24612 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_6392e7e021769227_test_utils_py.html
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095___init___py.html
+-rw-r--r--   0        0        0    43401 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095_agents_py.html
+-rw-r--r--   0        0        0    27864 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095_model_py.html
+-rw-r--r--   0        0        0    34577 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095_server_py.html
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e1dbc2383e9dc8ec___init___py.html
+-rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e1dbc2383e9dc8ec_statistics_py.html
+-rw-r--r--   0        0        0    14624 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3___init___py.html
+-rw-r--r--   0        0        0    52169 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_agents_py.html
+-rw-r--r--   0        0        0    20584 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_app_py.html
+-rw-r--r--   0        0        0    53509 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_model_py.html
+-rw-r--r--   0        0        0    60784 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_server_py.html
+-rw-r--r--   0        0        0    80723 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/favicon_32.png
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/keybd_open.png
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/coverage-html/style.css
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/coverage_html.js
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589___init___py.html
+-rw-r--r--   0        0        0    83693 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_agents_py.html
+-rw-r--r--   0        0        0    40711 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_interface_py.html
+-rw-r--r--   0        0        0    90092 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_model_py.html
+-rw-r--r--   0        0        0    27176 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_server_py.html
+-rw-r--r--   0        0        0    20757 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_space_py.html
+-rw-r--r--   0        0        0    33530 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_277402163e1a7589_utils_py.html
+-rw-r--r--   0        0        0    15089 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228___init___py.html
+-rw-r--r--   0        0        0    52036 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_agents_py.html
+-rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_app_py.html
+-rw-r--r--   0        0        0    19411 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_interface_py.html
+-rw-r--r--   0        0        0    53579 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_model_py.html
+-rw-r--r--   0        0        0    60441 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_server_py.html
+-rw-r--r--   0        0        0    80922 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_utils_py.html
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_3142edd200b00bad___init___py.html
+-rw-r--r--   0        0        0    49663 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_3142edd200b00bad_prune_py.html
+-rw-r--r--   0        0        0   105137 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_3142edd200b00bad_statistics_py.html
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_8a655f2681f565c9___init___py.html
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_8a655f2681f565c9_interface_py.html
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_8a655f2681f565c9_run_py.html
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f_SimpleContinuousModule_py.html
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f___init___py.html
+-rw-r--r--   0        0        0    43471 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f_agents_py.html
+-rw-r--r--   0        0        0    27934 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f_model_py.html
+-rw-r--r--   0        0        0    34647 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f_server_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/favicon_32.png
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/keybd_open.png
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/reports/html/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/__init__.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/test_model.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/test_server.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/test_space.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/test_statistics.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 scicom-0.4.0/tests/scicom/historicalletters/test_utils.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 scicom-0.4.0/.gitignore
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 scicom-0.4.0/README.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 scicom-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 scicom-0.4.0/PKG-INFO
```

### Comparing `scicom-0.3.1/.gitlab-ci.yml` & `scicom-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tox.ini` & `scicom-0.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/HistoricalLetters.png` & `scicom-0.4.0/docs/HistoricalLetters.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/Makefile` & `scicom-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/conf.py` & `scicom-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/index.rst` & `scicom-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/make.bat` & `scicom-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/usingmesa.rst` & `scicom-0.4.0/docs/usingmesa.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/_static/bmbf.png` & `scicom-0.4.0/docs/_static/bmbf.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/_static/logo.png` & `scicom-0.4.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/docs/_static/mpiwg.png` & `scicom-0.4.0/docs/_static/mpiwg.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/examples/RunModel.ipynb` & `scicom-0.4.0/examples/RunModel.ipynb`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/interface.py` & `scicom-0.4.0/src/scicom/interface.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/run.py` & `scicom-0.4.0/src/scicom/run.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson` & `scicom-0.4.0/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson` & `scicom-0.4.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/data/pone.0162678.s003.csv` & `scicom-0.4.0/src/scicom/data/pone.0162678.s003.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/data/relPop_plosOne.csv` & `scicom-0.4.0/src/scicom/data/relPop_plosOne.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/historicalletters/agents.py` & `scicom-0.4.0/src/scicom/historicalletters/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,18 +178,25 @@
                 # agent's currently held topic positions.
                 self.model.updatedTopicsDict.update(
                     {receiver.unique_id: updatedTopicVec},
                 )
 
     def step(self) -> None:
         """Perform one simulation step."""
-        self.topicVec = self.model.updatedTopicsDict[self.unique_id]
-        self.topicLedger.append(
-            self.topicVec,
-        )
+        # If the agent has received a letter in the previous step and
+        # has updated its internal topicVec state, the new topic state is
+        # appended to the topicLedger
+        if not self.topicLedger:
+            self.topicLedger.append(
+                self.topicVec,
+            )
+        elif self.topicVec != self.topicLedger[-1]:
+            self.topicLedger.append(
+                self.topicVec,
+            )
         currentActivation = random.choices(
             population=[0, 1],
             weights=[1 - self.activationWeight, self.activationWeight],
             k=1,
         )
         if currentActivation[0] == 1:
             neighborsMove = [
```

### Comparing `scicom-0.3.1/src/scicom/historicalletters/interface.py` & `scicom-0.4.0/src/scicom/historicalletters/interface.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/historicalletters/model.py` & `scicom-0.4.0/src/scicom/historicalletters/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,39 @@
 
 
 def getPrunedLedger(model: mesa.Model) -> pd.DataFrame:
     """Model reporter for simulation of archiving.
 
     Returns statistics of ledger network of model run
     and various iterations of statistics of pruned networks.
+
+    The routine assumes that the network contains fields of sender,
+    receiver and step information.
     """
-    # TODO(malte): Add all model params
     if model.runPruning is True:
         ledgerColumns = ["sender", "receiver", "sender_location", "receiver_location", "topic", "step"]
         modelparams = {
             "population": model.population,
             "moveRange": model.moveRange,
             "letterRange": model.letterRange,
             "useActivation": model.useActivation,
             "useSocialNetwork": model.useSocialNetwork,
+            "similarityThreshold": model.similarityThreshold,
+            "longRangeNetworkFactor": model.longRangeNetworkFactor,
+            "shortRangeNetworkFactor": model.shortRangeNetworkFactor,
         }
         result = prune(
             modelparameters=modelparams,
             network=model.letterLedger,
             columns=ledgerColumns,
+            iterations=3,
+            delAmounts=(0.1, 0.25, 0.5, 0.75, 0.9),
+            delTypes=("unif", "exp", "beta", "log_normal1", "log_normal2", "log_normal3"),
+            delMethod=("agents", "regions", "time"),
+            rankedVals=(True, False),
         )
     else:
         result = model.letterLedger
     return result
 
 
 def getComponents(model: mesa.Model) -> int:
@@ -102,14 +112,15 @@
         # Parameters for agents
         self.population = population
         self.moveRange = moveRange
         self.letterRange = letterRange
         # Parameters for model
         self.runPruning = runPruning
         self.useActivation = useActivation
+        self.similarityThreshold = similarityThreshold
         self.useSocialNetwork = useSocialNetwork
         self.longRangeNetworkFactor = longRangeNetworkFactor
         self.shortRangeNetworkFactor = shortRangeNetworkFactor
         # Initialize social network
         self.socialNetwork = nx.MultiDiGraph()
         # Output variables
         self.letterLedger = []
@@ -210,18 +221,14 @@
                 self.space.add_sender(sender, regionID[0])
             except IndexError as exc:
                 text = f"Problem finding region for {sender.geometry}."
                 raise IndexError(text) from exc
             # Add sender to schedule
             self.schedule.add(sender)
 
-        # Add graph to network grid for potential visualization.
-        # TODO(malte): Not yet implemented. Maybe use Solara backend for this?
-        # self.grid = mesa.space.NetworkGrid(self.socialNetwork)
-
         # Create social network
         if useSocialNetwork is True:
             for agent in self.schedule.agents:
                 if isinstance(agent, SenderAgent):
                     self._createSocialEdges(agent, self.socialNetwork)
 
         self.datacollector = mesa.DataCollector(
@@ -265,30 +272,36 @@
                     weights=[self.longRangeNetworkFactor, 1 - self.longRangeNetworkFactor],
                     k=1,
                 )
                 if connect[0] is True:
                     graph.add_edge(agent.unique_id, neighbor.unique_id, step=0)
 
     def step(self) -> None:
-        """One simulation step."""
-        self.scaleSendInput.update(
-            **{x.unique_id: x.numLettersReceived for x in self.schedule.agents},
-        )
-        self.schedule.step()
+        """One simulation step with data collection."""
+        self.step_no_data()
         self.datacollector.collect(self)
 
     def step_no_data(self) -> None:
-        """One simulation step without datacollection."""
+        """One simulation step without data collection."""
         self.scaleSendInput.update(
             **{x.unique_id: x.numLettersReceived for x in self.schedule.agents},
         )
+        # Update the currently held topicVec for each agent, based
+        # on potential previouse communication events.
+        for agent in self.schedule.agents:
+            agent.topicVec = self.updatedTopicsDict[agent.unique_id]
         self.schedule.step()
 
     def run(self, n:int) -> None:
-        """Run the model for n steps."""
+        """Run the model for n steps.
+
+        Data collection is only run at the end of n steps.
+        This is useful for batch runs accross different
+        parameters.
+        """
         if self.debug is True:
             for _ in tqdm(range(n)):
                 self.step_no_data()
         else:
             for _ in range(n):
                 self.step_no_data()
         self.datacollector.collect(self)
```

### Comparing `scicom-0.3.1/src/scicom/historicalletters/server.py` & `scicom-0.4.0/src/scicom/historicalletters/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/historicalletters/space.py` & `scicom-0.4.0/src/scicom/historicalletters/space.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/historicalletters/utils.py` & `scicom-0.4.0/src/scicom/historicalletters/utils.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/SimpleContinuousModule.py` & `scicom-0.4.0/src/scicom/knowledgespread/SimpleContinuousModule.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/agents.py` & `scicom-0.4.0/src/scicom/knowledgespread/agents.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/interface.py` & `scicom-0.4.0/src/scicom/knowledgespread/interface.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/model.py` & `scicom-0.4.0/src/scicom/knowledgespread/model.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/server.py` & `scicom-0.4.0/src/scicom/knowledgespread/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/simple_continuous_canvas.js` & `scicom-0.4.0/src/scicom/knowledgespread/simple_continuous_canvas.js`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/src/scicom/knowledgespread/utils.py` & `scicom-0.4.0/src/scicom/knowledgespread/utils.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/reports/html/coverage_html.js` & `scicom-0.4.0/tests/reports/coverage-html/coverage_html.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -32,63 +32,52 @@
     }
 }
 
 // Helpers for table sorting
 function getCellValue(row, column = 0) {
     const cell = row.cells[column] // nosemgrep: eslint.detect-object-injection
     if (cell.childElementCount == 1) {
-        var child = cell.firstElementChild;
-        if (child.tagName === "A") {
-            child = child.firstElementChild;
-        }
-        if (child instanceof HTMLDataElement && child.value) {
-            return child.value;
+        const child = cell.firstElementChild
+        if (child instanceof HTMLTimeElement && child.dateTime) {
+            return child.dateTime
+        } else if (child instanceof HTMLDataElement && child.value) {
+            return child.value
         }
     }
     return cell.innerText || cell.textContent;
 }
 
 function rowComparator(rowA, rowB, column = 0) {
     let valueA = getCellValue(rowA, column);
     let valueB = getCellValue(rowB, column);
     if (!isNaN(valueA) && !isNaN(valueB)) {
-        return valueA - valueB;
+        return valueA - valueB
     }
     return valueA.localeCompare(valueB, undefined, {
         numeric: true
     });
 }
 
 function sortColumn(th) {
     // Get the current sorting direction of the selected header,
-    // clear state on other headers and then set the new sorting direction.
+    // clear state on other headers and then set the new sorting direction
     const currentSortOrder = th.getAttribute("aria-sort");
     [...th.parentElement.cells].forEach(header => header.setAttribute("aria-sort", "none"));
-    var direction;
     if (currentSortOrder === "none") {
-        direction = th.dataset.defaultSortOrder || "ascending";
-    } else if (currentSortOrder === "ascending") {
-        direction = "descending";
+        th.setAttribute("aria-sort", th.dataset.defaultSortOrder || "ascending");
     } else {
-        direction = "ascending";
+        th.setAttribute("aria-sort", currentSortOrder === "ascending" ? "descending" : "ascending");
     }
-    th.setAttribute("aria-sort", direction);
 
     const column = [...th.parentElement.cells].indexOf(th)
 
-    // Sort all rows and afterwards append them in order to move them in the DOM.
+    // Sort all rows and afterwards append them in order to move them in the DOM
     Array.from(th.closest("table").querySelectorAll("tbody tr"))
-        .sort((rowA, rowB) => rowComparator(rowA, rowB, column) * (direction === "ascending" ? 1 : -1))
+        .sort((rowA, rowB) => rowComparator(rowA, rowB, column) * (th.getAttribute("aria-sort") === "ascending" ? 1 : -1))
         .forEach(tr => tr.parentElement.appendChild(tr));
-
-    // Save the sort order for next time.
-    localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
-        column,
-        direction
-    }));
 }
 
 // Find all the elements with data-shortcut attribute, and use them to assign a shortcut key.
 coverage.assign_shortkeys = function() {
     document.querySelectorAll("[data-shortcut]").forEach(element => {
         document.addEventListener("keypress", event => {
             if (event.target.tagName.toLowerCase() === "input") {
@@ -105,66 +94,38 @@
 coverage.wire_up_filter = function() {
     // Cache elements.
     const table = document.querySelector("table.index");
     const table_body_rows = table.querySelectorAll("tbody tr");
     const no_rows = document.getElementById("no_rows");
 
     // Observe filter keyevents.
-    const filter_handler = (event => {
+    document.getElementById("filter").addEventListener("input", debounce(event => {
         // Keep running total of each metric, first index contains number of shown rows
         const totals = new Array(table.rows[0].cells.length).fill(0);
         // Accumulate the percentage as fraction
         totals[totals.length - 1] = {
             "numer": 0,
             "denom": 0
         }; // nosemgrep: eslint.detect-object-injection
 
-        var text = document.getElementById("filter").value;
-        const casefold = (text === text.toLowerCase());
-        const hide100 = document.getElementById("hide100").checked;
-
         // Hide / show elements.
         table_body_rows.forEach(row => {
-            var show = false;
-            // Check the text filter.
-            for (let column = 0; column < totals.length; column++) {
-                cell = row.cells[column];
-                if (cell.classList.contains("name")) {
-                    var celltext = cell.textContent;
-                    if (casefold) {
-                        celltext = celltext.toLowerCase();
-                    }
-                    if (celltext.includes(text)) {
-                        show = true;
-                    }
-                }
-            }
-
-            // Check the "hide covered" filter.
-            if (show && hide100) {
-                const [numer, denom] = row.cells[row.cells.length - 1].dataset.ratio.split(" ");
-                show = (numer !== denom);
-            }
-
-            if (!show) {
+            if (!row.cells[0].textContent.includes(event.target.value)) {
                 // hide
                 row.classList.add("hidden");
                 return;
             }
 
             // show
             row.classList.remove("hidden");
             totals[0]++;
 
-            for (let column = 0; column < totals.length; column++) {
+            for (let column = 1; column < totals.length; column++) {
                 // Accumulate dynamic totals
                 cell = row.cells[column] // nosemgrep: eslint.detect-object-injection
-                if (cell.classList.contains("name")) {
-                    continue;
-                }
                 if (column === totals.length - 1) {
                     // Last column contains percentage
                     const [numer, denom] = cell.dataset.ratio.split(" ");
                     totals[column]["numer"] += parseInt(numer, 10); // nosemgrep: eslint.detect-object-injection
                     totals[column]["denom"] += parseInt(denom, 10); // nosemgrep: eslint.detect-object-injection
                 } else {
                     totals[column] += parseInt(cell.textContent, 10); // nosemgrep: eslint.detect-object-injection
@@ -182,20 +143,17 @@
 
         // Hide placeholder, show table.
         no_rows.style.display = null;
         table.style.display = null;
 
         const footer = table.tFoot.rows[0];
         // Calculate new dynamic sum values based on visible rows.
-        for (let column = 0; column < totals.length; column++) {
+        for (let column = 1; column < totals.length; column++) {
             // Get footer cell element.
             const cell = footer.cells[column]; // nosemgrep: eslint.detect-object-injection
-            if (cell.classList.contains("name")) {
-                continue;
-            }
 
             // Set value into dynamic footer cell element.
             if (column === totals.length - 1) {
                 // Percentage column uses the numerator and denominator,
                 // and adapts to the number of decimal places.
                 const match = /\.([0-9]+)/.exec(cell.textContent);
                 const places = match ? match[1].length : 0;
@@ -208,54 +166,55 @@
                 cell.textContent = denom ?
                     `${(numer * 100 / denom).toFixed(places)}%` :
                     `${(100).toFixed(places)}%`;
             } else {
                 cell.textContent = totals[column]; // nosemgrep: eslint.detect-object-injection
             }
         }
-    });
-
-    document.getElementById("filter").addEventListener("input", debounce(filter_handler));
-    document.getElementById("hide100").addEventListener("input", debounce(filter_handler));
+    }));
 
     // Trigger change event on setup, to force filter on page refresh
     // (filter value may still be present).
     document.getElementById("filter").dispatchEvent(new Event("input"));
-    document.getElementById("hide100").dispatchEvent(new Event("input"));
 };
 
-// Set up the click-to-sort columns.
-coverage.wire_up_sorting = function() {
+coverage.INDEX_SORT_STORAGE = "COVERAGE_INDEX_SORT_2";
+
+// Loaded on index.html
+coverage.index_ready = function() {
+    coverage.assign_shortkeys();
+    coverage.wire_up_filter();
     document.querySelectorAll("[data-sortable] th[aria-sort]").forEach(
         th => th.addEventListener("click", e => sortColumn(e.target))
     );
 
     // Look for a localStorage item containing previous sort settings:
-    var column = 0,
-        direction = "ascending";
     const stored_list = localStorage.getItem(coverage.INDEX_SORT_STORAGE);
+
     if (stored_list) {
-        ({
+        const {
             column,
             direction
-        } = JSON.parse(stored_list));
+        } = JSON.parse(stored_list);
+        const th = document.querySelector("[data-sortable]").tHead.rows[0].cells[column]; // nosemgrep: eslint.detect-object-injection
+        th.setAttribute("aria-sort", direction === "ascending" ? "descending" : "ascending");
+        th.click()
     }
 
-    const th = document.querySelector("[data-sortable]").tHead.rows[0].cells[column]; // nosemgrep: eslint.detect-object-injection
-    th.setAttribute("aria-sort", direction === "ascending" ? "descending" : "ascending");
-    th.click()
-};
-
-coverage.INDEX_SORT_STORAGE = "COVERAGE_INDEX_SORT_2";
-
-// Loaded on index.html
-coverage.index_ready = function() {
-    coverage.assign_shortkeys();
-    coverage.wire_up_filter();
-    coverage.wire_up_sorting();
+    // Watch for page unload events so we can save the final sort settings:
+    window.addEventListener("unload", function() {
+        const th = document.querySelector('[data-sortable] th[aria-sort="ascending"], [data-sortable] [aria-sort="descending"]');
+        if (!th) {
+            return;
+        }
+        localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
+            column: [...th.parentElement.cells].indexOf(th),
+            direction: th.getAttribute("aria-sort"),
+        }));
+    });
 
     on_click(".button_prev_file", coverage.to_prev_file);
     on_click(".button_next_file", coverage.to_next_file);
 
     on_click(".button_show_hide_help", coverage.show_hide_help);
 };
```

### Comparing `scicom-0.3.1/tests/reports/html/favicon_32.png` & `scicom-0.4.0/tests/reports/coverage-html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/reports/html/index.html` & `scicom-0.4.0/tests/reports/html/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">44%</span>
+            <span class="pc_cov">46%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
-                        <kbd>f</kbd>
+                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -37,201 +37,192 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <form id="filter_container">
-            <input id="filter" type="text" value="" placeholder="filter...">
-            <div>
-                <input id="hide100" type="checkbox" >
-                <label for="hide100">hide covered</label>
-            </div>
+            <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
-        <h2>
-                <a class="button current">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
-        </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:29 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 15:09 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th class="name left" aria-sort="none" data-shortcut="n">Module</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing</th>
+                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded</th>
+                <th class="right" aria-sort="none" data-shortcut="c">coverage</th>
             </tr>
         </thead>
         <tbody>
-            <tr class="region">
-                <td class="name left"><a href="z_e85bc3a05b58e6d3___init___py.html">.tox/p311/lib/python3.10/site-packages/scicom/__init__.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_8a655f2681f565c9___init___py.html">.tox/p311/lib/python3.11/site-packages/scicom/__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21___init___py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/__init__.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589___init___py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_agents_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/agents.py</a></td>
-                <td>113</td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_agents_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/agents.py</a></td>
+                <td>115</td>
                 <td>8</td>
                 <td>0</td>
-                <td class="right" data-ratio="105 113">93%</td>
+                <td class="right" data-ratio="107 115">93%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_interface_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/interface.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_interface_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/interface.py</a></td>
                 <td>39</td>
                 <td>39</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 39">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_model_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/model.py</a></td>
-                <td>108</td>
-                <td>6</td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_model_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/model.py</a></td>
+                <td>110</td>
+                <td>5</td>
                 <td>0</td>
-                <td class="right" data-ratio="102 108">94%</td>
+                <td class="right" data-ratio="105 110">95%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_server_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/server.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_server_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/server.py</a></td>
                 <td>22</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="22 22">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_space_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/space.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_space_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/space.py</a></td>
                 <td>27</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="27 27">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_a9eaaac38d807e21_utils_py.html">.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/utils.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_277402163e1a7589_utils_py.html">.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/utils.py</a></td>
                 <td>39</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="39 39">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_e85bc3a05b58e6d3_interface_py.html">.tox/p311/lib/python3.10/site-packages/scicom/interface.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_8a655f2681f565c9_interface_py.html">.tox/p311/lib/python3.11/site-packages/scicom/interface.py</a></td>
                 <td>15</td>
                 <td>15</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 15">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/SimpleContinuousModule.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_SimpleContinuousModule_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/SimpleContinuousModule.py</a></td>
                 <td>23</td>
                 <td>23</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 23">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79___init___py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/__init__.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228___init___py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_agents_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/agents.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_agents_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/agents.py</a></td>
                 <td>71</td>
                 <td>71</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 71">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_interface_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/interface.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_interface_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/interface.py</a></td>
                 <td>5</td>
                 <td>5</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 5">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_model_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/model.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_model_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/model.py</a></td>
                 <td>71</td>
                 <td>71</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 71">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_server_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/server.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_server_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/server.py</a></td>
                 <td>69</td>
                 <td>69</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 69">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_124ad581c8e87a79_utils_py.html">.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/utils.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_2e9db29e074df228_utils_py.html">.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/utils.py</a></td>
                 <td>127</td>
                 <td>127</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 127">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_e85bc3a05b58e6d3_run_py.html">.tox/p311/lib/python3.10/site-packages/scicom/run.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_8a655f2681f565c9_run_py.html">.tox/p311/lib/python3.11/site-packages/scicom/run.py</a></td>
                 <td>10</td>
                 <td>10</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 10">0%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_22d2582a602e487e___init___py.html">.tox/p311/lib/python3.10/site-packages/scicom/utilities/__init__.py</a></td>
+            <tr class="file">
+                <td class="name left"><a href="d_3142edd200b00bad___init___py.html">.tox/p311/lib/python3.11/site-packages/scicom/utilities/__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
-            <tr class="region">
-                <td class="name left"><a href="z_22d2582a602e487e_statistics_py.html">.tox/p311/lib/python3.10/site-packages/scicom/utilities/statistics.py</a></td>
-                <td>57</td>
-                <td>0</td>
+            <tr class="file">
+                <td class="name left"><a href="d_3142edd200b00bad_statistics_py.html">.tox/p311/lib/python3.11/site-packages/scicom/utilities/statistics.py</a></td>
+                <td>122</td>
+                <td>24</td>
                 <td>0</td>
-                <td class="right" data-ratio="57 57">100%</td>
+                <td class="right" data-ratio="98 122">80%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>796</td>
-                <td>444</td>
+                <td>865</td>
+                <td>467</td>
                 <td>0</td>
-                <td class="right" data-ratio="352 796">44%</td>
+                <td class="right" data-ratio="398 865">46%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:29 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 15:09 +0200
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="z_22d2582a602e487e_statistics_py.html"></a>
-        <a id="nextFileLink" class="nav" href="z_e85bc3a05b58e6d3___init___py.html"></a>
-        <button type="button" class="button_prev_file" data-shortcut="["></button>
-        <button type="button" class="button_next_file" data-shortcut="]"></button>
-        <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+        <a id="prevFileLink" class="nav" href="d_3142edd200b00bad_statistics_py.html"/>
+        <a id="nextFileLink" class="nav" href="d_8a655f2681f565c9___init___py.html"/>
+        <button type="button" class="button_prev_file" data-shortcut="["/>
+        <button type="button" class="button_next_file" data-shortcut="]"/>
+        <button type="button" class="button_show_hide_help" data-shortcut="?"/>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,53 +1,51 @@
-************ CCoovveerraaggee rreeppoorrtt:: 4444%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 4466%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x c   change column sorting
+n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-??hide covered
-********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-26 14:29 +0200
-FFiillee                                    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-15 15:09 +0200
+MMoodduullee                                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
 _s_c_i_c_o_m_/_____i_n_i_t_____._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_____i_n_i_t_____._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 113        8       0        93%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 115        8       0        93%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_a_g_e_n_t_s_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 39         39      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 39         39      0        0%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_i_n_t_e_r_f_a_c_e_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 108        6       0        94%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 110        5       0        95%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_m_o_d_e_l_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 22         0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 22         0       0        100%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_s_e_r_v_e_r_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 27         0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 27         0       0        100%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_s_p_a_c_e_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 39         0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 39         0       0        100%
 _s_c_i_c_o_m_/_h_i_s_t_o_r_i_c_a_l_l_e_t_t_e_r_s_/_u_t_i_l_s_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 15         15      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 15         15      0        0%
 _s_c_i_c_o_m_/_i_n_t_e_r_f_a_c_e_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/                 23         23      0        0%
 _S_i_m_p_l_e_C_o_n_t_i_n_u_o_u_s_M_o_d_u_l_e_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_____i_n_i_t_____._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 71         71      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 71         71      0        0%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_a_g_e_n_t_s_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 5          5       0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 5          5       0        0%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_i_n_t_e_r_f_a_c_e_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 71         71      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 71         71      0        0%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_m_o_d_e_l_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 69         69      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 69         69      0        0%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_s_e_r_v_e_r_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 127        127     0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 127        127     0        0%
 _s_c_i_c_o_m_/_k_n_o_w_l_e_d_g_e_s_p_r_e_a_d_/_u_t_i_l_s_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 10         10      0        0%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 10         10      0        0%
 _s_c_i_c_o_m_/_r_u_n_._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 0          0       0        100%
 _s_c_i_c_o_m_/_u_t_i_l_i_t_i_e_s_/_____i_n_i_t_____._p_y
-_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_0_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 57         0       0        100%
+_._t_o_x_/_p_3_1_1_/_l_i_b_/_p_y_t_h_o_n_3_._1_1_/_s_i_t_e_-_p_a_c_k_a_g_e_s_/ 122        24      0        80%
 _s_c_i_c_o_m_/_u_t_i_l_i_t_i_e_s_/_s_t_a_t_i_s_t_i_c_s_._p_y
-Total                                   796        444     0        44%
+Total                                   865        467     0        46%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-26 14:29 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-15 15:09 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/keybd_closed.png` & `scicom-0.4.0/tests/reports/coverage-html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/reports/html/keybd_open.png` & `scicom-0.4.0/tests/reports/coverage-html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/reports/html/style.css` & `scicom-0.4.0/tests/reports/coverage-html/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 table { border-collapse: collapse; }
 
 td { vertical-align: top; }
 
 table tr.hidden { display: none !important; }
 
-p#no_rows { display: none; font-size: 1.15em; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; }
+p#no_rows { display: none; font-size: 1.2em; }
 
 a.nav { text-decoration: none; color: inherit; }
 
 a.nav:hover { text-decoration: underline; color: inherit; }
 
 .hidden { display: none; }
 
@@ -36,26 +36,14 @@
 
 @media (prefers-color-scheme: dark) { header { border-color: #333; } }
 
 header .content { padding: 1rem 3.5rem; }
 
 header h2 { margin-top: .5em; font-size: 1em; }
 
-header h2 a.button { font-family: inherit; font-size: inherit; border: 1px solid; border-radius: .2em; background: #eee; color: inherit; text-decoration: none; padding: .1em .5em; margin: 1px calc(.1em + 1px); cursor: pointer; border-color: #ccc; }
-
-@media (prefers-color-scheme: dark) { header h2 a.button { background: #333; } }
-
-@media (prefers-color-scheme: dark) { header h2 a.button { border-color: #444; } }
-
-header h2 a.button.current { border: 2px solid; background: #fff; border-color: #999; cursor: default; }
-
-@media (prefers-color-scheme: dark) { header h2 a.button.current { background: #1e1e1e; } }
-
-@media (prefers-color-scheme: dark) { header h2 a.button.current { border-color: #777; } }
-
 header p.text { margin: .5em 0 -.5em; color: #666; font-style: italic; }
 
 @media (prefers-color-scheme: dark) { header p.text { color: #aaa; } }
 
 header.sticky { position: fixed; left: 0; right: 0; height: 2.5em; }
 
 header.sticky .text { display: none; }
@@ -76,37 +64,27 @@
 
 @media (prefers-color-scheme: dark) { footer .content { color: #aaa; } }
 
 #index { margin: 1rem 0 0 3.5rem; }
 
 h1 { font-size: 1.25em; display: inline-block; }
 
-#filter_container { float: right; margin: 0 2em 0 0; line-height: 1.66em; }
-
-#filter_container #filter { width: 10em; padding: 0.2em 0.5em; border: 2px solid #ccc; background: #fff; color: #000; }
+#filter_container { float: right; margin: 0 2em 0 0; }
 
-@media (prefers-color-scheme: dark) { #filter_container #filter { border-color: #444; } }
+#filter_container input { width: 10em; padding: 0.2em 0.5em; border: 2px solid #ccc; background: #fff; color: #000; }
 
-@media (prefers-color-scheme: dark) { #filter_container #filter { background: #1e1e1e; } }
+@media (prefers-color-scheme: dark) { #filter_container input { border-color: #444; } }
 
-@media (prefers-color-scheme: dark) { #filter_container #filter { color: #eee; } }
+@media (prefers-color-scheme: dark) { #filter_container input { background: #1e1e1e; } }
 
-#filter_container #filter:focus { border-color: #007acc; }
+@media (prefers-color-scheme: dark) { #filter_container input { color: #eee; } }
 
-#filter_container :disabled ~ label { color: #ccc; }
+#filter_container input:focus { border-color: #007acc; }
 
-@media (prefers-color-scheme: dark) { #filter_container :disabled ~ label { color: #444; } }
-
-#filter_container label { font-size: .875em; color: #666; }
-
-@media (prefers-color-scheme: dark) { #filter_container label { color: #aaa; } }
-
-header button { font-family: inherit; font-size: inherit; border: 1px solid; border-radius: .2em; background: #eee; color: inherit; text-decoration: none; padding: .1em .5em; margin: 1px calc(.1em + 1px); cursor: pointer; border-color: #ccc; }
-
-@media (prefers-color-scheme: dark) { header button { background: #333; } }
+header button { font-family: inherit; font-size: inherit; border: 1px solid; border-radius: .2em; color: inherit; padding: .1em .5em; margin: 1px calc(.1em + 1px); cursor: pointer; border-color: #ccc; }
 
 @media (prefers-color-scheme: dark) { header button { border-color: #444; } }
 
 header button:active, header button:focus { outline: 2px dashed #007acc; }
 
 header button.run { background: #eeffee; }
 
@@ -284,51 +262,45 @@
 
 @media (prefers-color-scheme: dark) { #source p .ctxs { background: #056; } }
 
 #index { font-family: SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 0.875em; }
 
 #index table.index { margin-left: -.5em; }
 
-#index td, #index th { text-align: right; padding: .25em .5em; border-bottom: 1px solid #eee; }
+#index td, #index th { text-align: right; width: 5em; padding: .25em .5em; border-bottom: 1px solid #eee; }
 
 @media (prefers-color-scheme: dark) { #index td, #index th { border-color: #333; } }
 
-#index td.name, #index th.name { text-align: left; width: auto; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; min-width: 15em; }
+#index td.name, #index th.name { text-align: left; width: auto; }
 
-#index th { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, Cantarell, "Helvetica Neue", sans-serif; font-style: italic; color: #333; cursor: pointer; }
+#index th { font-style: italic; color: #333; cursor: pointer; }
 
 @media (prefers-color-scheme: dark) { #index th { color: #ddd; } }
 
 #index th:hover { background: #eee; }
 
 @media (prefers-color-scheme: dark) { #index th:hover { background: #333; } }
 
-#index th .arrows { color: #666; font-size: 85%; font-family: sans-serif; font-style: normal; pointer-events: none; }
-
 #index th[aria-sort="ascending"], #index th[aria-sort="descending"] { white-space: nowrap; background: #eee; padding-left: .5em; }
 
 @media (prefers-color-scheme: dark) { #index th[aria-sort="ascending"], #index th[aria-sort="descending"] { background: #333; } }
 
-#index th[aria-sort="ascending"] .arrows::after { content: " ▲"; }
-
-#index th[aria-sort="descending"] .arrows::after { content: " ▼"; }
+#index th[aria-sort="ascending"]::after { font-family: sans-serif; content: " ↑"; }
 
-#index td.name { font-size: 1.15em; }
+#index th[aria-sort="descending"]::after { font-family: sans-serif; content: " ↓"; }
 
 #index td.name a { text-decoration: none; color: inherit; }
 
-#index td.name .no-noun { font-style: italic; }
-
 #index tr.total td, #index tr.total_dynamic td { font-weight: bold; border-top: 1px solid #ccc; border-bottom: none; }
 
-#index tr.region:hover { background: #eee; }
+#index tr.file:hover { background: #eee; }
 
-@media (prefers-color-scheme: dark) { #index tr.region:hover { background: #333; } }
+@media (prefers-color-scheme: dark) { #index tr.file:hover { background: #333; } }
 
-#index tr.region:hover td.name { text-decoration: underline; color: inherit; }
+#index tr.file:hover td.name { text-decoration: underline; color: inherit; }
 
 #scroll_marker { position: fixed; z-index: 3; right: 0; top: 0; width: 16px; height: 100%; background: #fff; border-left: 1px solid #eee; will-change: transform; }
 
 @media (prefers-color-scheme: dark) { #scroll_marker { background: #1e1e1e; } }
 
 @media (prefers-color-scheme: dark) { #scroll_marker { border-color: #333; } }
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_SimpleContinuousModule_py.html` & `scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f_SimpleContinuousModule_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/SimpleContinuousModule.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/randomletters/SimpleContinuousModule.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/SimpleContinuousModule.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/randomletters/SimpleContinuousModule.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,82 +50,83 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">23 statements &nbsp;</span>
+            <span class="text">24 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">23<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">24<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_d0052f7b3fb6bc9f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">class</span> <span class="nam">SimpleCanvas</span><span class="op">(</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">VisualizationElement</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">    <span class="str">"""Display agents on a map background. No coordinates."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">    <span class="nam">local_includes</span> <span class="op">=</span> <span class="op">[</span><span class="str">"knowledgespread/simple_continuous_canvas.js"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="nam">portrayal_method</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="nam">canvas_height</span> <span class="op">=</span> <span class="num">720</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">canvas_width</span> <span class="op">=</span> <span class="num">1280</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">portrayal_method</span><span class="op">,</span> <span class="nam">canvas_height</span><span class="op">=</span><span class="num">720</span><span class="op">,</span> <span class="nam">canvas_width</span><span class="op">=</span><span class="num">1280</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">        Instantiate a new SimpleCanvas</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">portrayal_method</span> <span class="op">=</span> <span class="nam">portrayal_method</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_height</span> <span class="op">=</span> <span class="nam">canvas_height</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_width</span> <span class="op">=</span> <span class="nam">canvas_width</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">new_element</span> <span class="op">=</span> <span class="str">"new Simple_Continuous_Module({}, {})"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_width</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_height</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">js_code</span> <span class="op">=</span> <span class="str">"elements.push("</span> <span class="op">+</span> <span class="nam">new_element</span> <span class="op">+</span> <span class="str">");"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">def</span> <span class="nam">render</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">model</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="str">"""Draw agents."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">space_state</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">for</span> <span class="nam">obj</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">            <span class="nam">portrayal</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">portrayal_method</span><span class="op">(</span><span class="nam">obj</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">obj</span><span class="op">.</span><span class="nam">pos</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="nam">x</span> <span class="op">=</span> <span class="op">(</span><span class="nam">x</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_min</span><span class="op">)</span> <span class="op">/</span> <span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_max</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_min</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">y</span> <span class="op">=</span> <span class="op">(</span><span class="nam">y</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_min</span><span class="op">)</span> <span class="op">/</span> <span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_max</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_min</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">portrayal</span><span class="op">[</span><span class="str">"x"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">x</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="nam">portrayal</span><span class="op">[</span><span class="str">"y"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">y</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="nam">space_state</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">portrayal</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">return</span> <span class="nam">space_state</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">    <span class="nam">local_includes</span> <span class="op">=</span> <span class="op">[</span><span class="str">"randomletters/simple_continuous_canvas.js"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="nam">local_css_includes</span> <span class="op">=</span> <span class="op">[</span><span class="str">"randomletters/map.png"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="nam">portrayal_method</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">canvas_height</span> <span class="op">=</span> <span class="num">720</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">canvas_width</span> <span class="op">=</span> <span class="num">1280</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">portrayal_method</span><span class="op">,</span> <span class="nam">canvas_height</span><span class="op">=</span><span class="num">720</span><span class="op">,</span> <span class="nam">canvas_width</span><span class="op">=</span><span class="num">1280</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">        Instantiate a new SimpleCanvas</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">portrayal_method</span> <span class="op">=</span> <span class="nam">portrayal_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_height</span> <span class="op">=</span> <span class="nam">canvas_height</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_width</span> <span class="op">=</span> <span class="nam">canvas_width</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">new_element</span> <span class="op">=</span> <span class="str">"new Simple_Continuous_Module({}, {})"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_width</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">canvas_height</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">js_code</span> <span class="op">=</span> <span class="str">"elements.push("</span> <span class="op">+</span> <span class="nam">new_element</span> <span class="op">+</span> <span class="str">");"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">def</span> <span class="nam">render</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">model</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="str">"""How to render the agents"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">space_state</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">for</span> <span class="nam">obj</span> <span class="key">in</span> <span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">portrayal</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">portrayal_method</span><span class="op">(</span><span class="nam">obj</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="op">=</span> <span class="nam">obj</span><span class="op">.</span><span class="nam">pos</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">x</span> <span class="op">=</span> <span class="op">(</span><span class="nam">x</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_min</span><span class="op">)</span> <span class="op">/</span> <span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_max</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">x_min</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">y</span> <span class="op">=</span> <span class="op">(</span><span class="nam">y</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_min</span><span class="op">)</span> <span class="op">/</span> <span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_max</span> <span class="op">-</span> <span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">y_min</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="nam">portrayal</span><span class="op">[</span><span class="str">"x"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">x</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="nam">portrayal</span><span class="op">[</span><span class="str">"y"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">y</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">            <span class="nam">space_state</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">portrayal</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="nam">space_state</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79___init___py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_d0052f7b3fb6bc9f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-kknnoowwlleeddggeesspprreeaadd//SSiimmpplleeCCoonnttiinnuuoouussMMoodduullee..ppyy:: 00%% ************
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+rraannddoommlleetttteerrss//SSiimmpplleeCCoonnttiinnuuoouussMMoodduullee..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2233 ssttaatteemmeennttss ?  00 rruunn 2233 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+********** 2244 ssttaatteemmeennttss ?  00 rruunn 2244 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
 _1import mesa 
 _2 
 _3 
 _4class SimpleCanvas(mesa.visualization.VisualizationElement): 
 _5 """Display agents on a map background. No coordinates.""" 
-_6 local_includes = ["knowledgespread/simple_continuous_canvas.js"] 
-_7 portrayal_method = None 
-_8 canvas_height = 720 
-_9 canvas_width = 1280 
-_1_0 
-_1_1 def __init__(self, portrayal_method, canvas_height=720, canvas_width=1280): 
-_1_2 """ 
-_1_3 Instantiate a new SimpleCanvas 
-_1_4 """ 
-_1_5 self.portrayal_method = portrayal_method 
-_1_6 self.canvas_height = canvas_height 
-_1_7 self.canvas_width = canvas_width 
-_1_8 new_element = "new Simple_Continuous_Module({}, {})".format( 
-_1_9 self.canvas_width, self.canvas_height 
-_2_0 ) 
-_2_1 self.js_code = "elements.push(" + new_element + ");" 
-_2_2 
-_2_3 def render(self, model): 
-_2_4 """Draw agents.""" 
-_2_5 space_state = [] 
-_2_6 for obj in model.schedule.agents: 
-_2_7 portrayal = self.portrayal_method(obj) 
-_2_8 x, y = obj.pos 
-_2_9 x = (x - model.space.x_min) / (model.space.x_max - model.space.x_min) 
-_3_0 y = (y - model.space.y_min) / (model.space.y_max - model.space.y_min) 
-_3_1 portrayal["x"] = x 
-_3_2 portrayal["y"] = y 
-_3_3 space_state.append(portrayal) 
-_3_4 return space_state 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_6 local_includes = ["randomletters/simple_continuous_canvas.js"] 
+_7 local_css_includes = ["randomletters/map.png"] 
+_8 portrayal_method = None 
+_9 canvas_height = 720 
+_1_0 canvas_width = 1280 
+_1_1 
+_1_2 def __init__(self, portrayal_method, canvas_height=720, canvas_width=1280): 
+_1_3 """ 
+_1_4 Instantiate a new SimpleCanvas 
+_1_5 """ 
+_1_6 self.portrayal_method = portrayal_method 
+_1_7 self.canvas_height = canvas_height 
+_1_8 self.canvas_width = canvas_width 
+_1_9 new_element = "new Simple_Continuous_Module({}, {})".format( 
+_2_0 self.canvas_width, self.canvas_height 
+_2_1 ) 
+_2_2 self.js_code = "elements.push(" + new_element + ");" 
+_2_3 
+_2_4 def render(self, model): 
+_2_5 """How to render the agents""" 
+_2_6 space_state = [] 
+_2_7 for obj in model.schedule.agents: 
+_2_8 portrayal = self.portrayal_method(obj) 
+_2_9 x, y = obj.pos 
+_3_0 x = (x - model.space.x_min) / (model.space.x_max - model.space.x_min) 
+_3_1 y = (y - model.space.y_min) / (model.space.y_max - model.space.y_min) 
+_3_2 portrayal["x"] = x 
+_3_3 portrayal["y"] = y 
+_3_4 space_state.append(portrayal) 
+_3_5 return space_state 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79___init___py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_baa64d8b15786095___init___py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/__init__.py: 100%</title>
+    <title>Coverage for src/scicom/randomletters/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/__init__.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/randomletters/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,42 +56,42 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_baa64d8b15786095_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_baa64d8b15786095_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_baa64d8b15786095_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_baa64d8b15786095_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-kknnoowwlleeddggeesspprreeaadd//____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//rraannddoommlleetttteerrss//____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_agents_py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_agents_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/agents.py: 0%</title>
+    <title>Coverage for src/scicom/knowledgespread/agents.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/agents.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/knowledgespread/agents.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,161 +50,161 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">71 statements &nbsp;</span>
+            <span class="text">73 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">71<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">73<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_interface_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_app_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">knowledgespread</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">epistemicRange</span><span class="op">,</span> <span class="nam">ageFunction</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">networkx</span> <span class="key">as</span> <span class="nam">nx</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">knowledgespread</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">ageFunction</span><span class="op">,</span> <span class="nam">epistemicRange</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">ScientistAgent</span><span class="op">(</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Agent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""A scientist with an idea.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    Each scientist has a geographic position, is related to other</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    agents by a social network, and is intialized with a starttime, that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    describes the year at which the agent becomes active. </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">unique_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">model</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">pos</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># The projected position in 2D epistemic space. For actual movements and neighborhood calculations take into account z coordinate as well.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">topicledger</span><span class="op">:</span> <span class="nam">list</span><span class="op">,</span>  <span class="com"># Representing the mental model of the agent: A list of all visited topics represented as triples [(x,y,z), (x,y,z)]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">geopos</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># Representing scientific affiliation, a tuple of latitude/longitude of current affiliation. Could also keep track of previous affiliations</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">birthtime</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>  <span class="com"># A step number that represents the timestep at which the scientist becomes active</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">productivity</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># Parameters determining the shape of the activation weight function</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">opposition</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>  <span class="com"># Whether or not an agent is always oposing new epistemic positions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">pos</span> <span class="op">=</span> <span class="nam">pos</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">a</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">b</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">c</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">2</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span> <span class="op">=</span> <span class="nam">topicledger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">geopos</span> <span class="op">=</span> <span class="nam">geopos</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">birthtime</span> <span class="op">=</span> <span class="nam">birthtime</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">age</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">opposition</span> <span class="op">=</span> <span class="nam">opposition</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="str">"""Return an age dependent activation weight.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        A bell-shaped function with a ramp, plateuax and decend.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        Can be drawn from random distribution in model initialization.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">return</span> <span class="nam">ageFunction</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">b</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">c</span><span class="op">,</span> <span class="nam">radius</span><span class="op">=</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">_changeEpistemicPosition</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">neighbors</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="str">"""Calculate the change in epistemic space.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        From all neighbors select one random choice.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">        To update the agents position, determine the heading </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">        towards the selected neighbor. If the agent is an</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">        oposing one, inverte the direction. Then select a </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">        random amount to move into the selected direction.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">        The new position is noted down in the topic ledger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        an the the agent is moved.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="com"># Select random elemt from potential neighbors</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="nam">neighborID</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">choice</span><span class="op">(</span><span class="nam">neighbors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">neighborID</span><span class="op">,</span> <span class="op">(</span><span class="nam">float</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="nam">neighbors</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                <span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span> <span class="key">if</span> <span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">==</span> <span class="nam">neighborID</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbors</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">                <span class="nam">neighbor</span> <span class="op">=</span> <span class="nam">neighbors</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">neighbor</span> <span class="op">=</span> <span class="nam">neighborID</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="com"># Get heading</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">direction</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_heading</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">pos</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="com"># Some agents always opose the epistemic position and therefore move in the oposite direction</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">opposition</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">            <span class="nam">direction</span> <span class="op">=</span> <span class="op">(</span><span class="op">-</span> <span class="nam">direction</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="op">-</span> <span class="nam">direction</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="com"># Select new postion with random amount into direction of neighbor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">amount</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="nam">new_pos</span> <span class="op">=</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">+</span> <span class="nam">amount</span> <span class="op">*</span> <span class="nam">direction</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="op">+</span> <span class="nam">amount</span> <span class="op">*</span> <span class="nam">direction</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="com"># New mental position</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="nam">topic</span> <span class="op">=</span> <span class="op">(</span><span class="nam">new_pos</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">new_pos</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="com"># Move agent</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">topic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">move_agent</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">new_pos</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">except</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="com"># Out of bounds of epi space</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="com"># TODO: What is a sensible exception of movement in this case.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="com"># Current solution: Append topic to ledger but do not move</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">topic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">def</span> <span class="nam">updateSocialNetwork</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="str">"""Create new links in agents social network."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">class</span> <span class="nam">ScientistAgent</span><span class="op">(</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Agent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="str">"""A scientist with an idea.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Each scientist has a geographic position, is related to other</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    agents by a social network, and is intialized with a starttime, that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    describes the year at which the agent becomes active. </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">unique_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">model</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">pos</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># The projected position in 2D epistemic space. For actual movements and neighborhood calculations take into account z coordinate as well. </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">topicledger</span><span class="op">:</span> <span class="nam">list</span><span class="op">,</span>  <span class="com"># Representing the mental model of the agent: A list of all visited topics represented as triples [(x,y,z), (x,y,z)] </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">geopos</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># Representing scientific affiliation, a tuple of latitude/longitude of current affiliation. Could also keep track of previous affiliations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">birthtime</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>  <span class="com"># A step number that represents the timestep at which the scientist becomes active</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">productivity</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span>  <span class="com"># Parameters determining the shape of the activation weight function</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">opposition</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>  <span class="com"># Whether or not an agent is always oposing new epistemic positions.  </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">pos</span> <span class="op">=</span> <span class="nam">pos</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">a</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">b</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">c</span> <span class="op">=</span> <span class="nam">productivity</span><span class="op">[</span><span class="num">2</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span> <span class="op">=</span> <span class="nam">topicledger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">geopos</span> <span class="op">=</span> <span class="nam">geopos</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">birthtime</span> <span class="op">=</span> <span class="nam">birthtime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">age</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">opposition</span> <span class="op">=</span> <span class="nam">opposition</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""Returns an age dependent activation weight.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        A bell-shaped function with a ramp, plateuax and decend.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        Can be drawn from random distribution in model initialization.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="key">return</span> <span class="nam">ageFunction</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">a</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">b</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">c</span><span class="op">,</span> <span class="nam">radius</span><span class="op">=</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">def</span> <span class="nam">_changeEpistemicPosition</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">neighbors</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="str">"""Calculate the change in epistemic space.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">        From all neighbors select one random choice.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        To update the agents position, determine the heading </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">        towards the selected neighbor. If the agent is an</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">        oposing one, inverte the direction. Then select a </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">        random amount to move into the selected direction.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">        The new position is noted down in the topic ledger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">        an the the agent is moved.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="com"># Select random elemt from potential neighbors</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">neighborID</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">choice</span><span class="op">(</span><span class="nam">neighbors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">neighborID</span><span class="op">,</span> <span class="nam">float</span><span class="op">)</span> <span class="key">or</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">neighborID</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">neighbors</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">                <span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span> <span class="key">if</span> <span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">==</span> <span class="nam">neighborID</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbors</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">                <span class="nam">neighbor</span> <span class="op">=</span> <span class="nam">neighbors</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="nam">neighbor</span> <span class="op">=</span> <span class="nam">neighborID</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="com"># Get heading</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">direction</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_heading</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">pos</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="com"># Some agents always opose the epistemic position and therefore move in the oposite direction</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">opposition</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">            <span class="nam">direction</span> <span class="op">=</span> <span class="op">(</span><span class="op">-</span> <span class="nam">direction</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="op">-</span> <span class="nam">direction</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="com"># Select new postion with random amount into direction of neighbor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">amount</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">new_pos</span> <span class="op">=</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">+</span> <span class="nam">amount</span> <span class="op">*</span> <span class="nam">direction</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="op">+</span> <span class="nam">amount</span> <span class="op">*</span> <span class="nam">direction</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="com"># New mental position</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">topic</span> <span class="op">=</span> <span class="op">(</span><span class="nam">new_pos</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">new_pos</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="com"># Move agent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">topic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">move_agent</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">new_pos</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="key">except</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">            <span class="com"># Out of bounds of epi space</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="com"># TODO: What is a sensible exception of movement in this case.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="com"># Current solution: Append topic to ledger but do not move</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicledger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">topic</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">def</span> <span class="nam">updateSocialNetwork</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="str">"""Create new links in agents social network."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">    <span class="key">def</span> <span class="nam">moveGeoSpace</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="key">def</span> <span class="nam">moveSocSpace</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">maxDist</span><span class="op">=</span><span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="str">"""Change epistemic position based on social network."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">neighbors</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">currentTime</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">G</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">socialNetwork</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">H</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">Graph</span><span class="op">(</span><span class="op">(</span><span class="op">(</span><span class="nam">u</span><span class="op">,</span> <span class="nam">v</span><span class="op">,</span> <span class="nam">e</span><span class="op">)</span> <span class="key">for</span> <span class="nam">u</span><span class="op">,</span> <span class="nam">v</span><span class="op">,</span> <span class="nam">e</span> <span class="key">in</span> <span class="nam">G</span><span class="op">.</span><span class="nam">edges</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="key">True</span><span class="op">)</span> <span class="key">if</span> <span class="nam">e</span><span class="op">[</span><span class="str">"time"</span><span class="op">]</span> <span class="op">&lt;=</span> <span class="nam">currentTime</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">H</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">Graph</span><span class="op">(</span><span class="op">(</span><span class="op">(</span><span class="nam">u</span><span class="op">,</span> <span class="nam">v</span><span class="op">,</span> <span class="nam">e</span><span class="op">)</span> <span class="key">for</span> <span class="nam">u</span><span class="op">,</span> <span class="nam">v</span><span class="op">,</span> <span class="nam">e</span> <span class="key">in</span> <span class="nam">G</span><span class="op">.</span><span class="nam">edges</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="key">True</span><span class="op">)</span> <span class="key">if</span> <span class="nam">e</span><span class="op">[</span><span class="str">'time'</span><span class="op">]</span> <span class="op">&lt;=</span> <span class="nam">currentTime</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="key">for</span> <span class="nam">dist</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="nam">maxDist</span> <span class="op">+</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">neighb</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">descendants_at_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="nam">H</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                <span class="nam">dist</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                <span class="nam">dist</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">            <span class="nam">neighbors</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">list</span><span class="op">(</span><span class="nam">neighb</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="key">if</span> <span class="nam">neighbors</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_changeEpistemicPosition</span><span class="op">(</span><span class="nam">neighbors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">            <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">            <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">def</span> <span class="nam">moveEpiSpace</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="str">"""Change epistemic position based on distance in epistemic space."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">neighbors</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">pos</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">            <span class="nam">radius</span><span class="op">=</span><span class="nam">epistemicRange</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">epiRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">birthtime</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">birthtime</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="key">if</span> <span class="nam">neighbors</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_changeEpistemicPosition</span><span class="op">(</span><span class="nam">neighbors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="com"># Random search for new epistemic position</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="nam">direction</span> <span class="op">=</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="nam">new_pos</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span> <span class="op">*</span> <span class="nam">direction</span>&nbsp;</span><span class="r"></span></p>
@@ -226,36 +226,37 @@
     <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="str">        the agent is removed from the schedule.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span> <span class="op">&lt;</span> <span class="nam">self</span><span class="op">.</span><span class="nam">birthtime</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">            <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">elif</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="op">)</span> <span class="op">&lt;=</span> <span class="num">0.00001</span> <span class="key">and</span> <span class="nam">self</span><span class="op">.</span><span class="nam">age</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="com"># self.age += 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">age</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">currentActivation</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">                <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                    <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">                <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="key">if</span> <span class="nam">currentActivation</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">                <span class="com"># TODO: Should the choice of movement be another random process?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">                <span class="nam">res</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">moveSocSpace</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="key">if</span> <span class="nam">res</span> <span class="key">is</span> <span class="key">False</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">moveEpiSpace</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">age</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">            <span class="nam">currentActivation</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">                    <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_currentActivationWeight</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">                <span class="nam">k</span><span class="op">=</span><span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="key">if</span> <span class="nam">currentActivation</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">                <span class="com"># TODO: Should the choice of movement be another random process?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="nam">res</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">moveSocSpace</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                <span class="key">if</span> <span class="nam">res</span> <span class="key">is</span> <span class="key">False</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">moveEpiSpace</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_interface_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_app_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,153 +1,152 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-kknnoowwlleeddggeesspprreeaadd//aaggeennttss..ppyy:: 00%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//kknnoowwlleeddggeesspprreeaadd//aaggeennttss..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 7711 ssttaatteemmeennttss ?  00 rruunn 7711 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+********** 7733 ssttaatteemmeennttss ?  00 rruunn 7733 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
 _1 
-_2import mesa 
+_2from scicom.knowledgespread.utils import epistemicRange, ageFunction 
 _3import networkx as nx 
-_4 
-_5from scicom.knowledgespread.utils import ageFunction, epistemicRange 
+_4import mesa 
+_5 
 _6 
-_7 
-_8class ScientistAgent(mesa.Agent): 
-_9 """A scientist with an idea. 
-_1_0  
-_1_1 Each scientist has a geographic position, is related to other 
-_1_2 agents by a social network, and is intialized with a starttime, that 
-_1_3 describes the year at which the agent becomes active.  
-_1_4 """ 
-_1_5 
-_1_6 def __init__( 
-_1_7 self, 
-_1_8 unique_id, 
-_1_9 model, 
-_2_0 pos: tuple, # The projected position in 2D epistemic space. For actual
-movements and neighborhood calculations take into account z coordinate as
-well. 
-_2_1 topicledger: list, # Representing the mental model of the agent: A list of
-all visited topics represented as triples [(x,y,z), (x,y,z)] 
-_2_2 geopos: tuple, # Representing scientific affiliation, a tuple of latitude/
+_7class ScientistAgent(mesa.Agent): 
+_8 """A scientist with an idea. 
+_9  
+_1_0 Each scientist has a geographic position, is related to other 
+_1_1 agents by a social network, and is intialized with a starttime, that 
+_1_2 describes the year at which the agent becomes active.  
+_1_3 """ 
+_1_4 
+_1_5 def __init__( 
+_1_6 self, 
+_1_7 unique_id, 
+_1_8 model, 
+_1_9 pos: tuple, # The projected position in 2D epistemic space. For actual
+movements and neighborhood calculations take into account z coordinate as well.
+ 
+_2_0 topicledger: list, # Representing the mental model of the agent: A list of
+all visited topics represented as triples [(x,y,z), (x,y,z)]  
+_2_1 geopos: tuple, # Representing scientific affiliation, a tuple of latitude/
 longitude of current affiliation. Could also keep track of previous
 affiliations 
-_2_3 birthtime: int, # A step number that represents the timestep at which the
+_2_2 birthtime: int, # A step number that represents the timestep at which the
 scientist becomes active 
-_2_4 productivity: tuple, # Parameters determining the shape of the activation
+_2_3 productivity: tuple, # Parameters determining the shape of the activation
 weight function 
-_2_5 opposition: bool = False, # Whether or not an agent is always oposing new
-epistemic positions. 
-_2_6 ): 
-_2_7 super().__init__(unique_id, model) 
-_2_8 self.pos = pos 
-_2_9 self.a = productivity[0] 
-_3_0 self.b = productivity[1] 
-_3_1 self.c = productivity[2] 
-_3_2 self.topicledger = topicledger 
-_3_3 self.geopos = geopos 
-_3_4 self.birthtime = birthtime 
-_3_5 self.age = 0 
-_3_6 self.opposition = opposition 
-_3_7 
-_3_8 def _currentActivationWeight(self) -> float: 
-_3_9 """Return an age dependent activation weight. 
-_4_0 
-_4_1 A bell-shaped function with a ramp, plateuax and decend. 
-_4_2 Can be drawn from random distribution in model initialization. 
-_4_3 """ 
-_4_4 return ageFunction(self, self.a, self.b, self.c, radius=1) 
-_4_5 
-_4_6 def _changeEpistemicPosition(self, neighbors): 
-_4_7 """Calculate the change in epistemic space. 
-_4_8 
-_4_9 From all neighbors select one random choice. 
-_5_0 To update the agents position, determine the heading  
-_5_1 towards the selected neighbor. If the agent is an 
-_5_2 oposing one, inverte the direction. Then select a  
-_5_3 random amount to move into the selected direction. 
-_5_4 The new position is noted down in the topic ledger 
-_5_5 an the the agent is moved. 
-_5_6 """ 
-_5_7 # Select random elemt from potential neighbors 
-_5_8 neighborID = self.random.choice(neighbors) 
-_5_9 if isinstance(neighborID, (float, int)): 
-_6_0 neighbors = [ 
-_6_1 x for x in self.model.schedule.agents if x.unique_id == neighborID 
-_6_2 ] 
-_6_3 if neighbors: 
-_6_4 neighbor = neighbors[0] 
-_6_5 else: 
-_6_6 return 
-_6_7 else: 
-_6_8 neighbor = neighborID 
-_6_9 # Get heading 
-_7_0 direction = self.model.space.get_heading(self.pos, neighbor.pos) 
-_7_1 # Some agents always opose the epistemic position and therefore move in the
+_2_4 opposition: bool = False, # Whether or not an agent is always oposing new
+epistemic positions.  
+_2_5 ): 
+_2_6 super().__init__(unique_id, model) 
+_2_7 self.pos = pos 
+_2_8 self.a = productivity[0] 
+_2_9 self.b = productivity[1] 
+_3_0 self.c = productivity[2] 
+_3_1 self.topicledger = topicledger 
+_3_2 self.geopos = geopos 
+_3_3 self.birthtime = birthtime 
+_3_4 self.age = 0 
+_3_5 self.opposition = opposition 
+_3_6 
+_3_7 def _currentActivationWeight(self): 
+_3_8 """Returns an age dependent activation weight. 
+_3_9  
+_4_0 A bell-shaped function with a ramp, plateuax and decend. 
+_4_1 Can be drawn from random distribution in model initialization. 
+_4_2 """ 
+_4_3 return ageFunction(self, self.a, self.b, self.c, radius=1) 
+_4_4 
+_4_5 def _changeEpistemicPosition(self, neighbors): 
+_4_6 """Calculate the change in epistemic space. 
+_4_7  
+_4_8 From all neighbors select one random choice. 
+_4_9 To update the agents position, determine the heading  
+_5_0 towards the selected neighbor. If the agent is an 
+_5_1 oposing one, inverte the direction. Then select a  
+_5_2 random amount to move into the selected direction. 
+_5_3 The new position is noted down in the topic ledger 
+_5_4 an the the agent is moved. 
+_5_5 """ 
+_5_6 # Select random elemt from potential neighbors 
+_5_7 neighborID = self.random.choice(neighbors) 
+_5_8 if isinstance(neighborID, float) or isinstance(neighborID, int): 
+_5_9 neighbors = [ 
+_6_0 x for x in self.model.schedule.agents if x.unique_id == neighborID 
+_6_1 ] 
+_6_2 if neighbors: 
+_6_3 neighbor = neighbors[0] 
+_6_4 else: 
+_6_5 return 
+_6_6 else: 
+_6_7 neighbor = neighborID 
+_6_8 # Get heading 
+_6_9 direction = self.model.space.get_heading(self.pos, neighbor.pos) 
+_7_0 # Some agents always opose the epistemic position and therefore move in the
 oposite direction 
-_7_2 if self.opposition is True: 
-_7_3 direction = (- direction[0], - direction[1]) 
-_7_4 # Select new postion with random amount into direction of neighbor 
-_7_5 amount = self.model.random.random() 
-_7_6 new_pos = (self.pos[0] + amount * direction[0], self.pos[1] + amount *
+_7_1 if self.opposition is True: 
+_7_2 direction = (- direction[0], - direction[1]) 
+_7_3 # Select new postion with random amount into direction of neighbor 
+_7_4 amount = self.model.random.random() 
+_7_5 new_pos = (self.pos[0] + amount * direction[0], self.pos[1] + amount *
 direction[1]) 
-_7_7 # New mental position 
-_7_8 topic = (new_pos[0], new_pos[1], self.model.random.random()) 
-_7_9 try: 
-_8_0 # Move agent 
-_8_1 self.topicledger.append(topic) 
-_8_2 self.model.space.move_agent(self, new_pos) 
-_8_3 except: 
-_8_4 # Out of bounds of epi space 
-_8_5 # TODO: What is a sensible exception of movement in this case. 
-_8_6 # Current solution: Append topic to ledger but do not move 
-_8_7 self.topicledger.append(topic) 
-_8_8 
-_8_9 def updateSocialNetwork(self): 
-_9_0 """Create new links in agents social network.""" 
+_7_6 # New mental position 
+_7_7 topic = (new_pos[0], new_pos[1], self.model.random.random()) 
+_7_8 try: 
+_7_9 # Move agent 
+_8_0 self.topicledger.append(topic) 
+_8_1 self.model.space.move_agent(self, new_pos) 
+_8_2 except: 
+_8_3 # Out of bounds of epi space 
+_8_4 # TODO: What is a sensible exception of movement in this case. 
+_8_5 # Current solution: Append topic to ledger but do not move 
+_8_6 self.topicledger.append(topic) 
+_8_7 
+_8_8 def updateSocialNetwork(self): 
+_8_9 """Create new links in agents social network.""" 
+_9_0 pass 
 _9_1 
 _9_2 def moveGeoSpace(self): 
 _9_3 pass 
 _9_4 
 _9_5 def moveSocSpace(self, maxDist=1): 
 _9_6 """Change epistemic position based on social network.""" 
 _9_7 neighbors = [] 
 _9_8 currentTime = self.model.schedule.time 
 _9_9 G = self.model.socialNetwork 
-_1_0_0 H = nx.Graph(((u, v, e) for u, v, e in G.edges(data=True) if e["time"] <=
+_1_0_0 H = nx.Graph(((u, v, e) for u, v, e in G.edges(data=True) if e['time'] <=
 currentTime)) 
 _1_0_1 for dist in range(0, maxDist + 1, 1): 
 _1_0_2 neighb = nx.descendants_at_distance( 
 _1_0_3 H, 
 _1_0_4 self.unique_id, 
-_1_0_5 dist, 
+_1_0_5 dist 
 _1_0_6 ) 
 _1_0_7 neighbors.extend(list(neighb)) 
 _1_0_8 if neighbors: 
 _1_0_9 self._changeEpistemicPosition(neighbors) 
 _1_1_0 return True 
 _1_1_1 else: 
 _1_1_2 return False 
 _1_1_3 
 _1_1_4 def moveEpiSpace(self): 
 _1_1_5 """Change epistemic position based on distance in epistemic space.""" 
 _1_1_6 neighbors = self.model.space.get_neighbors( 
 _1_1_7 self.pos, 
 _1_1_8 radius=epistemicRange( 
 _1_1_9 self.model.epiRange, 
-_1_2_0 self.model.schedule.time - self.birthtime, 
-_1_2_1 ), 
+_1_2_0 self.model.schedule.time - self.birthtime 
+_1_2_1 ) 
 _1_2_2 ) 
 _1_2_3 if neighbors: 
 _1_2_4 self._changeEpistemicPosition(neighbors) 
 _1_2_5 else: 
 _1_2_6 # Random search for new epistemic position 
 _1_2_7 direction = (self.model.random.random(), self.model.random.random()) 
 _1_2_8 new_pos = self.model.random.random() * direction 
@@ -169,23 +168,24 @@
 _1_4_4 the agent is removed from the schedule. 
 _1_4_5 """ 
 _1_4_6 if self.model.schedule.time < self.birthtime: 
 _1_4_7 pass 
 _1_4_8 elif self._currentActivationWeight() <= 0.00001 and self.age > 1: 
 _1_4_9 self.model.schedule.remove(self) 
 _1_5_0 # self.age += 1 
-_1_5_1 else: 
-_1_5_2 self.age += 1 
-_1_5_3 currentActivation = self.model.random.choices( 
-_1_5_4 population=[0, 1], 
-_1_5_5 weights=[ 
-_1_5_6 1 - self._currentActivationWeight(), self._currentActivationWeight(), 
-_1_5_7 ], 
-_1_5_8 k=1, 
-_1_5_9 ) 
-_1_6_0 if currentActivation[0] == 1: 
-_1_6_1 # TODO: Should the choice of movement be another random process? 
-_1_6_2 res = self.moveSocSpace() 
-_1_6_3 if res is False: 
-_1_6_4 self.moveEpiSpace() 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_1_5_1 pass 
+_1_5_2 else: 
+_1_5_3 self.age += 1 
+_1_5_4 currentActivation = self.model.random.choices( 
+_1_5_5 population=[0, 1], 
+_1_5_6 weights=[ 
+_1_5_7 1 - self._currentActivationWeight(), self._currentActivationWeight() 
+_1_5_8 ], 
+_1_5_9 k=1 
+_1_6_0 ) 
+_1_6_1 if currentActivation[0] == 1: 
+_1_6_2 # TODO: Should the choice of movement be another random process? 
+_1_6_3 res = self.moveSocSpace() 
+_1_6_4 if res is False: 
+_1_6_5 self.moveEpiSpace() 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_app_py.html` & `scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_app_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/app.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/app.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/app.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/app.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">9 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">9<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_model_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">experimental</span> <span class="key">import</span> <span class="nam">JupyterViz</span><span class="op">,</span> <span class="nam">make_text</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">altair</span> <span class="key">as</span> <span class="nam">alt</span>&nbsp;</span><span class="r"></span></p>
@@ -147,18 +147,18 @@
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">agent_portrayal</span><span class="op">=</span><span class="nam">agent_draw_altair</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">space_drawer</span><span class="op">=</span><span class="nam">epiSpace_draw_altair</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_model_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 kknnoowwlleeddggeesspprreeaadd//aapppp..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 99 ssttaatteemmeennttss ?  00 rruunn 99 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
 _1import mesa 
 _2from mesa.experimental import JupyterViz, make_text 
 _3import altair as alt 
 _4 
 _5from scicom.knowledgespread.agents import ScientistAgent 
 _6from scicom.knowledgespread.model import ( 
 _7 KnowledgeSpread, 
@@ -76,9 +76,9 @@
 _6_2 model_params, 
 _6_3 measures=[socialNetwork_draw_altair, chart_draw_altair_agents,
 chart_draw_altair_communities], 
 _6_4 name="Knowledge spread", 
 _6_5 agent_portrayal=agent_draw_altair, 
 _6_6 space_drawer=epiSpace_draw_altair 
 _6_7) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_interface_py.html` & `scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_interface_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/interface.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/interface.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/interface.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/interface.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">5 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_model_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""The interface to control and run the Knowledgespread ABM."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">experimental</span> <span class="key">import</span> <span class="nam">JupyterViz</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -142,18 +142,18 @@
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">agent_portrayal</span><span class="op">=</span><span class="nam">agent_draw_altair</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">space_drawer</span><span class="op">=</span><span class="nam">epiSpace_draw_altair</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_model_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 kknnoowwlleeddggeesspprreeaadd//iinntteerrffaaccee..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 55 ssttaatteemmeennttss ?  00 rruunn 55 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
 _1"""The interface to control and run the Knowledgespread ABM.""" 
 _2from mesa.experimental import JupyterViz 
 _3 
 _4from scicom.knowledgespread.model import ( 
 _5 KnowledgeSpread, 
 _6) 
 _7from scicom.knowledgespread.server import ( 
@@ -71,9 +71,9 @@
 _5_7 model_params, 
 _5_8 measures=[socialNetwork_draw_altair, chart_draw_altair_agents,
 chart_draw_altair_communities], 
 _5_9 name="Knowledge spread", 
 _6_0 agent_portrayal=agent_draw_altair, 
 _6_1 space_drawer=epiSpace_draw_altair, 
 _6_2) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_model_py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_model_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/model.py: 0%</title>
+    <title>Coverage for src/scicom/knowledgespread/model.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/model.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/knowledgespread/model.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">71 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">71<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_app_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_app_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_server_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">networkx</span> <span class="key">as</span> <span class="nam">nx</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">knowledgespread</span><span class="op">.</span><span class="nam">agents</span> <span class="key">import</span> <span class="nam">ScientistAgent</span>&nbsp;</span><span class="r"></span></p>
@@ -249,18 +249,18 @@
     <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="str">"""Run model for n steps."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">step</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_app_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_server_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_app_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-kknnoowwlleeddggeesspprreeaadd//mmooddeell..ppyy:: 00%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//kknnoowwlleeddggeesspprreeaadd//mmooddeell..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 7711 ssttaatteemmeennttss ?  00 rruunn 7711 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
 _1import networkx as nx 
 _2import mesa 
 _3from scicom.knowledgespread.agents import ScientistAgent 
 _4from scicom.knowledgespread.utils import GenerateInitalPopulation,
 GenerateSocNet 
 _5 
 _6 
@@ -188,9 +187,9 @@
 _1_6_3 self.schedule.step() 
 _1_6_4 self.datacollector.collect(self) 
 _1_6_5 
 _1_6_6 def run(self, n): 
 _1_6_7 """Run model for n steps.""" 
 _1_6_8 for _ in range(n): 
 _1_6_9 self.step() 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_server_py.html` & `scicom-0.4.0/tests/reports/html/d_2e9db29e074df228_server_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/server.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/server.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/server.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/knowledgespread/server.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">69 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">69<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_utils_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">altair</span> <span class="key">as</span> <span class="nam">alt</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">networkx</span> <span class="key">as</span> <span class="nam">nx</span>&nbsp;</span><span class="r"></span></p>
@@ -267,18 +267,18 @@
     <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="str">"Knowledge spread"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">model_params</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_utils_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 kknnoowwlleeddggeesspprreeaadd//sseerrvveerr..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 6699 ssttaatteemmeennttss ?  00 rruunn 6699 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
 _1import altair as alt 
 _2import mesa 
 _3import networkx as nx 
 _4import nx_altair as nxa 
 _5import pandas as pd 
 _6import solara 
 _7from matplotlib import colors 
@@ -199,9 +199,9 @@
 _1_8_1 
 _1_8_2server = mesa.visualization.ModularServer( 
 _1_8_3 KnowledgeSpread, 
 _1_8_4 [epistemic_canvas, chart], 
 _1_8_5 "Knowledge spread", 
 _1_8_6 model_params, 
 _1_8_7) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_124ad581c8e87a79_utils_py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3_utils_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/utils.py: 0%</title>
+    <title>Coverage for src/scicom/knowledgespread/utils.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/knowledgespread/utils.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/knowledgespread/utils.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,77 +50,77 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">127 statements &nbsp;</span>
+            <span class="text">128 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">127<span class="text"> missing</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">128<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_e85bc3a05b58e6d3_run_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_baa64d8b15786095_SimpleContinuousModule_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Utility functions for initial condition generation."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">itertools</span> <span class="key">import</span> <span class="nam">combinations</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">networkx</span> <span class="key">as</span> <span class="nam">nx</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">numpy</span> <span class="key">as</span> <span class="nam">np</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">pandas</span> <span class="key">as</span> <span class="nam">pd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">numpy</span> <span class="key">as</span> <span class="nam">np</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">pandas</span> <span class="key">as</span> <span class="nam">pd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">itertools</span> <span class="key">import</span> <span class="nam">combinations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">networkx</span> <span class="key">as</span> <span class="nam">nx</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">tqdm</span> <span class="key">import</span> <span class="nam">tqdm</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">def</span> <span class="nam">epistemicRange</span><span class="op">(</span><span class="nam">baseRange</span><span class="op">,</span> <span class="nam">age</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="str">"""Return the age dependent search radius for epistemic discovery."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="str">"""Returns the age dependent search radius for epistemic discovery."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">if</span> <span class="nam">age</span> <span class="op">></span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="key">return</span> <span class="nam">baseRange</span> <span class="op">/</span> <span class="nam">age</span>  <span class="com"># Refine e.g. in direction of ageFuntion</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="key">return</span> <span class="nam">baseRange</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">def</span> <span class="nam">ageFunction</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">a</span><span class="op">,</span> <span class="nam">b</span><span class="op">,</span> <span class="nam">c</span><span class="op">,</span> <span class="nam">radius</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"""Return an age dependent radius.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">def</span> <span class="nam">ageFunction</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">a</span><span class="op">,</span> <span class="nam">b</span><span class="op">,</span> <span class="nam">c</span><span class="op">,</span> <span class="nam">radius</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"""Returns an age dependent radius.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    Bell-shaped function with center at c, slop and width</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    of plateau defined by a, b.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    Can be used to show age-dependent activity of agents. </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">if</span> <span class="nam">agent</span><span class="op">.</span><span class="nam">age</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">return</span> <span class="num">0.0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">return</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="key">return</span> <span class="nam">radius</span><span class="op">/</span><span class="op">(</span><span class="num">1</span> <span class="op">+</span> <span class="nam">abs</span><span class="op">(</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">age</span> <span class="op">-</span> <span class="nam">c</span><span class="op">)</span><span class="op">/</span><span class="op">(</span><span class="nam">a</span><span class="op">)</span><span class="op">)</span><span class="op">**</span><span class="op">(</span><span class="num">2</span><span class="op">*</span><span class="nam">b</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="key">class</span> <span class="nam">GenerateInitalPopulation</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"""Generate sets of initial conditions."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="key">class</span> <span class="nam">GenerateInitalPopulation</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"""Generate sets of initial conditions,"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">numScientists</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">timesteps</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">timesteps</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">N</span> <span class="op">=</span> <span class="nam">numScientists</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">Tstep</span> <span class="op">=</span> <span class="nam">timesteps</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">def</span> <span class="nam">epistemicFunc</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">fc</span><span class="op">,</span> <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span><span class="op">,</span> <span class="nam">beta</span><span class="op">=</span><span class="num">8</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="str">"""Epistemic space initial sampling."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">if</span> <span class="nam">fc</span> <span class="op">==</span> <span class="str">"complex"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -137,61 +137,61 @@
     <p class="mis show_mis"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">elif</span> <span class="nam">fcT</span> <span class="op">==</span> <span class="str">"linear"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">n2step</span> <span class="op">=</span> <span class="nam">slope</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">elif</span> <span class="nam">fcT</span> <span class="op">==</span> <span class="str">"exponential"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">n2step</span> <span class="op">=</span> <span class="nam">base</span> <span class="op">**</span> <span class="nam">step</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="nam">dft</span> <span class="op">=</span> <span class="nam">dataframe</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                <span class="nam">n2step</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">abs</span><span class="op">(</span><span class="nam">dataframe</span><span class="op">.</span><span class="nam">z</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">abs</span><span class="op">(</span><span class="nam">dataframe</span><span class="op">.</span><span class="nam">z</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="key">return</span> <span class="nam">dft</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">except</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Your sample size is larger then the data. Adjust exponential time."</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="key">raise</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">def</span> <span class="nam">sample</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">fcE</span><span class="op">=</span><span class="str">"complex"</span><span class="op">,</span> <span class="nam">fcT</span><span class="op">=</span><span class="str">"saturate"</span><span class="op">,</span> <span class="nam">beta</span><span class="op">=</span><span class="num">8</span><span class="op">,</span> <span class="nam">slope</span><span class="op">=</span><span class="num">5</span><span class="op">,</span> <span class="nam">base</span><span class="op">=</span><span class="num">5</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="str">"""Generate the sample population and add activation time."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">dta</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_fullDist</span><span class="op">(</span><span class="nam">fcE</span><span class="op">=</span><span class="nam">fcE</span><span class="op">,</span> <span class="nam">beta</span><span class="op">=</span><span class="nam">beta</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">initial_population</span> <span class="op">=</span> <span class="nam">dta</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">N</span><span class="op">,</span> <span class="nam">weights</span><span class="op">=</span><span class="nam">abs</span><span class="op">(</span><span class="nam">dta</span><span class="op">.</span><span class="nam">z</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">initial_population</span><span class="op">[</span><span class="str">"t"</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">initial_population</span><span class="op">[</span><span class="str">'t'</span><span class="op">]</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">stepDF</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">for</span> <span class="nam">step</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">Tstep</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="nam">temp</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">timeFunc</span><span class="op">(</span><span class="nam">dta</span><span class="op">,</span> <span class="nam">step</span><span class="op">,</span> <span class="nam">fcT</span><span class="op">=</span><span class="nam">fcT</span><span class="op">,</span> <span class="nam">slope</span><span class="op">=</span><span class="nam">slope</span><span class="op">,</span> <span class="nam">base</span><span class="op">=</span><span class="nam">base</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">temp</span><span class="op">[</span><span class="str">"t"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">step</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">temp</span><span class="op">[</span><span class="str">'t'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">step</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">stepDF</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">temp</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="nam">joined</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="nam">stepDF</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">initial_population</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="op">[</span><span class="nam">initial_population</span><span class="op">,</span> <span class="nam">joined</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="op">[</span><span class="nam">initial_population</span><span class="op">,</span> <span class="nam">joined</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">initial_population</span> <span class="op">=</span> <span class="nam">initial_population</span><span class="op">.</span><span class="nam">reset_index</span><span class="op">(</span><span class="nam">drop</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">initial_population</span><span class="op">[</span><span class="str">"id"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">initial_population</span><span class="op">.</span><span class="nam">index</span> <span class="op">+</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">initial_population</span><span class="op">[</span><span class="str">'id'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">initial_population</span><span class="op">.</span><span class="nam">index</span> <span class="op">+</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">return</span> <span class="nam">initial_population</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">def</span> <span class="nam">_fullDist</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">fcE</span><span class="op">,</span> <span class="nam">beta</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="str">"""Full distribution to sample from."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="nam">x</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">linspace</span><span class="op">(</span><span class="op">-</span><span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">10000</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="nam">y</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">linspace</span><span class="op">(</span><span class="op">-</span><span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">10000</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">X</span><span class="op">,</span> <span class="nam">Y</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">meshgrid</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">Z</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">epistemicFunc</span><span class="op">(</span><span class="nam">fcE</span><span class="op">,</span> <span class="nam">X</span><span class="op">,</span> <span class="nam">Y</span><span class="op">,</span> <span class="nam">beta</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">dta</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="op">{</span><span class="str">"x"</span><span class="op">:</span> <span class="nam">X</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"y"</span><span class="op">:</span> <span class="nam">Y</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"z"</span><span class="op">:</span> <span class="nam">Z</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="op">{</span><span class="str">'x'</span><span class="op">:</span> <span class="nam">X</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">'y'</span><span class="op">:</span> <span class="nam">Y</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">'z'</span><span class="op">:</span> <span class="nam">Z</span><span class="op">.</span><span class="nam">flatten</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">return</span> <span class="nam">dta</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="key">class</span> <span class="nam">GenerateSocNet</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="key">class</span> <span class="nam">GenerateSocNet</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="nam">dataframe</span><span class="op">:</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="nam">minDist</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.0001</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="nam">minDist</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.0001</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">population</span> <span class="op">=</span> <span class="nam">dataframe</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">density</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">density</span> <span class="op">=</span> <span class="str">''</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span> <span class="op">=</span> <span class="str">''</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="str">''</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">minDist</span> <span class="op">=</span> <span class="nam">minDist</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">def</span> <span class="nam">_getWeighted</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">row</span><span class="op">,</span> <span class="nam">degree</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="key">return</span> <span class="nam">degree</span><span class="op">[</span><span class="nam">int</span><span class="op">(</span><span class="nam">row</span><span class="op">[</span><span class="str">"from_id"</span><span class="op">]</span><span class="op">)</span><span class="op">]</span> <span class="op">*</span> <span class="nam">row</span><span class="op">[</span><span class="str">"dist"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">except</span> <span class="nam">KeyError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
@@ -207,26 +207,26 @@
     <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">coordinateDict</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="nam">row</span><span class="op">[</span><span class="str">"id"</span><span class="op">]</span><span class="op">:</span> <span class="nam">np</span><span class="op">.</span><span class="nam">array</span><span class="op">(</span><span class="op">[</span><span class="nam">row</span><span class="op">[</span><span class="str">"x"</span><span class="op">]</span><span class="op">,</span> <span class="nam">row</span><span class="op">[</span><span class="str">"y"</span><span class="op">]</span><span class="op">,</span> <span class="nam">row</span><span class="op">[</span><span class="str">"z"</span><span class="op">]</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">ix</span><span class="op">,</span> <span class="nam">row</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">iterrows</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">idCombinations</span> <span class="op">=</span> <span class="op">[</span><span class="nam">tup</span> <span class="key">for</span> <span class="nam">tup</span> <span class="key">in</span> <span class="nam">combinations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">unique</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="num">2</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">edges</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="key">for</span> <span class="nam">combi</span> <span class="key">in</span> <span class="nam">idCombinations</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">            <span class="nam">dist</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">linalg</span><span class="op">.</span><span class="nam">norm</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="nam">coordinateDict</span><span class="op">[</span><span class="nam">combi</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">]</span> <span class="op">-</span> <span class="nam">coordinateDict</span><span class="op">[</span><span class="nam">combi</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="nam">coordinateDict</span><span class="op">[</span><span class="nam">combi</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">]</span> <span class="op">-</span> <span class="nam">coordinateDict</span><span class="op">[</span><span class="nam">combi</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">            <span class="key">if</span> <span class="nam">dist</span> <span class="op">&lt;=</span> <span class="num">0.0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                <span class="nam">dist</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">minDist</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="nam">edges</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="op">(</span><span class="nam">combi</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">combi</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">dist</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="op">(</span><span class="nam">combi</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">combi</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">dist</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span><span class="nam">edges</span><span class="op">,</span> <span class="nam">columns</span><span class="op">=</span><span class="op">[</span><span class="str">"from_id"</span><span class="op">,</span> <span class="str">"to_id"</span><span class="op">,</span> <span class="str">"dist"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">social_net</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">"from_id.isin(@first_gen) and to_id.isin(@first_gen)"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">social_net_sample</span> <span class="op">=</span> <span class="nam">social_net</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">            <span class="nam">round</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">density</span> <span class="op">*</span> <span class="op">(</span><span class="nam">initPopN</span> <span class="op">*</span> <span class="op">(</span><span class="nam">initPopN</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">/</span> <span class="num">2</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">            <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">social_net</span><span class="op">.</span><span class="nam">dist</span><span class="op">)</span> <span class="op">/</span> <span class="nam">social_net</span><span class="op">.</span><span class="nam">dist</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">            <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">social_net</span><span class="op">.</span><span class="nam">dist</span><span class="op">)</span> <span class="op">/</span> <span class="nam">social_net</span><span class="op">.</span><span class="nam">dist</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">social_net_sample</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"time"</span><span class="op">,</span> <span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="nam">social_net_sample</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="key">return</span> <span class="nam">social_net_sample</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">    <span class="key">def</span> <span class="nam">growNodes</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">time</span><span class="op">,</span> <span class="nam">nEdges</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="str">"""Add nodes with weighted preferential attachment.</span>&nbsp;</span><span class="r"></span></p>
@@ -238,105 +238,106 @@
     <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">        select N edges for each new agent.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">        Return the concatenated new edges</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">addedEdges</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="nam">oldIDs</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">"t &lt; @time"</span><span class="op">)</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">unique</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="key">for</span> <span class="nam">newID</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">"t == @time"</span><span class="op">)</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">unique</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="nam">potEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="str">"from_id == @newID or to_id == @newID"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="str">"from_id == @newID or to_id == @newID"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">            <span class="op">)</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                <span class="str">"from_id.isin(@oldIDs) or to_id.isin(@oldIDs)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                <span class="str">"from_id.isin(@oldIDs) or to_id.isin(@oldIDs)"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="nam">socialGraph</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">from_pandas_edgelist</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">                <span class="nam">source</span><span class="op">=</span><span class="str">"from_id"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">                <span class="nam">target</span><span class="op">=</span><span class="str">"to_id"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">                <span class="nam">target</span><span class="op">=</span><span class="str">"to_id"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">degree</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">degree</span><span class="op">(</span><span class="nam">socialGraph</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="nam">degreeDict</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">degree</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="nam">weightedDist</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">apply</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                <span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_getWeighted</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">degreeDict</span><span class="op">)</span><span class="op">,</span> <span class="nam">axis</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                <span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_getWeighted</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">degreeDict</span><span class="op">)</span><span class="op">,</span> <span class="nam">axis</span><span class="op">=</span><span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">            <span class="nam">potEdges</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                <span class="num">0</span><span class="op">,</span> <span class="str">"weighted"</span><span class="op">,</span> <span class="nam">weightedDist</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                <span class="num">0</span><span class="op">,</span> <span class="str">"weighted"</span><span class="op">,</span> <span class="nam">weightedDist</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="nam">potEdges</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">dropna</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">            <span class="nam">sample</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                <span class="nam">nEdges</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">)</span> <span class="op">/</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">)</span> <span class="op">/</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="nam">sample</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"time"</span><span class="op">,</span> <span class="nam">time</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="nam">addedEdges</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">sample</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="key">return</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="nam">addedEdges</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">    <span class="key">def</span> <span class="nam">growEdges</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">time</span><span class="op">,</span> <span class="nam">density</span><span class="op">,</span> <span class="nam">densityGrowth</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="str">"""Add edges with weighted preferential attachement.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t"><span class="str">        For a given time, select the current social network,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="str">        including newly added nodes. Add weights by current </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="str">        degree and distances. </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="str">        Sample a suffiecient number of edges to keep density</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="str">        at a given level. </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="nam">curSocEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">"time &lt;= time"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="nam">curSocNet</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">from_pandas_edgelist</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">            <span class="nam">curSocEdges</span><span class="op">,</span> <span class="nam">source</span><span class="op">=</span><span class="str">"from_id"</span><span class="op">,</span> <span class="nam">target</span><span class="op">=</span><span class="str">"to_id"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">        <span class="nam">edges2add</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_nodes</span><span class="op">(</span><span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_nodes</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">/</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="nam">density</span> <span class="op">+</span> <span class="nam">densityGrowth</span> <span class="op">*</span> <span class="nam">time</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">        <span class="op">)</span> <span class="op">-</span> <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_edges</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">from_degree</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">            <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">degree</span><span class="op">,</span> <span class="nam">columns</span><span class="op">=</span><span class="op">[</span><span class="str">"from_id"</span><span class="op">,</span> <span class="str">"from_degree"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="nam">to_degree</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">            <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">degree</span><span class="op">,</span> <span class="nam">columns</span><span class="op">=</span><span class="op">[</span><span class="str">"to_id"</span><span class="op">,</span> <span class="str">"to_degree"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">potEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">            <span class="nam">from_degree</span><span class="op">,</span> <span class="nam">how</span><span class="op">=</span><span class="str">"inner"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="op">)</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">            <span class="nam">to_degree</span><span class="op">,</span> <span class="nam">how</span><span class="op">=</span><span class="str">"inner"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">weights</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">from_degree</span> <span class="op">*</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">to_degree</span> <span class="op">*</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">dist</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">potEdges</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"weighted"</span><span class="op">,</span> <span class="nam">weights</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">            <span class="nam">sample</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">                <span class="nam">round</span><span class="op">(</span><span class="nam">edges2add</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">)</span> <span class="op">/</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="nam">sample</span> <span class="op">=</span> <span class="nam">sample</span><span class="op">[</span><span class="op">[</span><span class="str">"from_id"</span><span class="op">,</span> <span class="str">"to_id"</span><span class="op">,</span> <span class="str">"dist"</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">sample</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"time"</span><span class="op">,</span> <span class="nam">time</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="key">return</span> <span class="nam">sample</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">except</span> <span class="nam">ValueError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">"Failed"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="key">return</span> <span class="nam">potEdges</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">nEdges</span><span class="op">=</span><span class="num">4</span><span class="op">,</span> <span class="nam">density</span><span class="op">=</span><span class="num">0.2</span><span class="op">,</span> <span class="nam">densityGrowth</span><span class="op">=</span><span class="num">0</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">density</span> <span class="op">=</span> <span class="nam">density</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">maxT</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">t</span><span class="op">.</span><span class="nam">max</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="nam">_</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">initSocNet</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="key">for</span> <span class="nam">time</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">maxT</span> <span class="op">+</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="nam">newNodeEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">growNodes</span><span class="op">(</span><span class="nam">time</span><span class="op">,</span> <span class="nam">nEdges</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">,</span> <span class="nam">newNodeEdges</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="nam">newPrefEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">growEdges</span><span class="op">(</span><span class="nam">time</span><span class="op">,</span> <span class="nam">density</span><span class="op">,</span> <span class="nam">densityGrowth</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">,</span> <span class="nam">newPrefEdges</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="nam">curSocEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">"time &lt;= time"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="nam">curSocNet</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">from_pandas_edgelist</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="nam">curSocEdges</span><span class="op">,</span> <span class="nam">source</span><span class="op">=</span><span class="str">'from_id'</span><span class="op">,</span> <span class="nam">target</span><span class="op">=</span><span class="str">'to_id'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="nam">edges2add</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">            <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">                <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_nodes</span><span class="op">(</span><span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_nodes</span><span class="op">(</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">/</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="nam">density</span> <span class="op">+</span> <span class="nam">densityGrowth</span> <span class="op">*</span> <span class="nam">time</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="op">)</span> <span class="op">-</span> <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">number_of_edges</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="nam">from_degree</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">            <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">degree</span><span class="op">,</span> <span class="nam">columns</span><span class="op">=</span><span class="op">[</span><span class="str">'from_id'</span><span class="op">,</span> <span class="str">'from_degree'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="nam">to_degree</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="nam">curSocNet</span><span class="op">.</span><span class="nam">degree</span><span class="op">,</span> <span class="nam">columns</span><span class="op">=</span><span class="op">[</span><span class="str">'to_id'</span><span class="op">,</span> <span class="str">'to_degree'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="nam">potEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">allEdges</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">            <span class="nam">from_degree</span><span class="op">,</span> <span class="nam">how</span><span class="op">=</span><span class="str">'inner'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="op">)</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="nam">to_degree</span><span class="op">,</span> <span class="nam">how</span><span class="op">=</span><span class="str">'inner'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">weights</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">from_degree</span> <span class="op">*</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">to_degree</span> <span class="op">*</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">dist</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="nam">potEdges</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"weighted"</span><span class="op">,</span> <span class="nam">weights</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">            <span class="nam">sample</span> <span class="op">=</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">                <span class="nam">round</span><span class="op">(</span><span class="nam">edges2add</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">                <span class="nam">weights</span><span class="op">=</span><span class="nam">sum</span><span class="op">(</span><span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span><span class="op">)</span> <span class="op">/</span> <span class="nam">potEdges</span><span class="op">.</span><span class="nam">weighted</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">sample</span> <span class="op">=</span> <span class="nam">sample</span><span class="op">[</span><span class="op">[</span><span class="str">"from_id"</span><span class="op">,</span> <span class="str">"to_id"</span><span class="op">,</span> <span class="str">"dist"</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="nam">sample</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"time"</span><span class="op">,</span> <span class="nam">time</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">            <span class="key">return</span> <span class="nam">sample</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="key">except</span> <span class="nam">ValueError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">"Failed"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">            <span class="key">return</span> <span class="nam">potEdges</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">nEdges</span><span class="op">=</span><span class="num">4</span><span class="op">,</span> <span class="nam">density</span><span class="op">=</span><span class="num">0.2</span><span class="op">,</span> <span class="nam">densityGrowth</span><span class="op">=</span><span class="num">0</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">density</span> <span class="op">=</span> <span class="nam">density</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="nam">maxT</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">.</span><span class="nam">t</span><span class="op">.</span><span class="nam">max</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">_</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">initSocNet</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="key">for</span> <span class="nam">time</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">maxT</span> <span class="op">+</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="nam">newNodeEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">growNodes</span><span class="op">(</span><span class="nam">time</span><span class="op">,</span> <span class="nam">nEdges</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">,</span> <span class="nam">newNodeEdges</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">            <span class="nam">newPrefEdges</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">growEdges</span><span class="op">(</span><span class="nam">time</span><span class="op">,</span> <span class="nam">density</span><span class="op">,</span> <span class="nam">densityGrowth</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span><span class="op">,</span> <span class="nam">newPrefEdges</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNet</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_e85bc3a05b58e6d3_run_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_baa64d8b15786095_SimpleContinuousModule_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 11:45 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,58 +1,57 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-kknnoowwlleeddggeesspprreeaadd//uuttiillss..ppyy:: 00%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//kknnoowwlleeddggeesspprreeaadd//uuttiillss..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 112277 ssttaatteemmeennttss ?  00 rruunn 112277 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+********** 112288 ssttaatteemmeennttss ?  00 rruunn 112288 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
 _1"""Utility functions for initial condition generation.""" 
-_2from itertools import combinations 
-_3 
-_4import networkx as nx 
-_5import numpy as np 
-_6import pandas as pd 
+_2import numpy as np 
+_3import pandas as pd 
+_4from itertools import combinations 
+_5import networkx as nx 
+_6from tqdm import tqdm 
 _7 
 _8 
 _9def epistemicRange(baseRange, age): 
-_1_0 """Return the age dependent search radius for epistemic discovery.""" 
+_1_0 """Returns the age dependent search radius for epistemic discovery.""" 
 _1_1 if age > 0: 
 _1_2 return baseRange / age # Refine e.g. in direction of ageFuntion 
 _1_3 else: 
 _1_4 return baseRange 
 _1_5 
 _1_6 
-_1_7def ageFunction(agent, a, b, c, radius) -> float: 
-_1_8 """Return an age dependent radius. 
-_1_9 
+_1_7def ageFunction(agent, a, b, c, radius): 
+_1_8 """Returns an age dependent radius. 
+_1_9  
 _2_0 Bell-shaped function with center at c, slop and width 
 _2_1 of plateau defined by a, b. 
 _2_2 
 _2_3 Can be used to show age-dependent activity of agents.  
 _2_4 """ 
 _2_5 if agent.age == 0: 
-_2_6 return 0.0 
+_2_6 return 0 
 _2_7 else: 
 _2_8 return radius/(1 + abs((agent.age - c)/(a))**(2*b)) 
 _2_9 
 _3_0 
-_3_1class GenerateInitalPopulation: 
-_3_2 """Generate sets of initial conditions.""" 
+_3_1class GenerateInitalPopulation(): 
+_3_2 """Generate sets of initial conditions,""" 
 _3_3 
 _3_4 def __init__( 
 _3_5 self, 
 _3_6 numScientists, 
-_3_7 timesteps, 
+_3_7 timesteps 
 _3_8 ): 
 _3_9 self.N = numScientists 
 _4_0 self.Tstep = timesteps 
 _4_1 
 _4_2 def epistemicFunc(self, fc, x, y, beta=8): 
 _4_3 """Epistemic space initial sampling.""" 
 _4_4 if fc == "complex": 
@@ -69,62 +68,62 @@
 _5_5 elif fcT == "linear": 
 _5_6 n2step = slope 
 _5_7 elif fcT == "exponential": 
 _5_8 n2step = base ** step 
 _5_9 try: 
 _6_0 dft = dataframe.sample( 
 _6_1 n2step, 
-_6_2 weights=abs(dataframe.z), 
+_6_2 weights=abs(dataframe.z) 
 _6_3 ) 
 _6_4 return dft 
 _6_5 except ValueError("Your sample size is larger then the data. Adjust
 exponential time."): 
 _6_6 raise 
 _6_7 
 _6_8 def sample(self, fcE="complex", fcT="saturate", beta=8, slope=5, base=5): 
 _6_9 """Generate the sample population and add activation time.""" 
 _7_0 dta = self._fullDist(fcE=fcE, beta=beta) 
 _7_1 initial_population = dta.sample(self.N, weights=abs(dta.z)) 
-_7_2 initial_population["t"] = 0 
+_7_2 initial_population['t'] = 0 
 _7_3 stepDF = [] 
 _7_4 for step in range(1, self.Tstep + 1): 
 _7_5 temp = self.timeFunc(dta, step, fcT=fcT, slope=slope, base=base) 
-_7_6 temp["t"] = step 
+_7_6 temp['t'] = step 
 _7_7 stepDF.append(temp) 
 _7_8 joined = pd.concat(stepDF) 
 _7_9 initial_population = pd.concat( 
-_8_0 [initial_population, joined], 
+_8_0 [initial_population, joined] 
 _8_1 ) 
 _8_2 initial_population = initial_population.reset_index(drop=True) 
-_8_3 initial_population["id"] = initial_population.index + 1 
+_8_3 initial_population['id'] = initial_population.index + 1 
 _8_4 return initial_population 
 _8_5 
 _8_6 def _fullDist(self, fcE, beta): 
 _8_7 """Full distribution to sample from.""" 
 _8_8 x = np.linspace(-1, 1, 10000) 
 _8_9 y = np.linspace(-1, 1, 10000) 
 _9_0 X, Y = np.meshgrid(x, y) 
 _9_1 Z = self.epistemicFunc(fcE, X, Y, beta) 
 _9_2 dta = pd.DataFrame( 
-_9_3 {"x": X.flatten(), "y": Y.flatten(), "z": Z.flatten()}, 
+_9_3 {'x': X.flatten(), 'y': Y.flatten(), 'z': Z.flatten()} 
 _9_4 ) 
 _9_5 return dta 
 _9_6 
 _9_7 
-_9_8class GenerateSocNet: 
+_9_8class GenerateSocNet(): 
 _9_9 
 _1_0_0 def __init__( 
 _1_0_1 self, 
 _1_0_2 dataframe: pd.DataFrame, 
-_1_0_3 minDist: float = 0.0001, 
+_1_0_3 minDist: float = 0.0001 
 _1_0_4 ): 
 _1_0_5 self.population = dataframe 
-_1_0_6 self.density = "" 
-_1_0_7 self.allEdges = "" 
-_1_0_8 self.socialNet = "" 
+_1_0_6 self.density = '' 
+_1_0_7 self.allEdges = '' 
+_1_0_8 self.socialNet = '' 
 _1_0_9 self.minDist = minDist 
 _1_1_0 
 _1_1_1 def _getWeighted(self, row, degree): 
 _1_1_2 try: 
 _1_1_3 return degree[int(row["from_id"])] * row["dist"] 
 _1_1_4 except KeyError: 
 _1_1_5 return None 
@@ -142,27 +141,27 @@
 self.population.iterrows() 
 _1_2_7 } 
 _1_2_8 idCombinations = [tup for tup in combinations(self.population.id.unique(),
 2)] 
 _1_2_9 edges = [] 
 _1_3_0 for combi in idCombinations: 
 _1_3_1 dist = np.linalg.norm( 
-_1_3_2 coordinateDict[combi[0]] - coordinateDict[combi[1]], 
+_1_3_2 coordinateDict[combi[0]] - coordinateDict[combi[1]] 
 _1_3_3 ) 
 _1_3_4 if dist <= 0.0: 
 _1_3_5 dist = self.minDist 
 _1_3_6 edges.append( 
-_1_3_7 (combi[0], combi[1], dist), 
+_1_3_7 (combi[0], combi[1], dist) 
 _1_3_8 ) 
 _1_3_9 self.allEdges = pd.DataFrame(edges, columns=["from_id", "to_id", "dist"]) 
 _1_4_0 social_net = self.allEdges.query("from_id.isin(@first_gen) and to_id.isin
 (@first_gen)") 
 _1_4_1 social_net_sample = social_net.sample( 
 _1_4_2 round(self.density * (initPopN * (initPopN - 1) / 2)), 
-_1_4_3 weights=sum(social_net.dist) / social_net.dist, 
+_1_4_3 weights=sum(social_net.dist) / social_net.dist 
 _1_4_4 ) 
 _1_4_5 social_net_sample.insert(0, "time", 0) 
 _1_4_6 self.socialNet = social_net_sample 
 _1_4_7 return social_net_sample 
 _1_4_8 
 _1_4_9 def growNodes(self, time, nEdges): 
 _1_5_0 """Add nodes with weighted preferential attachment. 
@@ -174,92 +173,93 @@
 _1_5_6 select N edges for each new agent. 
 _1_5_7 Return the concatenated new edges 
 _1_5_8 """ 
 _1_5_9 addedEdges = [] 
 _1_6_0 oldIDs = self.population.query("t < @time").id.unique() 
 _1_6_1 for newID in self.population.query("t == @time").id.unique(): 
 _1_6_2 potEdges = self.allEdges.query( 
-_1_6_3 "from_id == @newID or to_id == @newID", 
+_1_6_3 "from_id == @newID or to_id == @newID" 
 _1_6_4 ).query( 
-_1_6_5 "from_id.isin(@oldIDs) or to_id.isin(@oldIDs)", 
+_1_6_5 "from_id.isin(@oldIDs) or to_id.isin(@oldIDs)" 
 _1_6_6 ) 
 _1_6_7 socialGraph = nx.from_pandas_edgelist( 
 _1_6_8 self.socialNet, 
 _1_6_9 source="from_id", 
-_1_7_0 target="to_id", 
+_1_7_0 target="to_id" 
 _1_7_1 ) 
 _1_7_2 
 _1_7_3 degree = nx.degree(socialGraph) 
 _1_7_4 degreeDict = dict(degree) 
 _1_7_5 
 _1_7_6 weightedDist = potEdges.apply( 
-_1_7_7 lambda x: self._getWeighted(x, degreeDict), axis=1, 
+_1_7_7 lambda x: self._getWeighted(x, degreeDict), axis=1 
 _1_7_8 ) 
 _1_7_9 potEdges.insert( 
-_1_8_0 0, "weighted", weightedDist, 
+_1_8_0 0, "weighted", weightedDist 
 _1_8_1 ) 
 _1_8_2 
 _1_8_3 potEdges = potEdges.dropna() 
 _1_8_4 sample = potEdges.sample( 
 _1_8_5 nEdges, 
-_1_8_6 weights=sum(potEdges.weighted) / potEdges.weighted, 
+_1_8_6 weights=sum(potEdges.weighted) / potEdges.weighted 
 _1_8_7 ) 
 _1_8_8 sample.insert(0, "time", time) 
 _1_8_9 addedEdges.append(sample) 
 _1_9_0 return pd.concat(addedEdges) 
 _1_9_1 
 _1_9_2 def growEdges(self, time, density, densityGrowth): 
 _1_9_3 """Add edges with weighted preferential attachement. 
 _1_9_4  
 _1_9_5 For a given time, select the current social network, 
 _1_9_6 including newly added nodes. Add weights by current  
 _1_9_7 degree and distances.  
 _1_9_8 Sample a suffiecient number of edges to keep density 
 _1_9_9 at a given level.  
 _2_0_0 """ 
-_2_0_1 curSocEdges = self.socialNet.query("time <= time") 
-_2_0_2 curSocNet = nx.from_pandas_edgelist( 
-_2_0_3 curSocEdges, source="from_id", target="to_id", 
-_2_0_4 ) 
-_2_0_5 edges2add = ( 
-_2_0_6 ( 
-_2_0_7 curSocNet.number_of_nodes() * (curSocNet.number_of_nodes() - 1) / 2 
-_2_0_8 ) * (density + densityGrowth * time) 
-_2_0_9 ) - curSocNet.number_of_edges() 
-_2_1_0 from_degree = pd.DataFrame( 
-_2_1_1 curSocNet.degree, columns=["from_id", "from_degree"], 
-_2_1_2 ) 
-_2_1_3 to_degree = pd.DataFrame( 
-_2_1_4 curSocNet.degree, columns=["to_id", "to_degree"], 
-_2_1_5 ) 
-_2_1_6 potEdges = self.allEdges.merge( 
-_2_1_7 from_degree, how="inner", 
-_2_1_8 ).merge( 
-_2_1_9 to_degree, how="inner", 
-_2_2_0 ) 
-_2_2_1 weights = potEdges.from_degree * potEdges.to_degree * potEdges.dist 
-_2_2_2 potEdges.insert(0, "weighted", weights) 
-_2_2_3 try: 
-_2_2_4 sample = potEdges.sample( 
-_2_2_5 round(edges2add), 
-_2_2_6 weights=sum(potEdges.weighted) / potEdges.weighted, 
-_2_2_7 ) 
-_2_2_8 sample = sample[["from_id", "to_id", "dist"]] 
-_2_2_9 sample.insert(0, "time", time) 
-_2_3_0 return sample 
-_2_3_1 except ValueError: 
-_2_3_2 print("Failed") 
-_2_3_3 return potEdges 
-_2_3_4 
-_2_3_5 def run(self, nEdges=4, density=0.2, densityGrowth=0): 
-_2_3_6 self.density = density 
-_2_3_7 maxT = self.population.t.max() 
-_2_3_8 _ = self.initSocNet() 
-_2_3_9 for time in range(1, maxT + 1, 1): 
-_2_4_0 newNodeEdges = self.growNodes(time, nEdges) 
-_2_4_1 self.socialNet = pd.concat([self.socialNet, newNodeEdges]) 
-_2_4_2 newPrefEdges = self.growEdges(time, density, densityGrowth) 
-_2_4_3 self.socialNet = pd.concat([self.socialNet, newPrefEdges]) 
-_2_4_4 return self.socialNet 
-_2_4_5 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 11:45 +0200
+_2_0_1 
+_2_0_2 curSocEdges = self.socialNet.query("time <= time") 
+_2_0_3 curSocNet = nx.from_pandas_edgelist( 
+_2_0_4 curSocEdges, source='from_id', target='to_id' 
+_2_0_5 ) 
+_2_0_6 edges2add = ( 
+_2_0_7 ( 
+_2_0_8 curSocNet.number_of_nodes() * (curSocNet.number_of_nodes() - 1) / 2 
+_2_0_9 ) * (density + densityGrowth * time) 
+_2_1_0 ) - curSocNet.number_of_edges() 
+_2_1_1 from_degree = pd.DataFrame( 
+_2_1_2 curSocNet.degree, columns=['from_id', 'from_degree'] 
+_2_1_3 ) 
+_2_1_4 to_degree = pd.DataFrame( 
+_2_1_5 curSocNet.degree, columns=['to_id', 'to_degree'] 
+_2_1_6 ) 
+_2_1_7 potEdges = self.allEdges.merge( 
+_2_1_8 from_degree, how='inner' 
+_2_1_9 ).merge( 
+_2_2_0 to_degree, how='inner' 
+_2_2_1 ) 
+_2_2_2 weights = potEdges.from_degree * potEdges.to_degree * potEdges.dist 
+_2_2_3 potEdges.insert(0, "weighted", weights) 
+_2_2_4 try: 
+_2_2_5 sample = potEdges.sample( 
+_2_2_6 round(edges2add), 
+_2_2_7 weights=sum(potEdges.weighted) / potEdges.weighted 
+_2_2_8 ) 
+_2_2_9 sample = sample[["from_id", "to_id", "dist"]] 
+_2_3_0 sample.insert(0, "time", time) 
+_2_3_1 return sample 
+_2_3_2 except ValueError: 
+_2_3_3 print("Failed") 
+_2_3_4 return potEdges 
+_2_3_5 
+_2_3_6 def run(self, nEdges=4, density=0.2, densityGrowth=0): 
+_2_3_7 self.density = density 
+_2_3_8 maxT = self.population.t.max() 
+_2_3_9 _ = self.initSocNet() 
+_2_4_0 for time in range(1, maxT + 1, 1): 
+_2_4_1 newNodeEdges = self.growNodes(time, nEdges) 
+_2_4_2 self.socialNet = pd.concat([self.socialNet, newNodeEdges]) 
+_2_4_3 newPrefEdges = self.growEdges(time, density, densityGrowth) 
+_2_4_4 self.socialNet = pd.concat([self.socialNet, newPrefEdges]) 
+_2_4_5 return self.socialNet 
+_2_4_6 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_22d2582a602e487e___init___py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_e5ea8e3c7b0425c3___init___py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/utilities/__init__.py: 100%</title>
+    <title>Coverage for src/scicom/knowledgespread/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/utilities/__init__.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/knowledgespread/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,42 +56,42 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_e85bc3a05b58e6d3_run_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_22d2582a602e487e_statistics_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_e85bc3a05b58e6d3_run_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_22d2582a602e487e_statistics_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_e5ea8e3c7b0425c3_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_e5ea8e3c7b0425c3_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//uuttiilliittiieess//
-____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//kknnoowwlleeddggeesspprreeaadd//____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_22d2582a602e487e_statistics_py.html` & `scicom-0.4.0/tests/reports/html/d_3142edd200b00bad_prune_py.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/utilities/statistics.py: 100%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/utilities/prune.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/utilities/statistics.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/utilities/prune.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,209 +56,191 @@
         <h2>
             <span class="text">57 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">57<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_22d2582a602e487e___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_3142edd200b00bad___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_3142edd200b00bad_statistics_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-19 14:00 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Prune a network."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">igraph</span> <span class="key">as</span> <span class="nam">ig</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">numpy</span> <span class="key">as</span> <span class="nam">np</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">pandas</span> <span class="key">as</span> <span class="nam">pd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">numpy</span> <span class="key">as</span> <span class="nam">np</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">pandas</span> <span class="key">as</span> <span class="nam">pd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">igraph</span> <span class="key">as</span> <span class="nam">ig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">tqdm</span> <span class="key">import</span> <span class="nam">tqdm</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">class</span> <span class="nam">PruneNetwork</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="str">"""Create statistics for communication networks by deletion.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    For a given dataset with sender and receiver information,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    create a weighted network with igraph. For a given number</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    of iterations, deletion amounts, and deletion types, the</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    algorithm then generates network statistics for randomly</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    sampled subnetworks.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">dataframe</span><span class="op">:</span><span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">"""Initialize pruning."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">PruneNetwork</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""Create statistics for communication networks by deletion.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    For a given dataset with sender and receiver information, </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    create a weighted network with igraph. For a given number </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    of iterations, deletion amounts, and deletion types, the </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    algorithm then generates network statistics for randomly</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    sampled subnetworks. </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">dataframe</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">inputDF</span> <span class="op">=</span> <span class="nam">dataframe</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">def</span> <span class="nam">makeNet</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">dataframe</span><span class="op">:</span><span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ig</span><span class="op">.</span><span class="nam">Graph</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">def</span> <span class="nam">makeNet</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">dataframe</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""Create network from dataframe.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">        Assumes the existence of sender, receiver and step</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        column names.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        column names. </span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">networkdata</span> <span class="op">=</span> <span class="nam">dataframe</span><span class="op">[</span><span class="op">[</span><span class="str">"sender"</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="str">"step"</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">networkdata</span> <span class="op">=</span> <span class="nam">networkdata</span><span class="op">.</span><span class="nam">groupby</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="op">[</span><span class="str">"sender"</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="op">)</span><span class="op">.</span><span class="nam">size</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">reset_index</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"Count"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="key">return</span> <span class="nam">ig</span><span class="op">.</span><span class="nam">Graph</span><span class="op">.</span><span class="nam">TupleList</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="nam">networkdata</span><span class="op">.</span><span class="nam">itertuples</span><span class="op">(</span><span class="nam">index</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span> <span class="nam">directed</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">weights</span><span class="op">=</span><span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">df</span> <span class="op">=</span> <span class="nam">dataframe</span><span class="op">[</span><span class="op">[</span><span class="str">'sender'</span><span class="op">,</span> <span class="str">'receiver'</span><span class="op">,</span> <span class="str">'step'</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">df</span> <span class="op">=</span> <span class="nam">df</span><span class="op">.</span><span class="nam">groupby</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="op">[</span><span class="str">'sender'</span><span class="op">,</span> <span class="str">'receiver'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="op">)</span><span class="op">.</span><span class="nam">size</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">reset_index</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">'Count'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">net</span> <span class="op">=</span> <span class="nam">ig</span><span class="op">.</span><span class="nam">Graph</span><span class="op">.</span><span class="nam">TupleList</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="nam">df</span><span class="op">.</span><span class="nam">itertuples</span><span class="op">(</span><span class="nam">index</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">,</span> <span class="nam">directed</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">weights</span><span class="op">=</span><span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">def</span> <span class="nam">netStats</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">G</span><span class="op">:</span><span class="nam">ig</span><span class="op">.</span><span class="nam">Graph</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="str">"""Generate network statistics.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">        Any statistic calculated on the full</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        network can be added in principle.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        Currently implemented are:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        average relative degree,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        density</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">        transitivtiy</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">        cohesion</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">        average path length</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">        modularity</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="nam">numVs</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="nam">avg_rel_deg</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">mean</span><span class="op">(</span><span class="op">[</span><span class="nam">x</span><span class="op">/</span><span class="nam">numVs</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">G</span><span class="op">.</span><span class="nam">degree</span><span class="op">(</span><span class="nam">mode</span><span class="op">=</span><span class="str">"all"</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">density</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">density</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">transitivity</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">transitivity_undirected</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">cohesion</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">cohesion</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">avg_path_len</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">average_path_length</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">modularity</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">modularity</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">components</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">return</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">                    <span class="str">"avg_relative_degree"</span><span class="op">:</span> <span class="nam">avg_rel_deg</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">                    <span class="str">"avg_path_length"</span><span class="op">:</span> <span class="nam">avg_path_len</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">                    <span class="str">"density"</span><span class="op">:</span> <span class="nam">density</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                    <span class="str">"transitivity"</span><span class="op">:</span> <span class="nam">transitivity</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                    <span class="str">"cohesion"</span><span class="op">:</span> <span class="nam">cohesion</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">                    <span class="str">"modularity"</span><span class="op">:</span> <span class="nam">modularity</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">                <span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">def</span> <span class="nam">generatePruningParameters</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">G</span><span class="op">:</span><span class="nam">ig</span><span class="op">.</span><span class="nam">Graph</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="str">"""Generate a random set of pruning weights."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">nodes</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_vertex_dataframe</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">id2name</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_vertex_dataframe</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">to_dict</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"name"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">rng</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">default_rng</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">del_parameter</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">            <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">                <span class="str">"ids"</span><span class="op">:</span> <span class="nam">nodes</span><span class="op">.</span><span class="nam">index</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">                <span class="str">"degree"</span><span class="op">:</span> <span class="nam">G</span><span class="op">.</span><span class="nam">degree</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">                <span class="str">"unif"</span><span class="op">:</span> <span class="nam">rng</span><span class="op">.</span><span class="nam">uniform</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">                <span class="str">"log_normal"</span><span class="op">:</span> <span class="nam">rng</span><span class="op">.</span><span class="nam">lognormal</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">                <span class="str">"exp"</span><span class="op">:</span> <span class="nam">rng</span><span class="op">.</span><span class="nam">exponential</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">                <span class="str">"beta"</span><span class="op">:</span> <span class="nam">rng</span><span class="op">.</span><span class="nam">beta</span><span class="op">(</span><span class="nam">a</span><span class="op">=</span><span class="num">2</span><span class="op">,</span> <span class="nam">b</span><span class="op">=</span><span class="num">3</span><span class="op">,</span> <span class="nam">size</span><span class="op">=</span><span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">del_parameter</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_edge_dataframe</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="op">[</span><span class="str">"source"</span><span class="op">,</span> <span class="str">"target"</span><span class="op">]</span><span class="op">]</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">,</span> <span class="nam">left_on</span><span class="op">=</span><span class="str">"source"</span><span class="op">,</span> <span class="nam">right_on</span><span class="op">=</span><span class="str">"ids"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="op">)</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">,</span> <span class="nam">left_on</span><span class="op">=</span><span class="str">"target"</span><span class="op">,</span> <span class="nam">right_on</span><span class="op">=</span><span class="str">"ids"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"degree"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_y</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"unif"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_y</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"log_normal"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_y</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"exp"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_y</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"beta"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_y</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">sender</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"source"</span><span class="op">]</span><span class="op">.</span><span class="nam">apply</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">id2name</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">receiver</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"target"</span><span class="op">]</span><span class="op">.</span><span class="nam">apply</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">id2name</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"sender"</span><span class="op">,</span> <span class="nam">sender</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="nam">receiver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="key">return</span> <span class="nam">del_parameter</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">            <span class="op">[</span><span class="str">"sender"</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="str">"degree"</span><span class="op">,</span> <span class="str">"unif"</span><span class="op">,</span> <span class="str">"log_normal"</span><span class="op">,</span> <span class="str">"exp"</span><span class="op">,</span> <span class="str">"beta"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="key">def</span> <span class="nam">deleteFromNetwork</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">iterations</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">delAmounts</span><span class="op">:</span> <span class="nam">tuple</span> <span class="op">=</span> <span class="op">(</span><span class="num">0.1</span><span class="op">,</span> <span class="num">0.25</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.75</span><span class="op">,</span> <span class="num">0.9</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">delTypes</span><span class="op">:</span> <span class="nam">tuple</span> <span class="op">=</span> <span class="op">(</span><span class="str">"degree"</span><span class="op">,</span> <span class="str">"unif"</span><span class="op">,</span> <span class="str">"log_normal"</span><span class="op">,</span> <span class="str">"exp"</span><span class="op">,</span> <span class="str">"beta"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="str">"""Run the deletion by sampling."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">results</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">fullNet</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">makeNet</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">inputDF</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">fullStats</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">netStats</span><span class="op">(</span><span class="nam">fullNet</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">fullStats</span> <span class="op">=</span> <span class="nam">fullStats</span><span class="op">.</span><span class="nam">assign</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="nam">delVal</span><span class="op">=</span><span class="num">0</span><span class="op">,</span> <span class="nam">delType</span><span class="op">=</span><span class="str">"NA"</span><span class="op">,</span> <span class="nam">delIteration</span><span class="op">=</span><span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">results</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">fullStats</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">iterations</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">            <span class="nam">prunVals</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generatePruningParameters</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                <span class="nam">fullNet</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">            <span class="nam">tempDF</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">inputDF</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                <span class="nam">prunVals</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="key">for</span> <span class="nam">val</span> <span class="key">in</span> <span class="nam">list</span><span class="op">(</span><span class="nam">delAmounts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="key">for</span> <span class="nam">deltype</span> <span class="key">in</span> <span class="nam">list</span><span class="op">(</span><span class="nam">delTypes</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                    <span class="nam">delDF</span> <span class="op">=</span> <span class="nam">tempDF</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                        <span class="nam">round</span><span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">tempDF</span><span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="num">1</span> <span class="op">-</span> <span class="nam">val</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                        <span class="nam">weights</span><span class="op">=</span><span class="nam">deltype</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                    <span class="nam">delNet</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">makeNet</span><span class="op">(</span><span class="nam">delDF</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                    <span class="nam">delStats</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">netStats</span><span class="op">(</span><span class="nam">delNet</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                    <span class="nam">delStats</span> <span class="op">=</span> <span class="nam">delStats</span><span class="op">.</span><span class="nam">assign</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                        <span class="nam">delVal</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">delType</span><span class="op">=</span><span class="nam">deltype</span><span class="op">,</span> <span class="nam">delIteration</span><span class="op">=</span><span class="nam">idx</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                    <span class="nam">results</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">delStats</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">return</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="nam">results</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">return</span> <span class="nam">net</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">def</span> <span class="nam">netStats</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">G</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="str">"""Generate network statistics.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        Any statistic calculated on the full</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        network can be added in principle.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        Currently implemented are: </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        average relative degree,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">        density</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">        transitivtiy</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">        cohesion</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">        average path length</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        modularity</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="nam">numVs</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">avg_rel_deg</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">mean</span><span class="op">(</span><span class="op">[</span><span class="nam">x</span><span class="op">/</span><span class="nam">numVs</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">G</span><span class="op">.</span><span class="nam">degree</span><span class="op">(</span><span class="nam">mode</span><span class="op">=</span><span class="str">"all"</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">density</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">density</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">transitivity</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">transitivity_undirected</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">cohesion</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">cohesion</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">avg_path_len</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">average_path_length</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">modularity</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">modularity</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">components</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">statDF</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">                <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">                    <span class="str">'avg_relative_degree'</span><span class="op">:</span> <span class="nam">avg_rel_deg</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">                    <span class="str">'avg_path_length'</span><span class="op">:</span> <span class="nam">avg_path_len</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">                    <span class="str">'density'</span><span class="op">:</span> <span class="nam">density</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">                    <span class="str">'transitivity'</span><span class="op">:</span> <span class="nam">transitivity</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">                    <span class="str">'cohesion'</span><span class="op">:</span> <span class="nam">cohesion</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">                    <span class="str">'modularity'</span><span class="op">:</span> <span class="nam">modularity</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">                <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="key">return</span> <span class="nam">statDF</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">def</span> <span class="nam">generatePruningParameters</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">G</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="str">"""Generate a random set of pruning weights."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">nodes</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_vertex_dataframe</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">id2name</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_vertex_dataframe</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">to_dict</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">'name'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">del_parameter</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">                <span class="str">'ids'</span><span class="op">:</span> <span class="nam">nodes</span><span class="op">.</span><span class="nam">index</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">                <span class="str">'degree'</span><span class="op">:</span> <span class="nam">G</span><span class="op">.</span><span class="nam">degree</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">                <span class="str">'unif'</span><span class="op">:</span> <span class="nam">np</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">uniform</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">                <span class="str">'log_normal'</span><span class="op">:</span> <span class="nam">np</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">lognormal</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">                <span class="str">'exp'</span><span class="op">:</span> <span class="nam">np</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">exponential</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">                <span class="str">'beta'</span><span class="op">:</span> <span class="nam">np</span><span class="op">.</span><span class="nam">random</span><span class="op">.</span><span class="nam">beta</span><span class="op">(</span><span class="nam">a</span><span class="op">=</span><span class="num">2</span><span class="op">,</span> <span class="nam">b</span><span class="op">=</span><span class="num">3</span><span class="op">,</span> <span class="nam">size</span><span class="op">=</span><span class="nam">len</span><span class="op">(</span><span class="nam">G</span><span class="op">.</span><span class="nam">vs</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">del_parameter</span> <span class="op">=</span> <span class="nam">G</span><span class="op">.</span><span class="nam">get_edge_dataframe</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="op">[</span><span class="str">"source"</span><span class="op">,</span> <span class="str">"target"</span><span class="op">]</span><span class="op">]</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">,</span> <span class="nam">left_on</span><span class="op">=</span><span class="str">'source'</span><span class="op">,</span> <span class="nam">right_on</span><span class="op">=</span><span class="str">'ids'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="op">)</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">            <span class="nam">del_parameter</span><span class="op">,</span> <span class="nam">left_on</span><span class="op">=</span><span class="str">'target'</span><span class="op">,</span> <span class="nam">right_on</span><span class="op">=</span><span class="str">'ids'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">'degree'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span><span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">degree_y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">'unif'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span><span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">unif_y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">'log_normal'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span><span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">log_normal_y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">'exp'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span><span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">exp_y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">[</span><span class="str">'beta'</span><span class="op">]</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_x</span> <span class="op">*</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_y</span> <span class="op">/</span> <span class="nam">np</span><span class="op">.</span><span class="nam">dot</span><span class="op">(</span><span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_x</span><span class="op">,</span> <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">beta_y</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">sender</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"source"</span><span class="op">]</span><span class="op">.</span><span class="nam">apply</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">id2name</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">receiver</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">[</span><span class="str">"target"</span><span class="op">]</span><span class="op">.</span><span class="nam">apply</span><span class="op">(</span><span class="key">lambda</span> <span class="nam">x</span><span class="op">:</span> <span class="nam">id2name</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"sender"</span><span class="op">,</span> <span class="nam">sender</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">del_parameter</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="nam">receiver</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">outDF</span> <span class="op">=</span> <span class="nam">del_parameter</span><span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">            <span class="op">[</span><span class="str">'sender'</span><span class="op">,</span> <span class="str">'receiver'</span><span class="op">,</span> <span class="str">'degree'</span><span class="op">,</span> <span class="str">'unif'</span><span class="op">,</span> <span class="str">'log_normal'</span><span class="op">,</span> <span class="str">'exp'</span><span class="op">,</span> <span class="str">'beta'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">return</span> <span class="nam">outDF</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="key">def</span> <span class="nam">deleteFromNetwork</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">iterations</span><span class="op">=</span><span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">delAmounts</span><span class="op">=</span><span class="op">(</span><span class="num">0.1</span><span class="op">,</span> <span class="num">0.25</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.75</span><span class="op">,</span> <span class="num">0.9</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">delTypes</span><span class="op">=</span><span class="op">(</span><span class="str">"degree"</span><span class="op">,</span> <span class="str">"unif"</span><span class="op">,</span> <span class="str">"log_normal"</span><span class="op">,</span> <span class="str">"exp"</span><span class="op">,</span> <span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="str">"""Run the deletion by sampling."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="nam">results</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="nam">fullNet</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">makeNet</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">inputDF</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">fullStats</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">netStats</span><span class="op">(</span><span class="nam">fullNet</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">fullStats</span> <span class="op">=</span> <span class="nam">fullStats</span><span class="op">.</span><span class="nam">assign</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="op">**</span><span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                <span class="str">"delVal"</span><span class="op">:</span> <span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="str">"delType"</span><span class="op">:</span> <span class="str">'NA'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="str">"delIteration"</span><span class="op">:</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="nam">results</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">fullStats</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="nam">iterations</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="nam">prunVals</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">generatePruningParameters</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                <span class="nam">fullNet</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="nam">tempDF</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">inputDF</span><span class="op">.</span><span class="nam">merge</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="nam">prunVals</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">            <span class="key">for</span> <span class="nam">val</span> <span class="key">in</span> <span class="nam">list</span><span class="op">(</span><span class="nam">delAmounts</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="key">for</span> <span class="nam">deltype</span> <span class="key">in</span> <span class="nam">list</span><span class="op">(</span><span class="nam">delTypes</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                    <span class="nam">delDF</span> <span class="op">=</span> <span class="nam">tempDF</span><span class="op">.</span><span class="nam">sample</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                        <span class="nam">round</span><span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">tempDF</span><span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="num">1</span> <span class="op">-</span> <span class="nam">val</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                        <span class="nam">weights</span><span class="op">=</span><span class="nam">deltype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                    <span class="nam">delNet</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">makeNet</span><span class="op">(</span><span class="nam">delDF</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                    <span class="nam">delStats</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">netStats</span><span class="op">(</span><span class="nam">delNet</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                    <span class="nam">delStats</span> <span class="op">=</span> <span class="nam">delStats</span><span class="op">.</span><span class="nam">assign</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                        <span class="op">**</span><span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                            <span class="str">"delVal"</span><span class="op">:</span> <span class="nam">val</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                            <span class="str">"delType"</span><span class="op">:</span> <span class="nam">deltype</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                            <span class="str">"delIteration"</span><span class="op">:</span> <span class="nam">idx</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                    <span class="nam">results</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">delStats</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="nam">resDF</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">concat</span><span class="op">(</span><span class="nam">results</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">return</span> <span class="nam">resDF</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="key">def</span> <span class="nam">prune</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="nam">modelparameters</span><span class="op">:</span> <span class="nam">dict</span><span class="op">,</span> <span class="nam">network</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">,</span> <span class="nam">columns</span><span class="op">:</span> <span class="nam">list</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="nam">iterations</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">10</span><span class="op">,</span> <span class="nam">delAmounts</span><span class="op">:</span> <span class="nam">tuple</span> <span class="op">=</span> <span class="op">(</span><span class="num">0.1</span><span class="op">,</span> <span class="num">0.25</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.75</span><span class="op">,</span> <span class="num">0.9</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="nam">delTypes</span><span class="op">:</span> <span class="nam">tuple</span> <span class="op">=</span> <span class="op">(</span><span class="str">"degree"</span><span class="op">,</span> <span class="str">"unif"</span><span class="op">)</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="str">"""Generate pruned networks from input.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">    Assumes existence of columns "sender", "receiver", and "step".</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">    <span class="nam">runDf</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span><span class="nam">network</span><span class="op">,</span> <span class="nam">columns</span> <span class="op">=</span> <span class="nam">columns</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="nam">pruning</span> <span class="op">=</span> <span class="nam">PruneNetwork</span><span class="op">(</span><span class="nam">runDf</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">pruning</span><span class="op">.</span><span class="nam">deleteFromNetwork</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="nam">iterations</span><span class="op">=</span><span class="nam">iterations</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="nam">delAmounts</span><span class="op">=</span><span class="nam">delAmounts</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">delTypes</span><span class="op">=</span><span class="nam">delTypes</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">assign</span><span class="op">(</span><span class="op">**</span><span class="nam">modelparameters</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_22d2582a602e487e___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_3142edd200b00bad___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_3142edd200b00bad_statistics_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-19 14:00 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,187 +1,171 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//uuttiilliittiieess//
-ssttaattiissttiiccss..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//uuttiilliittiieess//
+pprruunnee..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5577 ssttaatteemmeennttss ?  5577 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
-_1"""Prune a network.""" 
-_2import igraph as ig 
-_3import numpy as np 
-_4import pandas as pd 
-_5 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+19 14:00 +0200
+_1import os 
+_2import numpy as np 
+_3import pandas as pd 
+_4import igraph as ig 
+_5from tqdm import tqdm 
 _6 
-_7class PruneNetwork: 
-_8 """Create statistics for communication networks by deletion. 
-_9 
-_1_0 For a given dataset with sender and receiver information, 
-_1_1 create a weighted network with igraph. For a given number 
-_1_2 of iterations, deletion amounts, and deletion types, the 
-_1_3 algorithm then generates network statistics for randomly 
-_1_4 sampled subnetworks. 
-_1_5 """ 
-_1_6 
-_1_7 def __init__(self, dataframe:pd.DataFrame) -> None: 
-_1_8 """Initialize pruning.""" 
+_7 
+_8class PruneNetwork(): 
+_9 """Create statistics for communication networks by deletion. 
+_1_0 
+_1_1 For a given dataset with sender and receiver information,  
+_1_2 create a weighted network with igraph. For a given number  
+_1_3 of iterations, deletion amounts, and deletion types, the  
+_1_4 algorithm then generates network statistics for randomly 
+_1_5 sampled subnetworks.  
+_1_6 """ 
+_1_7 
+_1_8 def __init__(self, dataframe): 
 _1_9 self.inputDF = dataframe 
 _2_0 
-_2_1 def makeNet(self, dataframe:pd.DataFrame) -> ig.Graph: 
+_2_1 def makeNet(self, dataframe): 
 _2_2 """Create network from dataframe. 
-_2_3 
+_2_3  
 _2_4 Assumes the existence of sender, receiver and step 
-_2_5 column names. 
+_2_5 column names.  
 _2_6 """ 
-_2_7 networkdata = dataframe[["sender", "receiver", "step"]] 
-_2_8 networkdata = networkdata.groupby( 
-_2_9 ["sender", "receiver"], 
-_3_0 ).size().reset_index(name="Count") 
-_3_1 return ig.Graph.TupleList( 
-_3_2 networkdata.itertuples(index=False), directed=True, weights=True, 
+_2_7 df = dataframe[['sender', 'receiver', 'step']] 
+_2_8 df = df.groupby( 
+_2_9 ['sender', 'receiver'] 
+_3_0 ).size().reset_index(name='Count') 
+_3_1 net = ig.Graph.TupleList( 
+_3_2 df.itertuples(index=False), directed=True, weights=True 
 _3_3 ) 
-_3_4 
-_3_5 def netStats(self, G:ig.Graph) -> pd.DataFrame: 
-_3_6 """Generate network statistics. 
-_3_7 
-_3_8 Any statistic calculated on the full 
-_3_9 network can be added in principle. 
-_4_0 Currently implemented are: 
-_4_1 average relative degree, 
-_4_2 density 
-_4_3 transitivtiy 
-_4_4 cohesion 
-_4_5 average path length 
-_4_6 modularity 
-_4_7 """ 
-_4_8 numVs = len(G.vs) 
-_4_9 avg_rel_deg = np.mean([x/numVs for x in G.degree(mode="all")]) 
-_5_0 density = G.density() 
-_5_1 transitivity = G.transitivity_undirected() 
-_5_2 cohesion = G.cohesion() 
-_5_3 avg_path_len = G.average_path_length() 
-_5_4 modularity = G.modularity(G.components()) 
-_5_5 return pd.DataFrame( 
-_5_6 [ 
-_5_7 { 
-_5_8 "avg_relative_degree": avg_rel_deg, 
-_5_9 "avg_path_length": avg_path_len, 
-_6_0 "density": density, 
-_6_1 "transitivity": transitivity, 
-_6_2 "cohesion": cohesion, 
-_6_3 "modularity": modularity, 
-_6_4 }, 
-_6_5 ], 
-_6_6 ) 
-_6_7 
-_6_8 def generatePruningParameters(self, G:ig.Graph) -> pd.DataFrame: 
-_6_9 """Generate a random set of pruning weights.""" 
-_7_0 nodes = G.get_vertex_dataframe() 
-_7_1 id2name = G.get_vertex_dataframe().to_dict()["name"] 
-_7_2 rng = np.random.default_rng() 
-_7_3 del_parameter = pd.DataFrame( 
-_7_4 { 
-_7_5 "ids": nodes.index, 
-_7_6 "degree": G.degree(), 
-_7_7 "unif": rng.uniform(0, 1, len(G.vs)), 
-_7_8 "log_normal": rng.lognormal(0, 1, len(G.vs)), 
-_7_9 "exp": rng.exponential(1, len(G.vs)), 
-_8_0 "beta": rng.beta(a=2, b=3, size=len(G.vs)), 
-_8_1 }, 
-_8_2 ) 
-_8_3 
-_8_4 del_parameter = G.get_edge_dataframe()[["source", "target"]].merge( 
-_8_5 del_parameter, left_on="source", right_on="ids", 
-_8_6 ).merge( 
-_8_7 del_parameter, left_on="target", right_on="ids", 
-_8_8 ) 
-_8_9 del_parameter["degree"] = del_parameter.degree_x * del_parameter.degree_y /
-np.dot( 
-_9_0 del_parameter.degree_x, del_parameter.degree_y, 
-_9_1 ) 
-_9_2 del_parameter["unif"] = del_parameter.unif_x * del_parameter.unif_y / np.dot
-( 
-_9_3 del_parameter.unif_x, del_parameter.unif_y, 
-_9_4 ) 
-_9_5 del_parameter["log_normal"] = del_parameter.log_normal_x *
-del_parameter.log_normal_y / np.dot( 
-_9_6 del_parameter.log_normal_x, del_parameter.log_normal_y, 
-_9_7 ) 
-_9_8 del_parameter["exp"] = del_parameter.exp_x * del_parameter.exp_y / np.dot( 
-_9_9 del_parameter.exp_x, del_parameter.exp_y, 
-_1_0_0 ) 
-_1_0_1 del_parameter["beta"] = del_parameter.beta_x * del_parameter.beta_y /
-np.dot( 
-_1_0_2 del_parameter.beta_x, del_parameter.beta_y, 
-_1_0_3 ) 
-_1_0_4 sender = del_parameter["source"].apply(lambda x: id2name[x]) 
-_1_0_5 receiver = del_parameter["target"].apply(lambda x: id2name[x]) 
-_1_0_6 del_parameter.insert(0, "sender", sender) 
-_1_0_7 del_parameter.insert(0, "receiver", receiver) 
-_1_0_8 return del_parameter[ 
-_1_0_9 ["sender", "receiver", "degree", "unif", "log_normal", "exp", "beta"] 
-_1_1_0 ] 
-_1_1_1 
-_1_1_2 
-_1_1_3 def deleteFromNetwork( 
-_1_1_4 self, 
-_1_1_5 iterations: int = 10, 
-_1_1_6 delAmounts: tuple = (0.1, 0.25, 0.5, 0.75, 0.9), 
-_1_1_7 delTypes: tuple = ("degree", "unif", "log_normal", "exp", "beta"), 
-_1_1_8 ) -> pd.DataFrame: 
-_1_1_9 """Run the deletion by sampling.""" 
-_1_2_0 results = [] 
-_1_2_1 fullNet = self.makeNet( 
-_1_2_2 self.inputDF, 
-_1_2_3 ) 
-_1_2_4 fullStats = self.netStats(fullNet) 
-_1_2_5 fullStats = fullStats.assign( 
-_1_2_6 delVal=0, delType="NA", delIteration=0, 
+_3_4 return net 
+_3_5 
+_3_6 def netStats(self, G): 
+_3_7 """Generate network statistics. 
+_3_8  
+_3_9 Any statistic calculated on the full 
+_4_0 network can be added in principle. 
+_4_1 Currently implemented are:  
+_4_2 average relative degree, 
+_4_3 density 
+_4_4 transitivtiy 
+_4_5 cohesion 
+_4_6 average path length 
+_4_7 modularity 
+_4_8 """ 
+_4_9 numVs = len(G.vs) 
+_5_0 avg_rel_deg = np.mean([x/numVs for x in G.degree(mode="all")]) 
+_5_1 density = G.density() 
+_5_2 transitivity = G.transitivity_undirected() 
+_5_3 cohesion = G.cohesion() 
+_5_4 avg_path_len = G.average_path_length() 
+_5_5 modularity = G.modularity(G.components()) 
+_5_6 statDF = pd.DataFrame( 
+_5_7 [ 
+_5_8 { 
+_5_9 'avg_relative_degree': avg_rel_deg, 
+_6_0 'avg_path_length': avg_path_len, 
+_6_1 'density': density, 
+_6_2 'transitivity': transitivity, 
+_6_3 'cohesion': cohesion, 
+_6_4 'modularity': modularity 
+_6_5 } 
+_6_6 ] 
+_6_7 ) 
+_6_8 return statDF 
+_6_9 
+_7_0 def generatePruningParameters(self, G): 
+_7_1 """Generate a random set of pruning weights.""" 
+_7_2 nodes = G.get_vertex_dataframe() 
+_7_3 id2name = G.get_vertex_dataframe().to_dict()['name'] 
+_7_4 del_parameter = pd.DataFrame( 
+_7_5 { 
+_7_6 'ids': nodes.index, 
+_7_7 'degree': G.degree(), 
+_7_8 'unif': np.random.uniform(0, 1, len(G.vs)), 
+_7_9 'log_normal': np.random.lognormal(0, 1, len(G.vs)), 
+_8_0 'exp': np.random.exponential(1, len(G.vs)), 
+_8_1 'beta': np.random.beta(a=2, b=3, size=len(G.vs)) 
+_8_2 } 
+_8_3 ) 
+_8_4 
+_8_5 del_parameter = G.get_edge_dataframe()[["source", "target"]].merge( 
+_8_6 del_parameter, left_on='source', right_on='ids' 
+_8_7 ).merge( 
+_8_8 del_parameter, left_on='target', right_on='ids' 
+_8_9 ) 
+_9_0 del_parameter['degree'] = del_parameter.degree_x * del_parameter.degree_y /
+np.dot(del_parameter.degree_x, del_parameter.degree_y) 
+_9_1 del_parameter['unif'] = del_parameter.unif_x * del_parameter.unif_y / np.dot
+(del_parameter.unif_x, del_parameter.unif_y) 
+_9_2 del_parameter['log_normal'] = del_parameter.log_normal_x *
+del_parameter.log_normal_y / np.dot(del_parameter.log_normal_x,
+del_parameter.log_normal_y) 
+_9_3 del_parameter['exp'] = del_parameter.exp_x * del_parameter.exp_y / np.dot
+(del_parameter.exp_x, del_parameter.exp_y) 
+_9_4 del_parameter['beta'] = del_parameter.beta_x * del_parameter.beta_y / np.dot
+(del_parameter.beta_x, del_parameter.beta_y) 
+_9_5 sender = del_parameter["source"].apply(lambda x: id2name[x]) 
+_9_6 receiver = del_parameter["target"].apply(lambda x: id2name[x]) 
+_9_7 del_parameter.insert(0, "sender", sender) 
+_9_8 del_parameter.insert(0, "receiver", receiver) 
+_9_9 outDF = del_parameter[ 
+_1_0_0 ['sender', 'receiver', 'degree', 'unif', 'log_normal', 'exp', 'beta'] 
+_1_0_1 ] 
+_1_0_2 return outDF 
+_1_0_3 
+_1_0_4 def deleteFromNetwork( 
+_1_0_5 self, 
+_1_0_6 iterations=10, 
+_1_0_7 delAmounts=(0.1, 0.25, 0.5, 0.75, 0.9), 
+_1_0_8 delTypes=("degree", "unif", "log_normal", "exp", "beta") 
+_1_0_9 ): 
+_1_1_0 """Run the deletion by sampling.""" 
+_1_1_1 results = [] 
+_1_1_2 fullNet = self.makeNet( 
+_1_1_3 self.inputDF 
+_1_1_4 ) 
+_1_1_5 fullStats = self.netStats(fullNet) 
+_1_1_6 fullStats = fullStats.assign( 
+_1_1_7 **{ 
+_1_1_8 "delVal": 0, 
+_1_1_9 "delType": 'NA', 
+_1_2_0 "delIteration": 0 
+_1_2_1 } 
+_1_2_2 ) 
+_1_2_3 results.append(fullStats) 
+_1_2_4 for idx in range(1, iterations + 1): 
+_1_2_5 prunVals = self.generatePruningParameters( 
+_1_2_6 fullNet 
 _1_2_7 ) 
-_1_2_8 results.append(fullStats) 
-_1_2_9 for idx in range(1, iterations + 1): 
-_1_3_0 prunVals = self.generatePruningParameters( 
-_1_3_1 fullNet, 
-_1_3_2 ) 
-_1_3_3 tempDF = self.inputDF.merge( 
-_1_3_4 prunVals, 
-_1_3_5 ) 
-_1_3_6 for val in list(delAmounts): 
-_1_3_7 for deltype in list(delTypes): 
-_1_3_8 delDF = tempDF.sample( 
-_1_3_9 round(len(tempDF) * (1 - val)), 
-_1_4_0 weights=deltype, 
-_1_4_1 ) 
-_1_4_2 delNet = self.makeNet(delDF) 
-_1_4_3 delStats = self.netStats(delNet) 
-_1_4_4 delStats = delStats.assign( 
-_1_4_5 delVal=val, delType=deltype, delIteration=idx, 
-_1_4_6 ) 
-_1_4_7 results.append(delStats) 
-_1_4_8 return pd.concat(results) 
+_1_2_8 tempDF = self.inputDF.merge( 
+_1_2_9 prunVals 
+_1_3_0 ) 
+_1_3_1 for val in list(delAmounts): 
+_1_3_2 for deltype in list(delTypes): 
+_1_3_3 delDF = tempDF.sample( 
+_1_3_4 round(len(tempDF) * (1 - val)), 
+_1_3_5 weights=deltype 
+_1_3_6 ) 
+_1_3_7 delNet = self.makeNet(delDF) 
+_1_3_8 delStats = self.netStats(delNet) 
+_1_3_9 delStats = delStats.assign( 
+_1_4_0 **{ 
+_1_4_1 "delVal": val, 
+_1_4_2 "delType": deltype, 
+_1_4_3 "delIteration": idx 
+_1_4_4 } 
+_1_4_5 ) 
+_1_4_6 results.append(delStats) 
+_1_4_7 resDF = pd.concat(results) 
+_1_4_8 return resDF 
 _1_4_9 
-_1_5_0 
-_1_5_1 
-_1_5_2def prune( 
-_1_5_3 modelparameters: dict, network: tuple, columns: list, 
-_1_5_4 iterations: int = 10, delAmounts: tuple = (0.1, 0.25, 0.5, 0.75, 0.9), 
-_1_5_5 delTypes: tuple = ("degree", "unif")) -> pd.DataFrame: 
-_1_5_6 """Generate pruned networks from input. 
-_1_5_7 
-_1_5_8 Assumes existence of columns "sender", "receiver", and "step". 
-_1_5_9 """ 
-_1_6_0 runDf = pd.DataFrame(network, columns = columns) 
-_1_6_1 pruning = PruneNetwork(runDf) 
-_1_6_2 result = pruning.deleteFromNetwork( 
-_1_6_3 iterations=iterations, 
-_1_6_4 delAmounts=delAmounts, 
-_1_6_5 delTypes=delTypes, 
-_1_6_6 ) 
-_1_6_7 return result.assign(**modelparameters) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+19 14:00 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21___init___py.html` & `scicom-0.4.0/tests/reports/html/d_d0052f7b3fb6bc9f___init___py.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/__init__.py: 100%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/randomletters/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/__init__.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/randomletters/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,42 +56,42 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_e85bc3a05b58e6d3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_d0052f7b3fb6bc9f_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_agents_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_d0052f7b3fb6bc9f_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_e85bc3a05b58e6d3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_agents_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_d0052f7b3fb6bc9f_SimpleContinuousModule_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_d0052f7b3fb6bc9f_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 13:30 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-hhiissttoorriiccaalllleetttteerrss//____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+rraannddoommlleetttteerrss//____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 13:30 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_agents_py.html` & `scicom-0.4.0/tests/reports/html/d_277402163e1a7589_agents_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/agents.py: 93%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/historicalletters/agents.py: 93%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/agents.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/agents.py</b>:
             <span class="pc_cov">93%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,36 +50,36 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">113 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">105<span class="text"> run</span></button>
+            <span class="text">115 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">107<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">8<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_interface_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_interface_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 12:29 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""The agent classes for HistoricalLetters."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">random</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -260,97 +260,104 @@
     <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">                <span class="com"># agent's currently held topic positions.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">updatedTopicsDict</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                    <span class="op">{</span><span class="nam">receiver</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">updatedTopicVec</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="key">def</span> <span class="nam">step</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="str">"""Perform one simulation step."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">topicVec</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">updatedTopicsDict</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">topicLedger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">currentActivation</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">            <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">            <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">activationWeight</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">activationWeight</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">            <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="key">if</span> <span class="nam">currentActivation</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="nam">neighborsMove</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                <span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors_within_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                    <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                    <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                    <span class="nam">center</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                <span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="nam">neighborsSend</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="com"># If the agent has received a letter in the previous step and</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="com"># has updated its internal topicVec state, the new topic state is</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="com"># appended to the topicLedger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">topicLedger</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicLedger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="key">elif</span> <span class="nam">self</span><span class="op">.</span><span class="nam">topicVec</span> <span class="op">!=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">topicLedger</span><span class="op">[</span><span class="op">-</span><span class="num">1</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">topicLedger</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="nam">currentActivation</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">            <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">activationWeight</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">activationWeight</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">            <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="key">if</span> <span class="nam">currentActivation</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="nam">neighborsMove</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                <span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors_within_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                    <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">letterRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                    <span class="nam">center</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">sendLetter</span><span class="op">(</span><span class="nam">neighborsSend</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">move</span><span class="op">(</span><span class="nam">neighborsMove</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="key">class</span> <span class="nam">RegionAgent</span><span class="op">(</span><span class="nam">mg</span><span class="op">.</span><span class="nam">GeoAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="str">"""The region keeping track of contained agents.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">    This agent type is introduced for visualization purposes.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">    SenderAgents are linked to regions by calculation of a</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">    geographic overlap of the region shape with the SenderAgent</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    position.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    At initialization, the regions are populated with SenderAgents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">    giving rise to a dictionary of the contained SenderAgent IDs and</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    their initial topic.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">    At each movement, the SenderAgent might cross region boundaries.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">    This reqieres a re-calculation of the potential overlap.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="nam">unique_id</span><span class="op">:</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="nam">model</span><span class="op">:</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="nam">geometry</span><span class="op">:</span> <span class="nam">shapely</span><span class="op">.</span><span class="nam">geometry</span><span class="op">.</span><span class="nam">polygon</span><span class="op">.</span><span class="nam">Polygon</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">crs</span><span class="op">:</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="str">"""Initialize region with id, model, geometry and crs."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">model</span><span class="op">,</span> <span class="nam">geometry</span><span class="op">,</span> <span class="nam">crs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">main_topic</span><span class="op">:</span><span class="nam">tuple</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">has_main_topic</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_main_topic</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="str">"""Return weighted average topics of agents in region."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="nam">topics</span> <span class="op">=</span> <span class="op">[</span><span class="nam">y</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">for</span> <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">            <span class="nam">total</span> <span class="op">=</span> <span class="op">[</span><span class="nam">y</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">for</span> <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="nam">weight</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="op">/</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">total</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">total</span><span class="op">]</span> <span class="key">if</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">total</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span> <span class="key">else</span> <span class="op">[</span><span class="num">1</span> <span class="op">/</span> <span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span><span class="op">]</span> <span class="op">*</span> <span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">            <span class="nam">mixed_colors</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">sum</span><span class="op">(</span><span class="op">[</span><span class="nam">np</span><span class="op">.</span><span class="nam">multiply</span><span class="op">(</span><span class="nam">weight</span><span class="op">[</span><span class="nam">i</span><span class="op">]</span><span class="op">,</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">i</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">i</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span><span class="op">)</span><span class="op">]</span><span class="op">,</span> <span class="nam">axis</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">            <span class="key">return</span> <span class="nam">np</span><span class="op">.</span><span class="nam">subtract</span><span class="op">(</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span><span class="op">,</span> <span class="nam">mixed_colors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span><span class="num">0.5</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.5</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_sender</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">sender</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="str">"""Add a sender to the region."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="nam">receivedLetters</span> <span class="op">=</span> <span class="nam">sender</span><span class="op">.</span><span class="nam">numLettersReceived</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="nam">scale</span> <span class="op">=</span> <span class="nam">receivedLetters</span> <span class="key">if</span> <span class="nam">receivedLetters</span> <span class="key">else</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">            <span class="op">{</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="op">(</span><span class="nam">sender</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">,</span> <span class="nam">scale</span><span class="op">)</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_sender</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">sender</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="str">"""Remove a sender from the region."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">        <span class="key">del</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">[</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="nam">neighborsSend</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                <span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors_within_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                    <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">letterRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                    <span class="nam">center</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                <span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">sendLetter</span><span class="op">(</span><span class="nam">neighborsSend</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">move</span><span class="op">(</span><span class="nam">neighborsMove</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="key">class</span> <span class="nam">RegionAgent</span><span class="op">(</span><span class="nam">mg</span><span class="op">.</span><span class="nam">GeoAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="str">"""The region keeping track of contained agents.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">    This agent type is introduced for visualization purposes.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">    SenderAgents are linked to regions by calculation of a</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">    geographic overlap of the region shape with the SenderAgent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">    position.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">    At initialization, the regions are populated with SenderAgents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">    giving rise to a dictionary of the contained SenderAgent IDs and</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">    their initial topic.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">    At each movement, the SenderAgent might cross region boundaries.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">    This reqieres a re-calculation of the potential overlap.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="nam">unique_id</span><span class="op">:</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="nam">model</span><span class="op">:</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="nam">geometry</span><span class="op">:</span> <span class="nam">shapely</span><span class="op">.</span><span class="nam">geometry</span><span class="op">.</span><span class="nam">polygon</span><span class="op">.</span><span class="nam">Polygon</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">crs</span><span class="op">:</span><span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="str">"""Initialize region with id, model, geometry and crs."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">model</span><span class="op">,</span> <span class="nam">geometry</span><span class="op">,</span> <span class="nam">crs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">main_topic</span><span class="op">:</span><span class="nam">tuple</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">has_main_topic</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="key">def</span> <span class="nam">has_main_topic</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">tuple</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="str">"""Return weighted average topics of agents in region."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="nam">topics</span> <span class="op">=</span> <span class="op">[</span><span class="nam">y</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">for</span> <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">            <span class="nam">total</span> <span class="op">=</span> <span class="op">[</span><span class="nam">y</span><span class="op">[</span><span class="num">1</span><span class="op">]</span> <span class="key">for</span> <span class="nam">x</span><span class="op">,</span> <span class="nam">y</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">            <span class="nam">weight</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="op">/</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">total</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">total</span><span class="op">]</span> <span class="key">if</span> <span class="nam">sum</span><span class="op">(</span><span class="nam">total</span><span class="op">)</span> <span class="op">></span> <span class="num">0</span> <span class="key">else</span> <span class="op">[</span><span class="num">1</span> <span class="op">/</span> <span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span><span class="op">]</span> <span class="op">*</span> <span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">            <span class="nam">mixed_colors</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">sum</span><span class="op">(</span><span class="op">[</span><span class="nam">np</span><span class="op">.</span><span class="nam">multiply</span><span class="op">(</span><span class="nam">weight</span><span class="op">[</span><span class="nam">i</span><span class="op">]</span><span class="op">,</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">i</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">i</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">topics</span><span class="op">)</span><span class="op">)</span><span class="op">]</span><span class="op">,</span> <span class="nam">axis</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">            <span class="key">return</span> <span class="nam">np</span><span class="op">.</span><span class="nam">subtract</span><span class="op">(</span><span class="op">(</span><span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span><span class="op">,</span> <span class="nam">mixed_colors</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span><span class="num">0.5</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.5</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_sender</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">sender</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">        <span class="str">"""Add a sender to the region."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="nam">receivedLetters</span> <span class="op">=</span> <span class="nam">sender</span><span class="op">.</span><span class="nam">numLettersReceived</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">        <span class="nam">scale</span> <span class="op">=</span> <span class="nam">receivedLetters</span> <span class="key">if</span> <span class="nam">receivedLetters</span> <span class="key">else</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="op">{</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="op">(</span><span class="nam">sender</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">,</span> <span class="nam">scale</span><span class="op">)</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="key">def</span> <span class="nam">remove_sender</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">sender</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="str">"""Remove a sender from the region."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">        <span class="key">del</span> <span class="nam">self</span><span class="op">.</span><span class="nam">senders_in_region</span><span class="op">[</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_interface_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_interface_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 12:29 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 hhiissttoorriiccaalllleetttteerrss//aaggeennttss..ppyy:: 9933%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 111133 ssttaatteemmeennttss ?  110055 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+********** 111155 ssttaatteemmeennttss ?  110077 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 12:29 +0200
 _1"""The agent classes for HistoricalLetters.""" 
 _2import random 
 _3 
 _4import mesa 
 _5import mesa_geo as mg 
 _6import numpy as np 
 _7import shapely 
@@ -200,86 +200,93 @@
 _1_7_8 # agent's currently held topic positions. 
 _1_7_9 self.model.updatedTopicsDict.update( 
 _1_8_0 {receiver.unique_id: updatedTopicVec}, 
 _1_8_1 ) 
 _1_8_2 
 _1_8_3 def step(self) -> None: 
 _1_8_4 """Perform one simulation step.""" 
-_1_8_5 self.topicVec = self.model.updatedTopicsDict[self.unique_id] 
-_1_8_6 self.topicLedger.append( 
-_1_8_7 self.topicVec, 
-_1_8_8 ) 
-_1_8_9 currentActivation = random.choices( 
-_1_9_0 population=[0, 1], 
-_1_9_1 weights=[1 - self.activationWeight, self.activationWeight], 
-_1_9_2 k=1, 
-_1_9_3 ) 
-_1_9_4 if currentActivation[0] == 1: 
-_1_9_5 neighborsMove = [ 
-_1_9_6 x for x in self.model.space.get_neighbors_within_distance( 
-_1_9_7 self, 
-_1_9_8 distance=self.moveRange * self.model.meandistance, 
-_1_9_9 center=False, 
-_2_0_0 ) if isinstance(x, SenderAgent) 
-_2_0_1 ] 
-_2_0_2 neighborsSend = [ 
+_1_8_5 # If the agent has received a letter in the previous step and 
+_1_8_6 # has updated its internal topicVec state, the new topic state is 
+_1_8_7 # appended to the topicLedger 
+_1_8_8 if not self.topicLedger: 
+_1_8_9 self.topicLedger.append( 
+_1_9_0 self.topicVec, 
+_1_9_1 ) 
+_1_9_2 elif self.topicVec != self.topicLedger[-1]: 
+_1_9_3 self.topicLedger.append( 
+_1_9_4 self.topicVec, 
+_1_9_5 ) 
+_1_9_6 currentActivation = random.choices( 
+_1_9_7 population=[0, 1], 
+_1_9_8 weights=[1 - self.activationWeight, self.activationWeight], 
+_1_9_9 k=1, 
+_2_0_0 ) 
+_2_0_1 if currentActivation[0] == 1: 
+_2_0_2 neighborsMove = [ 
 _2_0_3 x for x in self.model.space.get_neighbors_within_distance( 
 _2_0_4 self, 
-_2_0_5 distance=self.letterRange * self.model.meandistance, 
+_2_0_5 distance=self.moveRange * self.model.meandistance, 
 _2_0_6 center=False, 
 _2_0_7 ) if isinstance(x, SenderAgent) 
 _2_0_8 ] 
-_2_0_9 self.sendLetter(neighborsSend) 
-_2_1_0 self.move(neighborsMove) 
-_2_1_1 
-_2_1_2 
-_2_1_3class RegionAgent(mg.GeoAgent): 
-_2_1_4 """The region keeping track of contained agents. 
-_2_1_5 
-_2_1_6 This agent type is introduced for visualization purposes. 
-_2_1_7 SenderAgents are linked to regions by calculation of a 
-_2_1_8 geographic overlap of the region shape with the SenderAgent 
-_2_1_9 position. 
-_2_2_0 At initialization, the regions are populated with SenderAgents 
-_2_2_1 giving rise to a dictionary of the contained SenderAgent IDs and 
-_2_2_2 their initial topic. 
-_2_2_3 At each movement, the SenderAgent might cross region boundaries. 
-_2_2_4 This reqieres a re-calculation of the potential overlap. 
-_2_2_5 """ 
-_2_2_6 
-_2_2_7 def __init__( 
-_2_2_8 self, 
-_2_2_9 unique_id:str, 
-_2_3_0 model:mesa.Model, 
-_2_3_1 geometry: shapely.geometry.polygon.Polygon, 
-_2_3_2 crs:str, 
-_2_3_3 ) -> None: 
-_2_3_4 """Initialize region with id, model, geometry and crs.""" 
-_2_3_5 super().__init__(unique_id, model, geometry, crs) 
-_2_3_6 self.senders_in_region = {} 
-_2_3_7 self.main_topic:tuple = self.has_main_topic() 
-_2_3_8 
-_2_3_9 def has_main_topic(self) -> tuple: 
-_2_4_0 """Return weighted average topics of agents in region.""" 
-_2_4_1 if len(self.senders_in_region) > 0: 
-_2_4_2 topics = [y[0] for x, y in self.senders_in_region.items()] 
-_2_4_3 total = [y[1] for x, y in self.senders_in_region.items()] 
-_2_4_4 weight = [x / sum(total) for x in total] if sum(total) > 0 else [1 / len
+_2_0_9 neighborsSend = [ 
+_2_1_0 x for x in self.model.space.get_neighbors_within_distance( 
+_2_1_1 self, 
+_2_1_2 distance=self.letterRange * self.model.meandistance, 
+_2_1_3 center=False, 
+_2_1_4 ) if isinstance(x, SenderAgent) 
+_2_1_5 ] 
+_2_1_6 self.sendLetter(neighborsSend) 
+_2_1_7 self.move(neighborsMove) 
+_2_1_8 
+_2_1_9 
+_2_2_0class RegionAgent(mg.GeoAgent): 
+_2_2_1 """The region keeping track of contained agents. 
+_2_2_2 
+_2_2_3 This agent type is introduced for visualization purposes. 
+_2_2_4 SenderAgents are linked to regions by calculation of a 
+_2_2_5 geographic overlap of the region shape with the SenderAgent 
+_2_2_6 position. 
+_2_2_7 At initialization, the regions are populated with SenderAgents 
+_2_2_8 giving rise to a dictionary of the contained SenderAgent IDs and 
+_2_2_9 their initial topic. 
+_2_3_0 At each movement, the SenderAgent might cross region boundaries. 
+_2_3_1 This reqieres a re-calculation of the potential overlap. 
+_2_3_2 """ 
+_2_3_3 
+_2_3_4 def __init__( 
+_2_3_5 self, 
+_2_3_6 unique_id:str, 
+_2_3_7 model:mesa.Model, 
+_2_3_8 geometry: shapely.geometry.polygon.Polygon, 
+_2_3_9 crs:str, 
+_2_4_0 ) -> None: 
+_2_4_1 """Initialize region with id, model, geometry and crs.""" 
+_2_4_2 super().__init__(unique_id, model, geometry, crs) 
+_2_4_3 self.senders_in_region = {} 
+_2_4_4 self.main_topic:tuple = self.has_main_topic() 
+_2_4_5 
+_2_4_6 def has_main_topic(self) -> tuple: 
+_2_4_7 """Return weighted average topics of agents in region.""" 
+_2_4_8 if len(self.senders_in_region) > 0: 
+_2_4_9 topics = [y[0] for x, y in self.senders_in_region.items()] 
+_2_5_0 total = [y[1] for x, y in self.senders_in_region.items()] 
+_2_5_1 weight = [x / sum(total) for x in total] if sum(total) > 0 else [1 / len
 (topics)] * len(topics) 
-_2_4_5 mixed_colors = np.sum([np.multiply(weight[i], topics[i]) for i in range(len
+_2_5_2 mixed_colors = np.sum([np.multiply(weight[i], topics[i]) for i in range(len
 (topics))], axis=0) 
-_2_4_6 return np.subtract((1, 1, 1), mixed_colors) 
-_2_4_7 return (0.5, 0.5, 0.5) 
-_2_4_8 
-_2_4_9 def add_sender(self, sender: SenderAgent) -> None: 
-_2_5_0 """Add a sender to the region.""" 
-_2_5_1 receivedLetters = sender.numLettersReceived 
-_2_5_2 scale = receivedLetters if receivedLetters else 1 
-_2_5_3 self.senders_in_region.update( 
-_2_5_4 {sender.unique_id: (sender.topicVec, scale)}, 
-_2_5_5 ) 
-_2_5_6 
-_2_5_7 def remove_sender(self, sender: SenderAgent) -> None: 
-_2_5_8 """Remove a sender from the region.""" 
-_2_5_9 del self.senders_in_region[sender.unique_id] 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+_2_5_3 return np.subtract((1, 1, 1), mixed_colors) 
+_2_5_4 return (0.5, 0.5, 0.5) 
+_2_5_5 
+_2_5_6 def add_sender(self, sender: SenderAgent) -> None: 
+_2_5_7 """Add a sender to the region.""" 
+_2_5_8 receivedLetters = sender.numLettersReceived 
+_2_5_9 scale = receivedLetters if receivedLetters else 1 
+_2_6_0 self.senders_in_region.update( 
+_2_6_1 {sender.unique_id: (sender.topicVec, scale)}, 
+_2_6_2 ) 
+_2_6_3 
+_2_6_4 def remove_sender(self, sender: SenderAgent) -> None: 
+_2_6_5 """Remove a sender from the region.""" 
+_2_6_6 del self.senders_in_region[sender.unique_id] 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 12:29 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_interface_py.html` & `scicom-0.4.0/tests/reports/html/d_277402163e1a7589_interface_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/interface.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/historicalletters/interface.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/interface.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/interface.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">39 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">39<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_model_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Define the solara interface to run and control the HistoricalLetters model."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -204,18 +204,18 @@
     <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="nam">agent_portrayal</span><span class="op">=</span><span class="nam">topic_draw</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="nam">space_drawer</span><span class="op">=</span><span class="nam">make_geospace</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_model_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_agents_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 hhiissttoorriiccaalllleetttteerrss//iinntteerrffaaccee..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3399 ssttaatteemmeennttss ?  00 rruunn 3399 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
 _1"""Define the solara interface to run and control the HistoricalLetters
 model.""" 
 _2from __future__ import annotations 
 _3 
 _4from typing import TYPE_CHECKING 
 _5 
 _6if TYPE_CHECKING: 
@@ -136,9 +136,9 @@
 _1_1_8 HistoricalLetters, 
 _1_1_9 model_params, 
 _1_2_0 measures=["Movements", "Clusters", "Letters"], 
 _1_2_1 name="Historical Letters ABM", 
 _1_2_2 agent_portrayal=topic_draw, 
 _1_2_3 space_drawer=make_geospace, 
 _1_2_4) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_model_py.html` & `scicom-0.4.0/tests/reports/html/d_277402163e1a7589_model_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/model.py: 94%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/historicalletters/model.py: 95%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/model.py</b>:
-            <span class="pc_cov">94%</span>
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/model.py</b>:
+            <span class="pc_cov">95%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,36 +50,36 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">108 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">102<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">6<span class="text"> missing</span></button>
+            <span class="text">110 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">105<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_interface_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_interface_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_server_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 13:48 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""The model class for HistoricalLetters."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">random</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
@@ -99,293 +99,306 @@
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">def</span> <span class="nam">getPrunedLedger</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="str">"""Model reporter for simulation of archiving.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    Returns statistics of ledger network of model run</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">    and various iterations of statistics of pruned networks.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="com"># TODO(malte): Add all model params</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">if</span> <span class="nam">model</span><span class="op">.</span><span class="nam">runPruning</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">ledgerColumns</span> <span class="op">=</span> <span class="op">[</span><span class="str">"sender"</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="str">"sender_location"</span><span class="op">,</span> <span class="str">"receiver_location"</span><span class="op">,</span> <span class="str">"topic"</span><span class="op">,</span> <span class="str">"step"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">modelparams</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="str">"population"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">population</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">moveRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">letterRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="str">"useActivation"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">useActivation</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="str">"useSocialNetwork"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">useSocialNetwork</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">prune</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="nam">modelparameters</span><span class="op">=</span><span class="nam">modelparams</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="nam">network</span><span class="op">=</span><span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="nam">columns</span><span class="op">=</span><span class="nam">ledgerColumns</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="key">def</span> <span class="nam">getComponents</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="str">"""Model reporter to get number of components.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">    The MultiDiGraph is converted to undirected,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">    considering only edges that are reciprocal, ie.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    edges are established if sender and receiver have</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    exchanged at least a letter in each direction.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">newg</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">.</span><span class="nam">to_undirected</span><span class="op">(</span><span class="nam">reciprocal</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">return</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">number_connected_components</span><span class="op">(</span><span class="nam">newg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">getScaledLetters</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""Return relative number of send letters."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span><span class="op">)</span><span class="op">/</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="key">def</span> <span class="nam">getScaledMovements</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="str">"""Return relative number of movements."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">movements</span><span class="op">/</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    The routine assumes that the network contains fields of sender,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">    receiver and step information.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">if</span> <span class="nam">model</span><span class="op">.</span><span class="nam">runPruning</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">ledgerColumns</span> <span class="op">=</span> <span class="op">[</span><span class="str">"sender"</span><span class="op">,</span> <span class="str">"receiver"</span><span class="op">,</span> <span class="str">"sender_location"</span><span class="op">,</span> <span class="str">"receiver_location"</span><span class="op">,</span> <span class="str">"topic"</span><span class="op">,</span> <span class="str">"step"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">modelparams</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="str">"population"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">population</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">moveRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">letterRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">            <span class="str">"useActivation"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">useActivation</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="str">"useSocialNetwork"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">useSocialNetwork</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="str">"similarityThreshold"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">similarityThreshold</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="str">"longRangeNetworkFactor"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="str">"shortRangeNetworkFactor"</span><span class="op">:</span> <span class="nam">model</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">prune</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="nam">modelparameters</span><span class="op">=</span><span class="nam">modelparams</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="nam">network</span><span class="op">=</span><span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="nam">columns</span><span class="op">=</span><span class="nam">ledgerColumns</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">            <span class="nam">iterations</span><span class="op">=</span><span class="num">3</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">delAmounts</span><span class="op">=</span><span class="op">(</span><span class="num">0.1</span><span class="op">,</span> <span class="num">0.25</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.75</span><span class="op">,</span> <span class="num">0.9</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="nam">delTypes</span><span class="op">=</span><span class="op">(</span><span class="str">"unif"</span><span class="op">,</span> <span class="str">"exp"</span><span class="op">,</span> <span class="str">"beta"</span><span class="op">,</span> <span class="str">"log_normal1"</span><span class="op">,</span> <span class="str">"log_normal2"</span><span class="op">,</span> <span class="str">"log_normal3"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="nam">delMethod</span><span class="op">=</span><span class="op">(</span><span class="str">"agents"</span><span class="op">,</span> <span class="str">"regions"</span><span class="op">,</span> <span class="str">"time"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">rankedVals</span><span class="op">=</span><span class="op">(</span><span class="key">True</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="key">def</span> <span class="nam">getComponents</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="str">"""Model reporter to get number of components.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    The MultiDiGraph is converted to undirected,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    considering only edges that are reciprocal, ie.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    edges are established if sender and receiver have</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">    exchanged at least a letter in each direction.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">newg</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">.</span><span class="nam">to_undirected</span><span class="op">(</span><span class="nam">reciprocal</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">return</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">number_connected_components</span><span class="op">(</span><span class="nam">newg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="key">class</span> <span class="nam">HistoricalLetters</span><span class="op">(</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="str">"""A letter sending model with historical informed initital positions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">    Each agent has an initial topic vector, expressed as a RGB value. The</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">    initial positions of the agents is based on a weighted random draw</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t"><span class="str">    based on data from [1].</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">    Each step, agents generate two neighbourhoods for sending letters and</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">    potential targets to move towards. The probability to send letters is</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">    a self-reinforcing process. During each sending the internal topic of</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">    the sender is updated as a random rotation towards the receivers topic.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="str">    [1] J. Lobo et al, Population-Area Relationship for Medieval European Cities,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="str">        PLoS ONE 11(10): e0162678.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">population</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="nam">moveRange</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.05</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="nam">letterRange</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.2</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="nam">similarityThreshold</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.2</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="nam">longRangeNetworkFactor</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.3</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">shortRangeNetworkFactor</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.4</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">regionData</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"data/NUTS_RG_60M_2021_3857_LEVL_2.geojson"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="nam">populationDistributionData</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"data/pone.0162678.s003.csv"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">useActivation</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">useSocialNetwork</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">runPruning</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">debug</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="str">"""Initialize a HistoricalLetters model."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="com"># Parameters for agents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">population</span> <span class="op">=</span> <span class="nam">population</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">=</span> <span class="nam">moveRange</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">letterRange</span> <span class="op">=</span> <span class="nam">letterRange</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="com"># Parameters for model</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">runPruning</span> <span class="op">=</span> <span class="nam">runPruning</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">useActivation</span> <span class="op">=</span> <span class="nam">useActivation</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">useSocialNetwork</span> <span class="op">=</span> <span class="nam">useSocialNetwork</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span> <span class="op">=</span> <span class="nam">longRangeNetworkFactor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span> <span class="op">=</span> <span class="nam">shortRangeNetworkFactor</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="com"># Initialize social network</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">MultiDiGraph</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="com"># Output variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">letterLedger</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">movements</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="com"># Internal variables</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">time</span><span class="op">.</span><span class="nam">RandomActivation</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">scaleSendInput</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">updatedTopicsDict</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">space</span> <span class="op">=</span> <span class="nam">Nuts2Eu</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">debug</span> <span class="op">=</span> <span class="nam">debug</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="com"># Initialize region agents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="com"># Set up the grid with patches for every NUTS region</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="com"># Create region agents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">ac</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">AgentCreator</span><span class="op">(</span><span class="nam">RegionAgent</span><span class="op">,</span> <span class="nam">model</span><span class="op">=</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">regions</span> <span class="op">=</span> <span class="nam">ac</span><span class="op">.</span><span class="nam">from_file</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="nam">regionData</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">            <span class="nam">unique_id</span><span class="op">=</span><span class="str">"NUTS_ID"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="com"># Add regions to Nuts2Eu geospace</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">add_regions</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">regions</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="com"># Initialize sender agents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="com"># Draw initial geographic positions of agents</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">initSenderGeoDf</span> <span class="op">=</span> <span class="nam">createData</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">            <span class="nam">population</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">populationDistribution</span><span class="op">=</span><span class="nam">populationDistributionData</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="com"># Calculate mean of mean distances for each agent.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="com"># This is used as a measure for the range of exchanges.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="nam">meandistances</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span> <span class="key">in</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">index</span><span class="op">.</span><span class="nam">to_numpy</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">            <span class="nam">name</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">loc</span><span class="op">[</span><span class="nam">idx</span><span class="op">,</span> <span class="str">"unique_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">geom</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">loc</span><span class="op">[</span><span class="nam">idx</span><span class="op">,</span> <span class="str">"geometry"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">            <span class="nam">otherAgents</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">f"unique_id != '{name}'"</span><span class="op">)</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">            <span class="nam">geometries</span> <span class="op">=</span> <span class="nam">otherAgents</span><span class="op">.</span><span class="nam">geometry</span><span class="op">.</span><span class="nam">to_numpy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">            <span class="nam">distances</span> <span class="op">=</span> <span class="op">[</span><span class="nam">geom</span><span class="op">.</span><span class="nam">distance</span><span class="op">(</span><span class="nam">othergeom</span><span class="op">)</span> <span class="key">for</span> <span class="nam">othergeom</span> <span class="key">in</span> <span class="nam">geometries</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">            <span class="nam">meandistances</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">mean</span><span class="op">(</span><span class="nam">distances</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">meandistance</span> <span class="op">=</span> <span class="nam">mean</span><span class="op">(</span><span class="nam">meandistances</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="com"># Populate factors dictionary</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">factors</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="str">"similarityThreshold"</span><span class="op">:</span> <span class="nam">similarityThreshold</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">moveRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">            <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">letterRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="com"># Set up agent creator for senders</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">ac_senders</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">AgentCreator</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="nam">SenderAgent</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">            <span class="nam">model</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="nam">agent_kwargs</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">factors</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">        <span class="com"># Create agents based on random coordinates generated</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">        <span class="com"># in the createData step above, see util.py file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">senders</span> <span class="op">=</span> <span class="nam">ac_senders</span><span class="op">.</span><span class="nam">from_GeoDataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">            <span class="nam">initSenderGeoDf</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="nam">unique_id</span><span class="op">=</span><span class="str">"unique_id"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="com"># Create random set of initial topic vectors.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="nam">topics</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="nam">tuple</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">                <span class="op">[</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">3</span><span class="op">)</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">            <span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="com"># Setup senders</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">sender</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">senders</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">            <span class="com"># Add to social network</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">.</span><span class="nam">add_node</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                <span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                <span class="nam">numLettersSend</span><span class="op">=</span><span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                <span class="nam">numLettersReceived</span><span class="op">=</span><span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="com"># Give sender topic</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="nam">sender</span><span class="op">.</span><span class="nam">topicVec</span> <span class="op">=</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">idx</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">            <span class="com"># Add current topic to dict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">updatedTopicsDict</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                <span class="op">{</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">idx</span><span class="op">]</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="com"># Set random activation weight</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">            <span class="key">if</span> <span class="nam">useActivation</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                <span class="nam">sender</span><span class="op">.</span><span class="nam">activationWeight</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="com"># Add sender to its region</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="nam">regionID</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">regions</span> <span class="key">if</span> <span class="nam">contains</span><span class="op">(</span><span class="nam">x</span><span class="op">.</span><span class="nam">geometry</span><span class="op">,</span> <span class="nam">sender</span><span class="op">.</span><span class="nam">geometry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">add_sender</span><span class="op">(</span><span class="nam">sender</span><span class="op">,</span> <span class="nam">regionID</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">            <span class="key">except</span> <span class="nam">IndexError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                <span class="nam">text</span> <span class="op">=</span> <span class="str">f"Problem finding region for {sender.geometry}."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                <span class="key">raise</span> <span class="nam">IndexError</span><span class="op">(</span><span class="nam">text</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">            <span class="com"># Add sender to schedule</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">sender</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">        <span class="com"># Add graph to network grid for potential visualization.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="com"># TODO(malte): Not yet implemented. Maybe use Solara backend for this?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="com"># self.grid = mesa.space.NetworkGrid(self.socialNetwork)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="com"># Create social network</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="key">if</span> <span class="nam">useSocialNetwork</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">            <span class="key">for</span> <span class="nam">agent</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">                <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">_createSocialEdges</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">DataCollector</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="nam">model_reporters</span><span class="op">=</span><span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">                <span class="str">"Ledger"</span><span class="op">:</span> <span class="nam">getPrunedLedger</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">                <span class="str">"Letters"</span><span class="op">:</span> <span class="nam">getScaledLetters</span> <span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">                <span class="str">"Movements"</span><span class="op">:</span> <span class="nam">getScaledMovements</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">                <span class="str">"Clusters"</span><span class="op">:</span> <span class="nam">getComponents</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="key">def</span> <span class="nam">_createSocialEdges</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">agent</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">,</span> <span class="nam">graph</span><span class="op">:</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">MultiDiGraph</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="str">"""Create social edges with the different wiring factors.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">        Define a close range by using the moveRange parameter. Among</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">        these neighbors, create a connection with probability set by</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">        the shortRangeNetworkFactor.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="key">def</span> <span class="nam">getScaledLetters</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="str">"""Return relative number of send letters."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">model</span><span class="op">.</span><span class="nam">letterLedger</span><span class="op">)</span><span class="op">/</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t"><span class="key">def</span> <span class="nam">getScaledMovements</span><span class="op">(</span><span class="nam">model</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span> <span class="op">-></span> <span class="nam">float</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="str">"""Return relative number of movements."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="key">return</span> <span class="nam">model</span><span class="op">.</span><span class="nam">movements</span><span class="op">/</span><span class="nam">model</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="key">class</span> <span class="nam">HistoricalLetters</span><span class="op">(</span><span class="nam">mesa</span><span class="op">.</span><span class="nam">Model</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="str">"""A letter sending model with historical informed initital positions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="str">    Each agent has an initial topic vector, expressed as a RGB value. The</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">    initial positions of the agents is based on a weighted random draw</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">    based on data from [1].</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="str">    Each step, agents generate two neighbourhoods for sending letters and</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="str">    potential targets to move towards. The probability to send letters is</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="str">    a self-reinforcing process. During each sending the internal topic of</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">    the sender is updated as a random rotation towards the receivers topic.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="str">    [1] J. Lobo et al, Population-Area Relationship for Medieval European Cities,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">        PLoS ONE 11(10): e0162678.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">population</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">moveRange</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.05</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">letterRange</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.2</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">similarityThreshold</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.2</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">longRangeNetworkFactor</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.3</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">shortRangeNetworkFactor</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="num">0.4</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">regionData</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"data/NUTS_RG_60M_2021_3857_LEVL_2.geojson"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="nam">populationDistributionData</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">Path</span><span class="op">(</span><span class="nam">__file__</span><span class="op">)</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">parent</span><span class="op">.</span><span class="nam">resolve</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="str">"data/pone.0162678.s003.csv"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">useActivation</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">useSocialNetwork</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">runPruning</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="nam">debug</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="str">"""Initialize a HistoricalLetters model."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="com"># Parameters for agents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">population</span> <span class="op">=</span> <span class="nam">population</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">=</span> <span class="nam">moveRange</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">letterRange</span> <span class="op">=</span> <span class="nam">letterRange</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="com"># Parameters for model</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">runPruning</span> <span class="op">=</span> <span class="nam">runPruning</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">useActivation</span> <span class="op">=</span> <span class="nam">useActivation</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">similarityThreshold</span> <span class="op">=</span> <span class="nam">similarityThreshold</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">useSocialNetwork</span> <span class="op">=</span> <span class="nam">useSocialNetwork</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span> <span class="op">=</span> <span class="nam">longRangeNetworkFactor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span> <span class="op">=</span> <span class="nam">shortRangeNetworkFactor</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="com"># Initialize social network</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span> <span class="op">=</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">MultiDiGraph</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="com"># Output variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">letterLedger</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">movements</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="com"># Internal variables</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">time</span><span class="op">.</span><span class="nam">RandomActivation</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">scaleSendInput</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">updatedTopicsDict</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">space</span> <span class="op">=</span> <span class="nam">Nuts2Eu</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">debug</span> <span class="op">=</span> <span class="nam">debug</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="com"># Initialize region agents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="com"># Set up the grid with patches for every NUTS region</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com"># Create region agents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">ac</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">AgentCreator</span><span class="op">(</span><span class="nam">RegionAgent</span><span class="op">,</span> <span class="nam">model</span><span class="op">=</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">regions</span> <span class="op">=</span> <span class="nam">ac</span><span class="op">.</span><span class="nam">from_file</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">            <span class="nam">regionData</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">            <span class="nam">unique_id</span><span class="op">=</span><span class="str">"NUTS_ID"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="com"># Add regions to Nuts2Eu geospace</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">add_regions</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">regions</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">        <span class="com"># Initialize sender agents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="com">#######</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="com"># Draw initial geographic positions of agents</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="nam">initSenderGeoDf</span> <span class="op">=</span> <span class="nam">createData</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">            <span class="nam">population</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">            <span class="nam">populationDistribution</span><span class="op">=</span><span class="nam">populationDistributionData</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="com"># Calculate mean of mean distances for each agent.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="com"># This is used as a measure for the range of exchanges.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="nam">meandistances</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span> <span class="key">in</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">index</span><span class="op">.</span><span class="nam">to_numpy</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="nam">name</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">loc</span><span class="op">[</span><span class="nam">idx</span><span class="op">,</span> <span class="str">"unique_id"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">            <span class="nam">geom</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">loc</span><span class="op">[</span><span class="nam">idx</span><span class="op">,</span> <span class="str">"geometry"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">            <span class="nam">otherAgents</span> <span class="op">=</span> <span class="nam">initSenderGeoDf</span><span class="op">.</span><span class="nam">query</span><span class="op">(</span><span class="str">f"unique_id != '{name}'"</span><span class="op">)</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">            <span class="nam">geometries</span> <span class="op">=</span> <span class="nam">otherAgents</span><span class="op">.</span><span class="nam">geometry</span><span class="op">.</span><span class="nam">to_numpy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="nam">distances</span> <span class="op">=</span> <span class="op">[</span><span class="nam">geom</span><span class="op">.</span><span class="nam">distance</span><span class="op">(</span><span class="nam">othergeom</span><span class="op">)</span> <span class="key">for</span> <span class="nam">othergeom</span> <span class="key">in</span> <span class="nam">geometries</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">            <span class="nam">meandistances</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">mean</span><span class="op">(</span><span class="nam">distances</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">meandistance</span> <span class="op">=</span> <span class="nam">mean</span><span class="op">(</span><span class="nam">meandistances</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="com"># Populate factors dictionary</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">factors</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="str">"similarityThreshold"</span><span class="op">:</span> <span class="nam">similarityThreshold</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">moveRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">            <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">letterRange</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">        <span class="com"># Set up agent creator for senders</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">ac_senders</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">AgentCreator</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">            <span class="nam">SenderAgent</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">            <span class="nam">model</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">agent_kwargs</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">factors</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="com"># Create agents based on random coordinates generated</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="com"># in the createData step above, see util.py file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">senders</span> <span class="op">=</span> <span class="nam">ac_senders</span><span class="op">.</span><span class="nam">from_GeoDataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="nam">initSenderGeoDf</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="nam">unique_id</span><span class="op">=</span><span class="str">"unique_id"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="com"># Create random set of initial topic vectors.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="nam">topics</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">            <span class="nam">tuple</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                <span class="op">[</span><span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">3</span><span class="op">)</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">population</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="com"># Setup senders</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">        <span class="key">for</span> <span class="nam">idx</span><span class="op">,</span> <span class="nam">sender</span> <span class="key">in</span> <span class="nam">enumerate</span><span class="op">(</span><span class="nam">senders</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="com"># Add to social network</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">.</span><span class="nam">add_node</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                <span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                <span class="nam">numLettersSend</span><span class="op">=</span><span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                <span class="nam">numLettersReceived</span><span class="op">=</span><span class="num">0</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">            <span class="com"># Give sender topic</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="nam">sender</span><span class="op">.</span><span class="nam">topicVec</span> <span class="op">=</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">idx</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">            <span class="com"># Add current topic to dict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">updatedTopicsDict</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                <span class="op">{</span><span class="nam">sender</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">topics</span><span class="op">[</span><span class="nam">idx</span><span class="op">]</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">            <span class="com"># Set random activation weight</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">            <span class="key">if</span> <span class="nam">useActivation</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">                <span class="nam">sender</span><span class="op">.</span><span class="nam">activationWeight</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">random</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="com"># Add sender to its region</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">            <span class="nam">regionID</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">                <span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">regions</span> <span class="key">if</span> <span class="nam">contains</span><span class="op">(</span><span class="nam">x</span><span class="op">.</span><span class="nam">geometry</span><span class="op">,</span> <span class="nam">sender</span><span class="op">.</span><span class="nam">geometry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">            <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">add_sender</span><span class="op">(</span><span class="nam">sender</span><span class="op">,</span> <span class="nam">regionID</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">            <span class="key">except</span> <span class="nam">IndexError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">                <span class="nam">text</span> <span class="op">=</span> <span class="str">f"Problem finding region for {sender.geometry}."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">                <span class="key">raise</span> <span class="nam">IndexError</span><span class="op">(</span><span class="nam">text</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">            <span class="com"># Add sender to schedule</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">sender</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="com"># Create social network</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">if</span> <span class="nam">useSocialNetwork</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="key">for</span> <span class="nam">agent</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">                <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">_createSocialEdges</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">socialNetwork</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">DataCollector</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">model_reporters</span><span class="op">=</span><span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">                <span class="str">"Ledger"</span><span class="op">:</span> <span class="nam">getPrunedLedger</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">                <span class="str">"Letters"</span><span class="op">:</span> <span class="nam">getScaledLetters</span> <span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">                <span class="str">"Movements"</span><span class="op">:</span> <span class="nam">getScaledMovements</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">                <span class="str">"Clusters"</span><span class="op">:</span> <span class="nam">getComponents</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="str">        For all other agents, that are not in this closeRange group,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">        create a connection with the probability set by the longRangeNetworkFactor.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">        <span class="nam">closerange</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors_within_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="nam">agent</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">            <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="nam">center</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">for</span> <span class="nam">neighbor</span> <span class="key">in</span> <span class="nam">closerange</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">!=</span> <span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                <span class="nam">connect</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                    <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="key">True</span><span class="op">,</span> <span class="key">False</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                    <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span><span class="op">,</span> <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                    <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                <span class="key">if</span> <span class="nam">connect</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                    <span class="nam">graph</span><span class="op">.</span><span class="nam">add_edge</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">step</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="nam">longrange</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span> <span class="key">if</span> <span class="nam">x</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">closerange</span> <span class="key">and</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">        <span class="key">for</span> <span class="nam">neighbor</span> <span class="key">in</span> <span class="nam">longrange</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">!=</span> <span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                <span class="nam">connect</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                    <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="key">True</span><span class="op">,</span> <span class="key">False</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                    <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span><span class="op">,</span> <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                    <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">                <span class="key">if</span> <span class="nam">connect</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">                    <span class="nam">graph</span><span class="op">.</span><span class="nam">add_edge</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">step</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="key">def</span> <span class="nam">step</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="str">"""One simulation step."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">scaleSendInput</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">            <span class="op">**</span><span class="op">{</span><span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">x</span><span class="op">.</span><span class="nam">numLettersReceived</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">step</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span><span class="op">.</span><span class="nam">collect</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="key">def</span> <span class="nam">step_no_data</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="str">"""One simulation step without datacollection."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">scaleSendInput</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">            <span class="op">**</span><span class="op">{</span><span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">x</span><span class="op">.</span><span class="nam">numLettersReceived</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">step</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">n</span><span class="op">:</span><span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="str">"""Run the model for n steps."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">debug</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">tqdm</span><span class="op">(</span><span class="nam">range</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">step_no_data</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">step_no_data</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span><span class="op">.</span><span class="nam">collect</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="key">def</span> <span class="nam">_createSocialEdges</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">agent</span><span class="op">:</span> <span class="nam">SenderAgent</span><span class="op">,</span> <span class="nam">graph</span><span class="op">:</span> <span class="nam">nx</span><span class="op">.</span><span class="nam">MultiDiGraph</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="str">"""Create social edges with the different wiring factors.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">        Define a close range by using the moveRange parameter. Among</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t"><span class="str">        these neighbors, create a connection with probability set by</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">        the shortRangeNetworkFactor.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">        For all other agents, that are not in this closeRange group,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        create a connection with the probability set by the longRangeNetworkFactor.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">        <span class="nam">closerange</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">space</span><span class="op">.</span><span class="nam">get_neighbors_within_distance</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">            <span class="nam">agent</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">            <span class="nam">distance</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">moveRange</span> <span class="op">*</span> <span class="nam">self</span><span class="op">.</span><span class="nam">meandistance</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">            <span class="nam">center</span><span class="op">=</span><span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">        <span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">for</span> <span class="nam">neighbor</span> <span class="key">in</span> <span class="nam">closerange</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">!=</span> <span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                <span class="nam">connect</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                    <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="key">True</span><span class="op">,</span> <span class="key">False</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                    <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span><span class="op">,</span> <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">shortRangeNetworkFactor</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                    <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">                <span class="key">if</span> <span class="nam">connect</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">                    <span class="nam">graph</span><span class="op">.</span><span class="nam">add_edge</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">step</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">        <span class="nam">longrange</span> <span class="op">=</span> <span class="op">[</span><span class="nam">x</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span> <span class="key">if</span> <span class="nam">x</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">closerange</span> <span class="key">and</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="key">for</span> <span class="nam">neighbor</span> <span class="key">in</span> <span class="nam">longrange</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">            <span class="key">if</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span> <span class="op">!=</span> <span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">                <span class="nam">connect</span> <span class="op">=</span> <span class="nam">random</span><span class="op">.</span><span class="nam">choices</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                    <span class="nam">population</span><span class="op">=</span><span class="op">[</span><span class="key">True</span><span class="op">,</span> <span class="key">False</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                    <span class="nam">weights</span><span class="op">=</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span><span class="op">,</span> <span class="num">1</span> <span class="op">-</span> <span class="nam">self</span><span class="op">.</span><span class="nam">longRangeNetworkFactor</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                    <span class="nam">k</span><span class="op">=</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">                <span class="key">if</span> <span class="nam">connect</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">                    <span class="nam">graph</span><span class="op">.</span><span class="nam">add_edge</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">neighbor</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">,</span> <span class="nam">step</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="key">def</span> <span class="nam">step</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="str">"""One simulation step with data collection."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">step_no_data</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span><span class="op">.</span><span class="nam">collect</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="key">def</span> <span class="nam">step_no_data</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="str">"""One simulation step without data collection."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">scaleSendInput</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">            <span class="op">**</span><span class="op">{</span><span class="nam">x</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">:</span> <span class="nam">x</span><span class="op">.</span><span class="nam">numLettersReceived</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="com"># Update the currently held topicVec for each agent, based</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="com"># on potential previouse communication events.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">        <span class="key">for</span> <span class="nam">agent</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">agents</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">            <span class="nam">agent</span><span class="op">.</span><span class="nam">topicVec</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">updatedTopicsDict</span><span class="op">[</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">schedule</span><span class="op">.</span><span class="nam">step</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">    <span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">n</span><span class="op">:</span><span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">        <span class="str">"""Run the model for n steps.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="str">        Data collection is only run at the end of n steps.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t"><span class="str">        This is useful for batch runs accross different</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t"><span class="str">        parameters.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">debug</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">tqdm</span><span class="op">(</span><span class="nam">range</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">step_no_data</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">            <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="nam">n</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">step_no_data</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">datacollector</span><span class="op">.</span><span class="nam">collect</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_interface_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_server_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_interface_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 13:48 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-hhiissttoorriiccaalllleetttteerrss//mmooddeell..ppyy:: 9944%% ************
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+hhiissttoorriiccaalllleetttteerrss//mmooddeell..ppyy:: 9955%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 110088 ssttaatteemmeennttss ?  110022 rruunn 66 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+********** 111100 ssttaatteemmeennttss ?  110055 rruunn 55 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 13:48 +0200
 _1"""The model class for HistoricalLetters.""" 
 _2import random 
 _3from pathlib import Path 
 _4 
 _5import mesa 
 _6import mesa_geo as mg 
 _7import networkx as nx 
@@ -31,287 +31,301 @@
 _1_7 
 _1_8 
 _1_9def getPrunedLedger(model: mesa.Model) -> pd.DataFrame: 
 _2_0 """Model reporter for simulation of archiving. 
 _2_1 
 _2_2 Returns statistics of ledger network of model run 
 _2_3 and various iterations of statistics of pruned networks. 
-_2_4 """ 
-_2_5 # TODO(malte): Add all model params 
-_2_6 if model.runPruning is True: 
-_2_7 ledgerColumns = ["sender", "receiver", "sender_location",
+_2_4 
+_2_5 The routine assumes that the network contains fields of sender, 
+_2_6 receiver and step information. 
+_2_7 """ 
+_2_8 if model.runPruning is True: 
+_2_9 ledgerColumns = ["sender", "receiver", "sender_location",
 "receiver_location", "topic", "step"] 
-_2_8 modelparams = { 
-_2_9 "population": model.population, 
-_3_0 "moveRange": model.moveRange, 
-_3_1 "letterRange": model.letterRange, 
-_3_2 "useActivation": model.useActivation, 
-_3_3 "useSocialNetwork": model.useSocialNetwork, 
-_3_4 } 
-_3_5 result = prune( 
-_3_6 modelparameters=modelparams, 
-_3_7 network=model.letterLedger, 
-_3_8 columns=ledgerColumns, 
-_3_9 ) 
-_4_0 else: 
-_4_1 result = model.letterLedger 
-_4_2 return result 
-_4_3 
-_4_4 
-_4_5def getComponents(model: mesa.Model) -> int: 
-_4_6 """Model reporter to get number of components. 
-_4_7 
-_4_8 The MultiDiGraph is converted to undirected, 
-_4_9 considering only edges that are reciprocal, ie. 
-_5_0 edges are established if sender and receiver have 
-_5_1 exchanged at least a letter in each direction. 
-_5_2 """ 
-_5_3 newg = model.socialNetwork.to_undirected(reciprocal=True) 
-_5_4 return nx.number_connected_components(newg) 
-_5_5 
-_5_6 
-_5_7def getScaledLetters(model: mesa.Model) -> float: 
-_5_8 """Return relative number of send letters.""" 
-_5_9 return len(model.letterLedger)/model.schedule.time 
-_6_0 
-_6_1 
-_6_2def getScaledMovements(model: mesa.Model) -> float: 
-_6_3 """Return relative number of movements.""" 
-_6_4 return model.movements/model.schedule.time 
+_3_0 modelparams = { 
+_3_1 "population": model.population, 
+_3_2 "moveRange": model.moveRange, 
+_3_3 "letterRange": model.letterRange, 
+_3_4 "useActivation": model.useActivation, 
+_3_5 "useSocialNetwork": model.useSocialNetwork, 
+_3_6 "similarityThreshold": model.similarityThreshold, 
+_3_7 "longRangeNetworkFactor": model.longRangeNetworkFactor, 
+_3_8 "shortRangeNetworkFactor": model.shortRangeNetworkFactor, 
+_3_9 } 
+_4_0 result = prune( 
+_4_1 modelparameters=modelparams, 
+_4_2 network=model.letterLedger, 
+_4_3 columns=ledgerColumns, 
+_4_4 iterations=3, 
+_4_5 delAmounts=(0.1, 0.25, 0.5, 0.75, 0.9), 
+_4_6 delTypes=("unif", "exp", "beta", "log_normal1", "log_normal2",
+"log_normal3"), 
+_4_7 delMethod=("agents", "regions", "time"), 
+_4_8 rankedVals=(True, False), 
+_4_9 ) 
+_5_0 else: 
+_5_1 result = model.letterLedger 
+_5_2 return result 
+_5_3 
+_5_4 
+_5_5def getComponents(model: mesa.Model) -> int: 
+_5_6 """Model reporter to get number of components. 
+_5_7 
+_5_8 The MultiDiGraph is converted to undirected, 
+_5_9 considering only edges that are reciprocal, ie. 
+_6_0 edges are established if sender and receiver have 
+_6_1 exchanged at least a letter in each direction. 
+_6_2 """ 
+_6_3 newg = model.socialNetwork.to_undirected(reciprocal=True) 
+_6_4 return nx.number_connected_components(newg) 
 _6_5 
 _6_6 
-_6_7class HistoricalLetters(mesa.Model): 
-_6_8 """A letter sending model with historical informed initital positions. 
-_6_9 
-_7_0 Each agent has an initial topic vector, expressed as a RGB value. The 
-_7_1 initial positions of the agents is based on a weighted random draw 
-_7_2 based on data from [1]. 
-_7_3 
-_7_4 Each step, agents generate two neighbourhoods for sending letters and 
-_7_5 potential targets to move towards. The probability to send letters is 
-_7_6 a self-reinforcing process. During each sending the internal topic of 
-_7_7 the sender is updated as a random rotation towards the receivers topic. 
-_7_8 
-_7_9 [1] J. Lobo et al, Population-Area Relationship for Medieval European
+_6_7def getScaledLetters(model: mesa.Model) -> float: 
+_6_8 """Return relative number of send letters.""" 
+_6_9 return len(model.letterLedger)/model.schedule.time 
+_7_0 
+_7_1 
+_7_2def getScaledMovements(model: mesa.Model) -> float: 
+_7_3 """Return relative number of movements.""" 
+_7_4 return model.movements/model.schedule.time 
+_7_5 
+_7_6 
+_7_7class HistoricalLetters(mesa.Model): 
+_7_8 """A letter sending model with historical informed initital positions. 
+_7_9 
+_8_0 Each agent has an initial topic vector, expressed as a RGB value. The 
+_8_1 initial positions of the agents is based on a weighted random draw 
+_8_2 based on data from [1]. 
+_8_3 
+_8_4 Each step, agents generate two neighbourhoods for sending letters and 
+_8_5 potential targets to move towards. The probability to send letters is 
+_8_6 a self-reinforcing process. During each sending the internal topic of 
+_8_7 the sender is updated as a random rotation towards the receivers topic. 
+_8_8 
+_8_9 [1] J. Lobo et al, Population-Area Relationship for Medieval European
 Cities, 
-_8_0 PLoS ONE 11(10): e0162678. 
-_8_1 """ 
-_8_2 
-_8_3 def __init__( 
-_8_4 self, 
-_8_5 population: int = 100, 
-_8_6 moveRange: float = 0.05, 
-_8_7 letterRange: float = 0.2, 
-_8_8 similarityThreshold: float = 0.2, 
-_8_9 longRangeNetworkFactor: float = 0.3, 
-_9_0 shortRangeNetworkFactor: float = 0.4, 
-_9_1 regionData: str = Path(Path(__file__).parent.parent.resolve(), "data/
+_9_0 PLoS ONE 11(10): e0162678. 
+_9_1 """ 
+_9_2 
+_9_3 def __init__( 
+_9_4 self, 
+_9_5 population: int = 100, 
+_9_6 moveRange: float = 0.05, 
+_9_7 letterRange: float = 0.2, 
+_9_8 similarityThreshold: float = 0.2, 
+_9_9 longRangeNetworkFactor: float = 0.3, 
+_1_0_0 shortRangeNetworkFactor: float = 0.4, 
+_1_0_1 regionData: str = Path(Path(__file__).parent.parent.resolve(), "data/
 NUTS_RG_60M_2021_3857_LEVL_2.geojson"), 
-_9_2 populationDistributionData: str = Path(Path(__file__).parent.parent.resolve
+_1_0_2 populationDistributionData: str = Path(Path(__file__).parent.parent.resolve
 (), "data/pone.0162678.s003.csv"), 
-_9_3 *, 
-_9_4 useActivation: bool = False, 
-_9_5 useSocialNetwork: bool = False, 
-_9_6 runPruning: bool = False, 
-_9_7 debug: bool = False, 
-_9_8 ) -> None: 
-_9_9 """Initialize a HistoricalLetters model.""" 
-_1_0_0 super().__init__() 
-_1_0_1 
-_1_0_2 # Parameters for agents 
-_1_0_3 self.population = population 
-_1_0_4 self.moveRange = moveRange 
-_1_0_5 self.letterRange = letterRange 
-_1_0_6 # Parameters for model 
-_1_0_7 self.runPruning = runPruning 
-_1_0_8 self.useActivation = useActivation 
-_1_0_9 self.useSocialNetwork = useSocialNetwork 
-_1_1_0 self.longRangeNetworkFactor = longRangeNetworkFactor 
-_1_1_1 self.shortRangeNetworkFactor = shortRangeNetworkFactor 
-_1_1_2 # Initialize social network 
-_1_1_3 self.socialNetwork = nx.MultiDiGraph() 
-_1_1_4 # Output variables 
-_1_1_5 self.letterLedger = [] 
-_1_1_6 self.movements = 0 
-_1_1_7 # Internal variables 
-_1_1_8 self.schedule = mesa.time.RandomActivation(self) 
-_1_1_9 self.scaleSendInput = {} 
-_1_2_0 self.updatedTopicsDict = {} 
-_1_2_1 self.space = Nuts2Eu() 
-_1_2_2 self.debug = debug 
-_1_2_3 
-_1_2_4 ####### 
-_1_2_5 # Initialize region agents 
-_1_2_6 ####### 
-_1_2_7 
-_1_2_8 # Set up the grid with patches for every NUTS region 
-_1_2_9 # Create region agents 
-_1_3_0 ac = mg.AgentCreator(RegionAgent, model=self) 
-_1_3_1 self.regions = ac.from_file( 
-_1_3_2 regionData, 
-_1_3_3 unique_id="NUTS_ID", 
-_1_3_4 ) 
-_1_3_5 # Add regions to Nuts2Eu geospace 
-_1_3_6 self.space.add_regions(self.regions) 
-_1_3_7 
-_1_3_8 ####### 
-_1_3_9 # Initialize sender agents 
-_1_4_0 ####### 
-_1_4_1 
-_1_4_2 # Draw initial geographic positions of agents 
-_1_4_3 initSenderGeoDf = createData( 
-_1_4_4 population, 
-_1_4_5 populationDistribution=populationDistributionData, 
-_1_4_6 ) 
-_1_4_7 
-_1_4_8 # Calculate mean of mean distances for each agent. 
-_1_4_9 # This is used as a measure for the range of exchanges. 
-_1_5_0 meandistances = [] 
-_1_5_1 for idx in initSenderGeoDf.index.to_numpy(): 
-_1_5_2 name = initSenderGeoDf.loc[idx, "unique_id"] 
-_1_5_3 geom = initSenderGeoDf.loc[idx, "geometry"] 
-_1_5_4 otherAgents = initSenderGeoDf.query(f"unique_id != '{name}'").copy() 
-_1_5_5 geometries = otherAgents.geometry.to_numpy() 
-_1_5_6 distances = [geom.distance(othergeom) for othergeom in geometries] 
-_1_5_7 meandistances.append(mean(distances)) 
-_1_5_8 self.meandistance = mean(meandistances) 
-_1_5_9 
-_1_6_0 # Populate factors dictionary 
-_1_6_1 self.factors = { 
-_1_6_2 "similarityThreshold": similarityThreshold, 
-_1_6_3 "moveRange": moveRange, 
-_1_6_4 "letterRange": letterRange, 
-_1_6_5 } 
-_1_6_6 
-_1_6_7 # Set up agent creator for senders 
-_1_6_8 ac_senders = mg.AgentCreator( 
-_1_6_9 SenderAgent, 
-_1_7_0 model=self, 
-_1_7_1 agent_kwargs=self.factors, 
-_1_7_2 ) 
-_1_7_3 
-_1_7_4 # Create agents based on random coordinates generated 
-_1_7_5 # in the createData step above, see util.py file. 
-_1_7_6 senders = ac_senders.from_GeoDataFrame( 
-_1_7_7 initSenderGeoDf, 
-_1_7_8 unique_id="unique_id", 
-_1_7_9 ) 
-_1_8_0 
-_1_8_1 # Create random set of initial topic vectors. 
-_1_8_2 topics = [ 
-_1_8_3 tuple( 
-_1_8_4 [random.random() for x in range(3)], 
-_1_8_5 ) for x in range(self.population) 
-_1_8_6 ] 
-_1_8_7 
-_1_8_8 # Setup senders 
-_1_8_9 for idx, sender in enumerate(senders): 
-_1_9_0 # Add to social network 
-_1_9_1 self.socialNetwork.add_node( 
-_1_9_2 sender.unique_id, 
-_1_9_3 numLettersSend=0, 
-_1_9_4 numLettersReceived=0, 
-_1_9_5 ) 
-_1_9_6 # Give sender topic 
-_1_9_7 sender.topicVec = topics[idx] 
-_1_9_8 # Add current topic to dict 
-_1_9_9 self.updatedTopicsDict.update( 
-_2_0_0 {sender.unique_id: topics[idx]}, 
-_2_0_1 ) 
-_2_0_2 # Set random activation weight 
-_2_0_3 if useActivation is True: 
-_2_0_4 sender.activationWeight = random.random() 
-_2_0_5 # Add sender to its region 
-_2_0_6 regionID = [ 
-_2_0_7 x.unique_id for x in self.regions if contains(x.geometry, sender.geometry) 
-_2_0_8 ] 
-_2_0_9 try: 
-_2_1_0 self.space.add_sender(sender, regionID[0]) 
-_2_1_1 except IndexError as exc: 
-_2_1_2 text = f"Problem finding region for {sender.geometry}." 
-_2_1_3 raise IndexError(text) from exc 
-_2_1_4 # Add sender to schedule 
-_2_1_5 self.schedule.add(sender) 
-_2_1_6 
-_2_1_7 # Add graph to network grid for potential visualization. 
-_2_1_8 # TODO(malte): Not yet implemented. Maybe use Solara backend for this? 
-_2_1_9 # self.grid = mesa.space.NetworkGrid(self.socialNetwork) 
-_2_2_0 
-_2_2_1 # Create social network 
-_2_2_2 if useSocialNetwork is True: 
-_2_2_3 for agent in self.schedule.agents: 
-_2_2_4 if isinstance(agent, SenderAgent): 
-_2_2_5 self._createSocialEdges(agent, self.socialNetwork) 
-_2_2_6 
-_2_2_7 self.datacollector = mesa.DataCollector( 
-_2_2_8 model_reporters={ 
-_2_2_9 "Ledger": getPrunedLedger, 
-_2_3_0 "Letters": getScaledLetters , 
-_2_3_1 "Movements": getScaledMovements, 
-_2_3_2 "Clusters": getComponents, 
-_2_3_3 }, 
-_2_3_4 ) 
-_2_3_5 
-_2_3_6 def _createSocialEdges(self, agent: SenderAgent, graph: nx.MultiDiGraph) -
-> None: 
-_2_3_7 """Create social edges with the different wiring factors. 
-_2_3_8 
-_2_3_9 Define a close range by using the moveRange parameter. Among 
-_2_4_0 these neighbors, create a connection with probability set by 
-_2_4_1 the shortRangeNetworkFactor. 
+_1_0_3 *, 
+_1_0_4 useActivation: bool = False, 
+_1_0_5 useSocialNetwork: bool = False, 
+_1_0_6 runPruning: bool = False, 
+_1_0_7 debug: bool = False, 
+_1_0_8 ) -> None: 
+_1_0_9 """Initialize a HistoricalLetters model.""" 
+_1_1_0 super().__init__() 
+_1_1_1 
+_1_1_2 # Parameters for agents 
+_1_1_3 self.population = population 
+_1_1_4 self.moveRange = moveRange 
+_1_1_5 self.letterRange = letterRange 
+_1_1_6 # Parameters for model 
+_1_1_7 self.runPruning = runPruning 
+_1_1_8 self.useActivation = useActivation 
+_1_1_9 self.similarityThreshold = similarityThreshold 
+_1_2_0 self.useSocialNetwork = useSocialNetwork 
+_1_2_1 self.longRangeNetworkFactor = longRangeNetworkFactor 
+_1_2_2 self.shortRangeNetworkFactor = shortRangeNetworkFactor 
+_1_2_3 # Initialize social network 
+_1_2_4 self.socialNetwork = nx.MultiDiGraph() 
+_1_2_5 # Output variables 
+_1_2_6 self.letterLedger = [] 
+_1_2_7 self.movements = 0 
+_1_2_8 # Internal variables 
+_1_2_9 self.schedule = mesa.time.RandomActivation(self) 
+_1_3_0 self.scaleSendInput = {} 
+_1_3_1 self.updatedTopicsDict = {} 
+_1_3_2 self.space = Nuts2Eu() 
+_1_3_3 self.debug = debug 
+_1_3_4 
+_1_3_5 ####### 
+_1_3_6 # Initialize region agents 
+_1_3_7 ####### 
+_1_3_8 
+_1_3_9 # Set up the grid with patches for every NUTS region 
+_1_4_0 # Create region agents 
+_1_4_1 ac = mg.AgentCreator(RegionAgent, model=self) 
+_1_4_2 self.regions = ac.from_file( 
+_1_4_3 regionData, 
+_1_4_4 unique_id="NUTS_ID", 
+_1_4_5 ) 
+_1_4_6 # Add regions to Nuts2Eu geospace 
+_1_4_7 self.space.add_regions(self.regions) 
+_1_4_8 
+_1_4_9 ####### 
+_1_5_0 # Initialize sender agents 
+_1_5_1 ####### 
+_1_5_2 
+_1_5_3 # Draw initial geographic positions of agents 
+_1_5_4 initSenderGeoDf = createData( 
+_1_5_5 population, 
+_1_5_6 populationDistribution=populationDistributionData, 
+_1_5_7 ) 
+_1_5_8 
+_1_5_9 # Calculate mean of mean distances for each agent. 
+_1_6_0 # This is used as a measure for the range of exchanges. 
+_1_6_1 meandistances = [] 
+_1_6_2 for idx in initSenderGeoDf.index.to_numpy(): 
+_1_6_3 name = initSenderGeoDf.loc[idx, "unique_id"] 
+_1_6_4 geom = initSenderGeoDf.loc[idx, "geometry"] 
+_1_6_5 otherAgents = initSenderGeoDf.query(f"unique_id != '{name}'").copy() 
+_1_6_6 geometries = otherAgents.geometry.to_numpy() 
+_1_6_7 distances = [geom.distance(othergeom) for othergeom in geometries] 
+_1_6_8 meandistances.append(mean(distances)) 
+_1_6_9 self.meandistance = mean(meandistances) 
+_1_7_0 
+_1_7_1 # Populate factors dictionary 
+_1_7_2 self.factors = { 
+_1_7_3 "similarityThreshold": similarityThreshold, 
+_1_7_4 "moveRange": moveRange, 
+_1_7_5 "letterRange": letterRange, 
+_1_7_6 } 
+_1_7_7 
+_1_7_8 # Set up agent creator for senders 
+_1_7_9 ac_senders = mg.AgentCreator( 
+_1_8_0 SenderAgent, 
+_1_8_1 model=self, 
+_1_8_2 agent_kwargs=self.factors, 
+_1_8_3 ) 
+_1_8_4 
+_1_8_5 # Create agents based on random coordinates generated 
+_1_8_6 # in the createData step above, see util.py file. 
+_1_8_7 senders = ac_senders.from_GeoDataFrame( 
+_1_8_8 initSenderGeoDf, 
+_1_8_9 unique_id="unique_id", 
+_1_9_0 ) 
+_1_9_1 
+_1_9_2 # Create random set of initial topic vectors. 
+_1_9_3 topics = [ 
+_1_9_4 tuple( 
+_1_9_5 [random.random() for x in range(3)], 
+_1_9_6 ) for x in range(self.population) 
+_1_9_7 ] 
+_1_9_8 
+_1_9_9 # Setup senders 
+_2_0_0 for idx, sender in enumerate(senders): 
+_2_0_1 # Add to social network 
+_2_0_2 self.socialNetwork.add_node( 
+_2_0_3 sender.unique_id, 
+_2_0_4 numLettersSend=0, 
+_2_0_5 numLettersReceived=0, 
+_2_0_6 ) 
+_2_0_7 # Give sender topic 
+_2_0_8 sender.topicVec = topics[idx] 
+_2_0_9 # Add current topic to dict 
+_2_1_0 self.updatedTopicsDict.update( 
+_2_1_1 {sender.unique_id: topics[idx]}, 
+_2_1_2 ) 
+_2_1_3 # Set random activation weight 
+_2_1_4 if useActivation is True: 
+_2_1_5 sender.activationWeight = random.random() 
+_2_1_6 # Add sender to its region 
+_2_1_7 regionID = [ 
+_2_1_8 x.unique_id for x in self.regions if contains(x.geometry, sender.geometry) 
+_2_1_9 ] 
+_2_2_0 try: 
+_2_2_1 self.space.add_sender(sender, regionID[0]) 
+_2_2_2 except IndexError as exc: 
+_2_2_3 text = f"Problem finding region for {sender.geometry}." 
+_2_2_4 raise IndexError(text) from exc 
+_2_2_5 # Add sender to schedule 
+_2_2_6 self.schedule.add(sender) 
+_2_2_7 
+_2_2_8 # Create social network 
+_2_2_9 if useSocialNetwork is True: 
+_2_3_0 for agent in self.schedule.agents: 
+_2_3_1 if isinstance(agent, SenderAgent): 
+_2_3_2 self._createSocialEdges(agent, self.socialNetwork) 
+_2_3_3 
+_2_3_4 self.datacollector = mesa.DataCollector( 
+_2_3_5 model_reporters={ 
+_2_3_6 "Ledger": getPrunedLedger, 
+_2_3_7 "Letters": getScaledLetters , 
+_2_3_8 "Movements": getScaledMovements, 
+_2_3_9 "Clusters": getComponents, 
+_2_4_0 }, 
+_2_4_1 ) 
 _2_4_2 
-_2_4_3 For all other agents, that are not in this closeRange group, 
-_2_4_4 create a connection with the probability set by the
+_2_4_3 def _createSocialEdges(self, agent: SenderAgent, graph: nx.MultiDiGraph) -
+> None: 
+_2_4_4 """Create social edges with the different wiring factors. 
+_2_4_5 
+_2_4_6 Define a close range by using the moveRange parameter. Among 
+_2_4_7 these neighbors, create a connection with probability set by 
+_2_4_8 the shortRangeNetworkFactor. 
+_2_4_9 
+_2_5_0 For all other agents, that are not in this closeRange group, 
+_2_5_1 create a connection with the probability set by the
 longRangeNetworkFactor. 
-_2_4_5 """ 
-_2_4_6 closerange = [x for x in self.space.get_neighbors_within_distance( 
-_2_4_7 agent, 
-_2_4_8 distance=self.moveRange * self.meandistance, 
-_2_4_9 center=False, 
-_2_5_0 ) if isinstance(x, SenderAgent)] 
-_2_5_1 for neighbor in closerange: 
-_2_5_2 if neighbor.unique_id != agent.unique_id: 
-_2_5_3 connect = random.choices( 
-_2_5_4 population=[True, False], 
-_2_5_5 weights=[self.shortRangeNetworkFactor, 1 - self.shortRangeNetworkFactor], 
-_2_5_6 k=1, 
-_2_5_7 ) 
-_2_5_8 if connect[0] is True: 
-_2_5_9 graph.add_edge(agent.unique_id, neighbor.unique_id, step=0) 
-_2_6_0 longrange = [x for x in self.schedule.agents if x not in closerange and
+_2_5_2 """ 
+_2_5_3 closerange = [x for x in self.space.get_neighbors_within_distance( 
+_2_5_4 agent, 
+_2_5_5 distance=self.moveRange * self.meandistance, 
+_2_5_6 center=False, 
+_2_5_7 ) if isinstance(x, SenderAgent)] 
+_2_5_8 for neighbor in closerange: 
+_2_5_9 if neighbor.unique_id != agent.unique_id: 
+_2_6_0 connect = random.choices( 
+_2_6_1 population=[True, False], 
+_2_6_2 weights=[self.shortRangeNetworkFactor, 1 - self.shortRangeNetworkFactor], 
+_2_6_3 k=1, 
+_2_6_4 ) 
+_2_6_5 if connect[0] is True: 
+_2_6_6 graph.add_edge(agent.unique_id, neighbor.unique_id, step=0) 
+_2_6_7 longrange = [x for x in self.schedule.agents if x not in closerange and
 isinstance(x, SenderAgent)] 
-_2_6_1 for neighbor in longrange: 
-_2_6_2 if neighbor.unique_id != agent.unique_id: 
-_2_6_3 connect = random.choices( 
-_2_6_4 population=[True, False], 
-_2_6_5 weights=[self.longRangeNetworkFactor, 1 - self.longRangeNetworkFactor], 
-_2_6_6 k=1, 
-_2_6_7 ) 
-_2_6_8 if connect[0] is True: 
-_2_6_9 graph.add_edge(agent.unique_id, neighbor.unique_id, step=0) 
-_2_7_0 
-_2_7_1 def step(self) -> None: 
-_2_7_2 """One simulation step.""" 
-_2_7_3 self.scaleSendInput.update( 
-_2_7_4 **{x.unique_id: x.numLettersReceived for x in self.schedule.agents}, 
-_2_7_5 ) 
-_2_7_6 self.schedule.step() 
-_2_7_7 self.datacollector.collect(self) 
-_2_7_8 
-_2_7_9 def step_no_data(self) -> None: 
-_2_8_0 """One simulation step without datacollection.""" 
-_2_8_1 self.scaleSendInput.update( 
-_2_8_2 **{x.unique_id: x.numLettersReceived for x in self.schedule.agents}, 
-_2_8_3 ) 
-_2_8_4 self.schedule.step() 
-_2_8_5 
-_2_8_6 def run(self, n:int) -> None: 
-_2_8_7 """Run the model for n steps.""" 
-_2_8_8 if self.debug is True: 
-_2_8_9 for _ in tqdm(range(n)): 
-_2_9_0 self.step_no_data() 
-_2_9_1 else: 
-_2_9_2 for _ in range(n): 
-_2_9_3 self.step_no_data() 
-_2_9_4 self.datacollector.collect(self) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+_2_6_8 for neighbor in longrange: 
+_2_6_9 if neighbor.unique_id != agent.unique_id: 
+_2_7_0 connect = random.choices( 
+_2_7_1 population=[True, False], 
+_2_7_2 weights=[self.longRangeNetworkFactor, 1 - self.longRangeNetworkFactor], 
+_2_7_3 k=1, 
+_2_7_4 ) 
+_2_7_5 if connect[0] is True: 
+_2_7_6 graph.add_edge(agent.unique_id, neighbor.unique_id, step=0) 
+_2_7_7 
+_2_7_8 def step(self) -> None: 
+_2_7_9 """One simulation step with data collection.""" 
+_2_8_0 self.step_no_data() 
+_2_8_1 self.datacollector.collect(self) 
+_2_8_2 
+_2_8_3 def step_no_data(self) -> None: 
+_2_8_4 """One simulation step without data collection.""" 
+_2_8_5 self.scaleSendInput.update( 
+_2_8_6 **{x.unique_id: x.numLettersReceived for x in self.schedule.agents}, 
+_2_8_7 ) 
+_2_8_8 # Update the currently held topicVec for each agent, based 
+_2_8_9 # on potential previouse communication events. 
+_2_9_0 for agent in self.schedule.agents: 
+_2_9_1 agent.topicVec = self.updatedTopicsDict[agent.unique_id] 
+_2_9_2 self.schedule.step() 
+_2_9_3 
+_2_9_4 def run(self, n:int) -> None: 
+_2_9_5 """Run the model for n steps. 
+_2_9_6 
+_2_9_7 Data collection is only run at the end of n steps. 
+_2_9_8 This is useful for batch runs accross different 
+_2_9_9 parameters. 
+_3_0_0 """ 
+_3_0_1 if self.debug is True: 
+_3_0_2 for _ in tqdm(range(n)): 
+_3_0_3 self.step_no_data() 
+_3_0_4 else: 
+_3_0_5 for _ in range(n): 
+_3_0_6 self.step_no_data() 
+_3_0_7 self.datacollector.collect(self) 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 13:48 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_server_py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe_server_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/server.py: 100%</title>
+    <title>Coverage for src/scicom/historicalletters/server.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/server.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="text">Coverage for </span><b>src/scicom/historicalletters/server.py</b>:
+            <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -50,134 +50,132 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">22 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">22<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <span class="text">26 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">26<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_444d8314c29d6cbe_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_space_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_444d8314c29d6cbe_space_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""A visualization interface for HistoricalLetters using the older visualization option of mesa."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa_geo</span> <span class="key">as</span> <span class="nam">mg</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">matplotlib</span> <span class="key">import</span> <span class="nam">colors</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">modules</span> <span class="key">import</span> <span class="nam">ChartVisualization</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">matplotlib</span><span class="op">.</span><span class="nam">colors</span> <span class="key">as</span> <span class="nam">colors</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa_geo</span> <span class="key">as</span> <span class="nam">mg</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">modules</span> <span class="key">import</span> <span class="nam">ChartVisualization</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">historicalletters</span><span class="op">.</span><span class="nam">agents</span> <span class="key">import</span> <span class="nam">RegionAgent</span><span class="op">,</span> <span class="nam">SenderAgent</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">historicalletters</span><span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">HistoricalLetters</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">historicalletters</span><span class="op">.</span><span class="nam">agents</span> <span class="key">import</span> <span class="nam">SenderAgent</span><span class="op">,</span> <span class="nam">RegionAgent</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">historicalletters</span><span class="op">.</span><span class="nam">model</span> <span class="key">import</span> <span class="nam">HistoricalLetters</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">model_params</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="str">"population"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="str">"Number of persons"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="num">50</span><span class="op">,</span> <span class="num">10</span><span class="op">,</span> <span class="num">100</span><span class="op">,</span> <span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose how many senders to include in the model."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"useSocialNetwork"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Checkbox</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">"Create initial social network of agents"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="str">"useActivation"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Checkbox</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="str">"Use heterogenous activations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"similarityThreshold"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="str">"Similarity threshold"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="num">0.5</span><span class="op">,</span> <span class="num">0.0</span><span class="op">,</span> <span class="num">1.0</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose how similar two agents topics have to be, to send a letter."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="str">"Range for moving position&lt;/br>(% of mean agent distances)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="num">0.01</span><span class="op">,</span> <span class="num">0.00</span><span class="op">,</span> <span class="num">0.5</span><span class="op">,</span> <span class="num">0.05</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose the visibility range for finding potential locations to move to."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="str">"Range for letter sending&lt;/br>(% of mean agent distances)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="num">0.2</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span> <span class="num">1.0</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose the visibility range for finding potential recipients."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">model_params</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="com">#"population": 100,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="str">"population"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">         <span class="str">"Number of persons"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">         <span class="num">50</span><span class="op">,</span> <span class="num">10</span><span class="op">,</span> <span class="num">100</span><span class="op">,</span> <span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">         <span class="nam">description</span><span class="op">=</span><span class="str">"Choose how many senders to include in the model."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">     <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="str">"useSocialNetwork"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Checkbox</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">"Create initial social network of agents"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="str">"useActivation"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Checkbox</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"Use heterogenous activations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"similarityThreshold"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="str">"Similarity threshold"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="num">0.5</span><span class="op">,</span> <span class="num">0.0</span><span class="op">,</span> <span class="num">1.0</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose how similar two agents topics have to be, to send a letter."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"moveRange"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="str">"Range for moving position&lt;/br>(% of mean agent distances)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="num">0.1</span><span class="op">,</span> <span class="num">0.05</span><span class="op">,</span> <span class="num">0.75</span><span class="op">,</span> <span class="num">0.05</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose the visibility range for finding potential locations to move to."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"letterRange"</span><span class="op">:</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">Slider</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="str">"Range for letter sending&lt;/br>(% of mean agent distances)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="num">0.2</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span><span class="num">1.0</span><span class="op">,</span> <span class="num">0.1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="nam">description</span><span class="op">=</span><span class="str">"Choose the visibility range for finding potential recipients."</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="key">def</span> <span class="nam">topic_draw</span><span class="op">(</span><span class="nam">agent</span><span class="op">:</span><span class="nam">mg</span><span class="op">.</span><span class="nam">GeoAgent</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"""Define visualization strategies for agents.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    Region agents get the main color as a mean of</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    all region agents topic vectors.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">    Sender agetns have the color of their current</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">    topic vector.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="nam">portrayal</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">RegionAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">color</span> <span class="op">=</span> <span class="nam">colors</span><span class="op">.</span><span class="nam">to_hex</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">has_main_topic</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"color"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">color</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">colortuple</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"radius"</span><span class="op">]</span> <span class="op">=</span> <span class="num">5</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"shape"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"circle"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"color"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">colors</span><span class="op">.</span><span class="nam">to_hex</span><span class="op">(</span><span class="nam">colortuple</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"description"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">return</span> <span class="nam">portrayal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="nam">map_element</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">MapModule</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">portrayal_method</span><span class="op">=</span><span class="nam">topic_draw</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">view</span><span class="op">=</span><span class="op">[</span><span class="num">52</span><span class="op">,</span> <span class="num">12</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">zoom</span><span class="op">=</span><span class="num">4</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">map_width</span><span class="op">=</span><span class="num">700</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="nam">map_height</span><span class="op">=</span><span class="num">500</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="nam">chart</span> <span class="op">=</span> <span class="nam">ChartVisualization</span><span class="op">.</span><span class="nam">ChartModule</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="op">{</span><span class="str">"Label"</span><span class="op">:</span> <span class="str">"Movements"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"red"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="op">{</span><span class="str">"Label"</span><span class="op">:</span> <span class="str">"Clusters"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"black"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="op">{</span><span class="str">"Label"</span><span class="op">:</span> <span class="str">"Letters"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"green"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">data_collector_name</span><span class="op">=</span><span class="str">"datacollector"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="nam">server</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">ModularServer</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="nam">HistoricalLetters</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="op">[</span><span class="nam">map_element</span><span class="op">,</span> <span class="nam">chart</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="str">"Historical Letters"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="nam">model_params</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="key">def</span> <span class="nam">topic_draw</span><span class="op">(</span><span class="nam">agent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">portrayal</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">RegionAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="nam">color</span> <span class="op">=</span> <span class="nam">colors</span><span class="op">.</span><span class="nam">to_hex</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">has_main_topic</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="key">except</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">has_main_topic</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="key">raise</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"color"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">color</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">agent</span><span class="op">,</span> <span class="nam">SenderAgent</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">colortuple</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">topicVec</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"radius"</span><span class="op">]</span> <span class="op">=</span> <span class="num">5</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"shape"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"circle"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"color"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">colors</span><span class="op">.</span><span class="nam">to_hex</span><span class="op">(</span><span class="nam">colortuple</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">portrayal</span><span class="op">[</span><span class="str">"description"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">str</span><span class="op">(</span><span class="nam">agent</span><span class="op">.</span><span class="nam">unique_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">return</span> <span class="nam">portrayal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="nam">map_element</span> <span class="op">=</span> <span class="nam">mg</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">MapModule</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">portrayal_method</span><span class="op">=</span><span class="nam">topic_draw</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">view</span><span class="op">=</span><span class="op">[</span><span class="num">52</span><span class="op">,</span> <span class="num">12</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">zoom</span><span class="op">=</span><span class="num">4</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">map_width</span><span class="op">=</span><span class="num">700</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">map_height</span><span class="op">=</span><span class="num">500</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="nam">chart</span> <span class="op">=</span> <span class="nam">ChartVisualization</span><span class="op">.</span><span class="nam">ChartModule</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="op">{</span><span class="str">"Label"</span><span class="op">:</span> <span class="str">"Movements"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"red"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="op">{</span><span class="str">"Label"</span><span class="op">:</span> <span class="str">"Clusters"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"black"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="op">{</span><span class="str">'Label'</span><span class="op">:</span> <span class="str">"Letters"</span><span class="op">,</span> <span class="str">"Color"</span><span class="op">:</span> <span class="str">"green"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="nam">data_collector_name</span><span class="op">=</span><span class="str">'datacollector'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="nam">server</span> <span class="op">=</span> <span class="nam">mesa</span><span class="op">.</span><span class="nam">visualization</span><span class="op">.</span><span class="nam">ModularServer</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="nam">HistoricalLetters</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="op">[</span><span class="nam">map_element</span><span class="op">,</span> <span class="nam">chart</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="str">"Historical Letters"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">model_params</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_space_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_444d8314c29d6cbe_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_444d8314c29d6cbe_space_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,106 +1,102 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
-hhiissttoorriiccaalllleetttteerrss//sseerrvveerr..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//hhiissttoorriiccaalllleetttteerrss//sseerrvveerr..ppyy:: 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2222 ssttaatteemmeennttss ?  2222 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
-_1"""A visualization interface for HistoricalLetters using the older
-visualization option of mesa.""" 
-_2import mesa 
-_3import mesa_geo as mg 
-_4from matplotlib import colors 
+********** 2266 ssttaatteemmeennttss ?  00 rruunn 2266 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
+_1import matplotlib.colors as colors 
+_2 
+_3import mesa 
+_4import mesa_geo as mg 
 _5from mesa.visualization.modules import ChartVisualization 
 _6 
-_7from scicom.historicalletters.agents import RegionAgent, SenderAgent 
+_7from scicom.historicalletters.agents import SenderAgent, RegionAgent 
 _8from scicom.historicalletters.model import HistoricalLetters 
 _9 
 _1_0model_params = { 
-_1_1 "population": mesa.visualization.Slider( 
-_1_2 "Number of persons", 
-_1_3 50, 10, 100, 10, 
-_1_4 description="Choose how many senders to include in the model.", 
-_1_5 ), 
-_1_6 "useSocialNetwork": mesa.visualization.Checkbox( 
-_1_7 "Create initial social network of agents", 
-_1_8 False, 
-_1_9 ), 
-_2_0 "useActivation": mesa.visualization.Checkbox( 
-_2_1 "Use heterogenous activations", 
-_2_2 False, 
-_2_3 ), 
-_2_4 "similarityThreshold": mesa.visualization.Slider( 
-_2_5 "Similarity threshold", 
-_2_6 0.5, 0.0, 1.0, 0.1, 
-_2_7 description="Choose how similar two agents topics have to be, to send a
+_1_1 #"population": 100, 
+_1_2 "population": mesa.visualization.Slider( 
+_1_3 "Number of persons", 
+_1_4 50, 10, 100, 10, 
+_1_5 description="Choose how many senders to include in the model.", 
+_1_6 ), 
+_1_7 "useSocialNetwork": mesa.visualization.Checkbox( 
+_1_8 "Create initial social network of agents", 
+_1_9 False 
+_2_0 ), 
+_2_1 "useActivation": mesa.visualization.Checkbox( 
+_2_2 "Use heterogenous activations", 
+_2_3 False 
+_2_4 ), 
+_2_5 "similarityThreshold": mesa.visualization.Slider( 
+_2_6 "Similarity threshold", 
+_2_7 0.5, 0.0, 1.0, 0.1, 
+_2_8 description="Choose how similar two agents topics have to be, to send a
 letter.", 
-_2_8 ), 
-_2_9 "moveRange": mesa.visualization.Slider( 
-_3_0 "Range for moving position</br>(% of mean agent distances)", 
-_3_1 0.01, 0.00, 0.5, 0.05, 
-_3_2 description="Choose the visibility range for finding potential locations to
+_2_9 ), 
+_3_0 "moveRange": mesa.visualization.Slider( 
+_3_1 "Range for moving position</br>(% of mean agent distances)", 
+_3_2 0.1, 0.05, 0.75, 0.05, 
+_3_3 description="Choose the visibility range for finding potential locations to
 move to.", 
-_3_3 ), 
-_3_4 "letterRange": mesa.visualization.Slider( 
-_3_5 "Range for letter sending</br>(% of mean agent distances)", 
-_3_6 0.2, 0.1, 1.0, 0.1, 
-_3_7 description="Choose the visibility range for finding potential
+_3_4 ), 
+_3_5 "letterRange": mesa.visualization.Slider( 
+_3_6 "Range for letter sending</br>(% of mean agent distances)", 
+_3_7 0.2, 0.1,1.0, 0.1, 
+_3_8 description="Choose the visibility range for finding potential
 recipients.", 
-_3_8 ), 
-_3_9} 
-_4_0 
+_3_9 ), 
+_4_0} 
 _4_1 
-_4_2def topic_draw(agent:mg.GeoAgent) -> dict: 
-_4_3 """Define visualization strategies for agents. 
-_4_4 
-_4_5 Region agents get the main color as a mean of 
-_4_6 all region agents topic vectors. 
-_4_7 
-_4_8 Sender agetns have the color of their current 
-_4_9 topic vector. 
-_5_0 """ 
-_5_1 portrayal = {} 
-_5_2 if isinstance(agent, RegionAgent): 
-_5_3 color = colors.to_hex(agent.has_main_topic()) 
-_5_4 portrayal["color"] = color 
-_5_5 elif isinstance(agent, SenderAgent): 
-_5_6 colortuple = set(agent.topicVec) 
-_5_7 portrayal["radius"] = 5 
-_5_8 portrayal["shape"] = "circle" 
-_5_9 portrayal["color"] = colors.to_hex(colortuple) 
-_6_0 portrayal["description"] = str(agent.unique_id) 
-_6_1 return portrayal 
-_6_2 
-_6_3map_element = mg.visualization.MapModule( 
-_6_4 portrayal_method=topic_draw, 
-_6_5 view=[52, 12], 
-_6_6 zoom=4, 
-_6_7 map_width=700, 
-_6_8 map_height=500, 
-_6_9) 
-_7_0 
-_7_1chart = ChartVisualization.ChartModule( 
-_7_2 [ 
-_7_3 {"Label": "Movements", "Color": "red"}, 
-_7_4 {"Label": "Clusters", "Color": "black"}, 
-_7_5 {"Label": "Letters", "Color": "green"}, 
-_7_6 ], 
-_7_7 data_collector_name="datacollector", 
-_7_8) 
-_7_9 
-_8_0 
-_8_1server = mesa.visualization.ModularServer( 
-_8_2 HistoricalLetters, 
-_8_3 [map_element, chart], 
-_8_4 "Historical Letters", 
-_8_5 model_params, 
-_8_6) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
+_4_2 
+_4_3def topic_draw(agent): 
+_4_4 portrayal = {} 
+_4_5 if isinstance(agent, RegionAgent): 
+_4_6 try: 
+_4_7 color = colors.to_hex(agent.has_main_topic()) 
+_4_8 except: 
+_4_9 print(agent.has_main_topic()) 
+_5_0 raise 
+_5_1 portrayal["color"] = color 
+_5_2 elif isinstance(agent, SenderAgent): 
+_5_3 colortuple = set(agent.topicVec) 
+_5_4 portrayal["radius"] = 5 
+_5_5 portrayal["shape"] = "circle" 
+_5_6 portrayal["color"] = colors.to_hex(colortuple) 
+_5_7 portrayal["description"] = str(agent.unique_id) 
+_5_8 return portrayal 
+_5_9 
+_6_0 
+_6_1map_element = mg.visualization.MapModule( 
+_6_2 portrayal_method=topic_draw, 
+_6_3 view=[52, 12], 
+_6_4 zoom=4, 
+_6_5 map_width=700, 
+_6_6 map_height=500, 
+_6_7) 
+_6_8 
+_6_9chart = ChartVisualization.ChartModule( 
+_7_0 [ 
+_7_1 {"Label": "Movements", "Color": "red"}, 
+_7_2 {"Label": "Clusters", "Color": "black"}, 
+_7_3 {'Label': "Letters", "Color": "green"} 
+_7_4 ], 
+_7_5 data_collector_name='datacollector', 
+_7_6) 
+_7_7 
+_7_8 
+_7_9server = mesa.visualization.ModularServer( 
+_8_0 HistoricalLetters, 
+_8_1 [map_element, chart], 
+_8_2 "Historical Letters", 
+_8_3 model_params, 
+_8_4) 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_space_py.html` & `scicom-0.4.0/tests/reports/html/d_277402163e1a7589_space_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/space.py: 100%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/historicalletters/space.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/space.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/space.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">27 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">27<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-19 14:30 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""The geographical space for HistoricalLetters."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">mesa</span>&nbsp;</span><span class="r"></span></p>
@@ -139,18 +139,18 @@
     <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="str">"""Remove sender."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">remove_agent</span><span class="op">(</span><span class="nam">agent</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">remove_sender_from_region</span><span class="op">(</span><span class="nam">agent</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_277402163e1a7589_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 14:26 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-19 14:30 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 hhiissttoorriiccaalllleetttteerrss//ssppaaccee..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2277 ssttaatteemmeennttss ?  2277 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+19 14:30 +0200
 _1"""The geographical space for HistoricalLetters.""" 
 _2 
 _3import mesa 
 _4import mesa_geo as mg 
 _5 
 _6from scicom.historicalletters.agents import RegionAgent, SenderAgent 
 _7 
@@ -68,9 +68,9 @@
 _5_3 agent.geometry = pos 
 _5_4 self.add_sender(agent, regionID) 
 _5_5 
 _5_6 def __remove_sender(self, agent: SenderAgent) -> None: 
 _5_7 """Remove sender.""" 
 _5_8 super().remove_agent(agent) 
 _5_9 self.remove_sender_from_region(agent) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 14:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+19 14:30 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_a9eaaac38d807e21_utils_py.html` & `scicom-0.4.0/tests/reports/html/d_277402163e1a7589_utils_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/historicalletters/utils.py: 100%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/historicalletters/utils.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/historicalletters/utils.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/historicalletters/utils.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">39 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">39<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_space_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_space_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_8a655f2681f565c9_interface_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 15:05 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 12:29 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Utility functions for HistoricalLetters."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">random</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -194,18 +194,18 @@
     <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="nam">p2</span> <span class="op">=</span> <span class="nam">np</span><span class="op">.</span><span class="nam">array</span><span class="op">(</span><span class="nam">target</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="nam">p3</span> <span class="op">=</span> <span class="nam">p1</span> <span class="op">+</span> <span class="nam">random</span><span class="op">.</span><span class="nam">uniform</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="op">(</span><span class="nam">p2</span> <span class="op">-</span><span class="nam">p1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">p3</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_space_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_space_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_8a655f2681f565c9_interface_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 15:05 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-15 12:29 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//
 hhiissttoorriiccaalllleetttteerrss//uuttiillss..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3399 ssttaatteemmeennttss ?  3399 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 15:05 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 12:29 +0200
 _1"""Utility functions for HistoricalLetters.""" 
 _2import random 
 _3 
 _4import geopandas as gpd 
 _5import mesa 
 _6import numpy as np 
 _7import pandas as pd 
@@ -127,9 +127,9 @@
 _1_0_8 
 _1_0_9 The amount of moving from start to target is random. 
 _1_1_0 """ 
 _1_1_1 p1 = np.array(start) 
 _1_1_2 p2 = np.array(target) 
 _1_1_3 p3 = p1 + random.uniform(0, 1) * (p2 -p1) 
 _1_1_4 return tuple(p3) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 15:05 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+15 12:29 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3___init___py.html` & `scicom-0.4.0/tests/reports/coverage-html/d_444d8314c29d6cbe___init___py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/__init__.py: 100%</title>
+    <title>Coverage for src/scicom/historicalletters/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/__init__.py</b>:
+            <span class="text">Coverage for </span><b>src/scicom/historicalletters/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,42 +56,42 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_02d42bec932dca30___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_a9eaaac38d807e21___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_444d8314c29d6cbe_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_a9eaaac38d807e21___init___py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_02d42bec932dca30___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_444d8314c29d6cbe_agents_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-15 13:26 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//____iinniitt____..ppyy::
-110000%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//sscciiccoomm//hhiissttoorriiccaalllleetttteerrss//____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+15 13:26 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3_interface_py.html` & `scicom-0.4.0/tests/reports/html/d_8a655f2681f565c9_interface_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/interface.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/interface.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/interface.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/interface.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">15 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">15<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_SimpleContinuousModule_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Solara interface for all simulations."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -117,18 +117,18 @@
     <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">label</span><span class="op">=</span><span class="str">"Knowledge Spread"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a9eaaac38d807e21_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_124ad581c8e87a79_SimpleContinuousModule_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_277402163e1a7589_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_2e9db29e074df228_SimpleContinuousModule_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-26 13:41 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-05-14 11:31 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//iinntteerrffaaccee..ppyy::
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//iinntteerrffaaccee..ppyy::
 00%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1155 ssttaatteemmeennttss ?  00 rruunn 1155 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
 _1"""Solara interface for all simulations.""" 
 _2from pathlib import Path 
 _3 
 _4import solara 
 _5 
 _6from scicom.historicalletters.interface import page as
 historical_letters_page 
@@ -48,9 +48,9 @@
 _3_1 ), 
 _3_2 solara.Route( 
 _3_3 path="knowledgespread", 
 _3_4 component=knowledgespread, 
 _3_5 label="Knowledge Spread", 
 _3_6 ), 
 _3_7] 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-26 13:41 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-05-
+14 11:31 +0200
```

### Comparing `scicom-0.3.1/tests/reports/html/z_e85bc3a05b58e6d3_run_py.html` & `scicom-0.4.0/tests/reports/html/d_8a655f2681f565c9_run_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for .tox/p311/lib/python3.10/site-packages/scicom/run.py: 0%</title>
+    <title>Coverage for .tox/p311/lib/python3.11/site-packages/scicom/run.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.10/site-packages/scicom/run.py</b>:
+            <span class="text">Coverage for </span><b>.tox/p311/lib/python3.11/site-packages/scicom/run.py</b>:
             <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,30 +56,30 @@
         <h2>
             <span class="text">10 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">10<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_124ad581c8e87a79_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_22d2582a602e487e___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_3142edd200b00bad___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 14:46 +0200
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Run simulations."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -104,18 +104,18 @@
     <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">elif</span> <span class="nam">args</span><span class="op">.</span><span class="nam">simulation</span> <span class="op">==</span> <span class="str">"knowledgespread"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">from</span> <span class="nam">scicom</span><span class="op">.</span><span class="nam">knowledgespread</span><span class="op">.</span><span class="nam">server</span> <span class="key">import</span> <span class="nam">server</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">server</span><span class="op">.</span><span class="nam">launch</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_124ad581c8e87a79_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_22d2582a602e487e___init___py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_2e9db29e074df228_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_3142edd200b00bad___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-25 12:40 +0200
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-17 14:46 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1100//ssiittee--ppaacckkaaggeess//sscciiccoomm//rruunn..ppyy:: 00%%
+************ CCoovveerraaggee ffoorr ..ttooxx//pp331111//lliibb//ppyytthhoonn33..1111//ssiittee--ppaacckkaaggeess//sscciiccoomm//rruunn..ppyy:: 00%%
 ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1100 ssttaatteemmeennttss ?  00 rruunn 1100 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 14:46 +0200
 _1"""Run simulations.""" 
 _2import argparse 
 _3 
 _4parser = argparse.ArgumentParser( 
 _5 prog="Run SciCom Simulations", 
 _6 description="This script starts the server interfaces for the different
 ABM.", 
@@ -34,9 +34,9 @@
 _1_8 
 _1_9if args.simulation == "historicalletters": 
 _2_0 from scicom.historicalletters.server import server 
 _2_1 server.launch() 
 _2_2elif args.simulation == "knowledgespread": 
 _2_3 from scicom.knowledgespread.server import server 
 _2_4 server.launch() 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-25 12:40 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+17 14:46 +0200
```

### Comparing `scicom-0.3.1/tests/scicom/historicalletters/test_model.py` & `scicom-0.4.0/tests/scicom/historicalletters/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,28 +57,14 @@
     )
     # 30 agents should be on the scheduler
     c1 = 30
     assert len(model.schedule.agents) == c1
     model.run(5)
 
 
-def test_model_initialization_with_pruning() -> None:
-    """Model initialization puts agents on sheduler."""
-    # initialize model for 30 agents with defaults
-    model = HistoricalLetters(
-        population=30,
-        runPruning=True,
-        debug=True,
-    )
-    # 30 agents should be on the scheduler
-    c1 = 30
-    assert len(model.schedule.agents) == c1
-    model.run(5)
-
-
 def test_model_smallworldiness() -> None:
     """Test if parameter changes increase smallworldiness."""
     model1 = HistoricalLetters(
         population=30,
         useSocialNetwork=True,
         longRangeNetworkFactor=0.3,
         shortRangeNetworkFactor=0.4,
```

### Comparing `scicom-0.3.1/tests/scicom/historicalletters/test_server.py` & `scicom-0.4.0/tests/scicom/historicalletters/test_server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/scicom/historicalletters/test_space.py` & `scicom-0.4.0/tests/scicom/historicalletters/test_space.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/tests/scicom/historicalletters/test_utils.py` & `scicom-0.4.0/tests/scicom/historicalletters/test_utils.py`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/LICENSE.md` & `scicom-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/README.md` & `scicom-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scicom-0.3.1/pyproject.toml` & `scicom-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SciCom"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Bernardo S. Buarque", email="bernardo.buarque@motu.org.nz"},
   { name="Malte Vogl", email="vogl@gea.mpg.de"}
 ]
 description = "Simulating various aspects of scientific communication via Agent-based models."
 readme = "README.md"
 license = {file = "LICENSE.md"}
```

### Comparing `scicom-0.3.1/PKG-INFO` & `scicom-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: SciCom
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simulating various aspects of scientific communication via Agent-based models.
 Project-URL: Project Homepage, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Homepage, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 Project-URL: Issues, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels/-/issues
 Author-email: "Bernardo S. Buarque" <bernardo.buarque@motu.org.nz>, Malte Vogl <vogl@gea.mpg.de>
 License: MIT License
```

