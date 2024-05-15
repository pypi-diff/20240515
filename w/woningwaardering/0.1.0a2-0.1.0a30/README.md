# Comparing `tmp/woningwaardering-0.1.0a2.tar.gz` & `tmp/woningwaardering-0.1.0a30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woningwaardering-0.1.0a2.tar", last modified: Mon May 13 19:26:01 2024, max compression
+gzip compressed data, was "woningwaardering-0.1.0a30.tar", last modified: Wed May 15 20:19:46 2024, max compression
```

## Comparing `woningwaardering-0.1.0a2.tar` & `woningwaardering-0.1.0a30.tar`

### file list

```diff
@@ -1,16 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:26:01.711197 woningwaardering-0.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 19:25:57.000000 woningwaardering-0.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-05-13 19:26:01.711197 woningwaardering-0.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22339 2024-05-13 19:25:57.000000 woningwaardering-0.1.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 19:25:57.000000 woningwaardering-0.1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:26:01.711197 woningwaardering-0.1.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:26:01.707198 woningwaardering-0.1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-13 19:25:57.000000 woningwaardering-0.1.0a2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:26:01.711197 woningwaardering-0.1.0a2/woningwaardering/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-13 19:25:57.000000 woningwaardering-0.1.0a2/woningwaardering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:26:01.711197 woningwaardering-0.1.0a2/woningwaardering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-05-13 19:26:01.000000 woningwaardering-0.1.0a2/woningwaardering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 19:26:01.000000 woningwaardering-0.1.0a2/woningwaardering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:26:01.000000 woningwaardering-0.1.0a2/woningwaardering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 19:26:01.000000 woningwaardering-0.1.0a2/woningwaardering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 19:26:01.000000 woningwaardering-0.1.0a2/woningwaardering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.322944 woningwaardering-0.1.0a30/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24037 2024-05-15 20:19:46.322944 woningwaardering-0.1.0a30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22339 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/docs/afbeeldingen/
+-rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/docs/afbeeldingen/excel_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/docs/afbeeldingen/oppervlakte_van_vertrekken.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/docs/implementatietoelichting-beleidsboeken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/docs/implementatietoelichting-beleidsboeken/2024/
+-rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/scripts/genereer_opzet_woningwaarderinggroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/scripts/genereer_test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/scripts/genereer_vera_referentiedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/scripts/uitbreiden_vera_modellen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:19:46.322944 woningwaardering-0.1.0a30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/taskfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.262944 woningwaardering-0.1.0a30/tests/data/input/generiek/
+-rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/generiek/37101000032.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.266944 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/12006000004.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/23003000050.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/25048000007.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/28018000044.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41027000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41162000015.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/51011000042.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/71211000027.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/81020000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/81065000089.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/85651000021.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/87402000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/input/zelfstandige_woonruimten/87402000003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/config/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/test_ZelfstandigeWoonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/utils/test_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/utils/test_is_geldig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/utils/test_vind_yaml_bestanden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.270944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.254944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.274944 woningwaardering-0.1.0a30/wettelijke-documenten/
+-rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/stelsels/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/stelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/stelselgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.278944 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.258944 woningwaardering-0.1.0a30/woningwaardering/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.258944 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/vera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136654 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.282944 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/model_uitbreidingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/aanbiedingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/adressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/afletterstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/afspraakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/afwezigheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/aktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/bedrijfsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/begrotingversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/bestemming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/betaalgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/betaalwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekingdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/boekjaarstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/brandwerendheidscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/btw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/btwaangiftestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/burgerlijkestaat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/clustersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/communicatiekanaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/communicatierichting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/conditiescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/contactgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/contactgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/crediteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/crediteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/dagdeel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/debiteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/debiteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/defectlocatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/defectoorzaak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/defectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/defectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/doelgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/dossier/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/dossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidinterieur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidisolatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidmonument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidsanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eenheidstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eindedetailreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/eindereden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energie/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energielabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energieprestatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energieprestatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/externeincassosoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/externeincassostatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/factuursoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/financien/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/financien/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/gebeurtenissoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/geometriesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/geslacht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/huurgeschilsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/huurgeschilstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/huurklasse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/incassomoment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/informatieobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inkomensbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inkomenssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inspectierapportsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/inspectierapportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/kandidaatstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/kwaliteit/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/leningaflosvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/leningdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/leningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/maatschappelijklabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/machtigingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/materiaalsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/medewerkerrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/medewerkersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/meeteenheid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoud/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/opleidingsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/oppervlaktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/opzegtermijn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/organisatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/organisatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/organisatievorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomsten/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomstsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/overeenkomststatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/passendheidssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prestatieafspraak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prijscomponentsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectontwikkeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/projectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/provincie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/publicatieintakevorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/publicatiemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/publicatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/reclamatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/reclamatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/redenontbinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/redenopzegging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/redenvernietiging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/regiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relatieadressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relatiedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relatierolsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relaties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relaties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/relatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/rentesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/ruimteligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/ruimtesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/sanctiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/sanctiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/signaleringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/signaleringstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/taal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/uitexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/uitvoerendesoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/vastgoed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/vastgoed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/verantwoordingregime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/verrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/voorrangsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.318944 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woonruimteverdeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woonsituatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/woonvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zaakobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zaakrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zaakstatussoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zaaktypesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/referentiedata_uitbreiding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 20:19:41.000000 woningwaardering-0.1.0a30/woningwaardering/vera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:19:46.322944 woningwaardering-0.1.0a30/woningwaardering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24037 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 20:19:46.000000 woningwaardering-0.1.0a30/woningwaardering.egg-info/top_level.txt
```

### Comparing `woningwaardering-0.1.0a2/LICENSE` & `woningwaardering-0.1.0a30/LICENSE`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a2/PKG-INFO` & `woningwaardering-0.1.0a30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.1.0a2
+Version: 0.1.0a30
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `woningwaardering-0.1.0a2/README.md` & `woningwaardering-0.1.0a30/README.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a2/pyproject.toml` & `woningwaardering-0.1.0a30/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "woningwaardering"
-version = "0.1.0-a.2"
+dynamic = ["version"]
 description = "Berekent de punten van een woning op basis van het woningwaarderingsstelsel."
 authors = [
     { name = "Ben Verhees", email = "ben.verhees@woonstadrotterdam.nl" },
     { name = "Tiddo Loos", email = "tiddo.loos@woonstadrotterdam.nl" },
     { name = "Tomer Gabay", email = "tomer.gabay@woonstadrotterdam.nl" }
 ]
 keywords = ["woning", "waardering", "stelsel", "woningwaarderingsstelsel", "wws"]
@@ -30,15 +30,18 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/WoonstadRotterdamTemp/woningwaardering"
 Issues = "https://github.com/WoonstadRotterdamTemp/woningwaardering/issues"
 
 [tool.setuptools.packages.find]
-include = ["woningwaardering"]
+include = ["woningwaardering*"]
+
+[tool.setuptools_scm]
+version_file = "woningwaardering/_version.py"
 
 [project.optional-dependencies]
 test = [
     "pre-commit==3.3.*",
     "ruff==0.3.*",
     "pytest==8.0.*",
     "types-requests==2.*",
```

### Comparing `woningwaardering-0.1.0a2/tests/test_utils.py` & `woningwaardering-0.1.0a30/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a2/woningwaardering/__init__.py` & `woningwaardering-0.1.0a30/woningwaardering/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a2/woningwaardering.egg-info/PKG-INFO` & `woningwaardering-0.1.0a30/woningwaardering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.1.0a2
+Version: 0.1.0a30
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

