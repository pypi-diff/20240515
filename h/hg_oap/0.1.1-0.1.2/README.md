# Comparing `tmp/hg_oap-0.1.1.tar.gz` & `tmp/hg_oap-0.1.2.tar.gz`

## Comparing `hg_oap-0.1.1.tar` & `hg_oap-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,75 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.coveragerc
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hg_oap-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/workflows/deploy-on-tag.yml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/asset.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/commodities.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/currency.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/__init__.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/calendar.py
--rw-r--r--   0        0        0    23590 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/dgen.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/tenor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/cash.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/commodity.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/forward.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/future.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/fx.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/instrument.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/physical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/__init__.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order.py
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order_service.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/portfolio/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/position/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/position/position.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/pricing/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/pricing/price.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/quanity/__init__.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/U.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/__init__.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/dimension.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/quantity.py
--rw-r--r--   0        0        0    13230 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/unit.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/unit_system.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/exprclass.py
--rw-r--r--   0        0        0    25216 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/op.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/op_delarations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/example/__init__.py
--rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/example/test_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/orders/__init__.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/orders/test_order_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/quantity/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_calendar.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dataclassex.py
--rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dgen.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dimension.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_magic.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity_ts.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hg_oap-0.1.1/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hg_oap-0.1.1/README.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hg_oap-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hg_oap-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hg_oap-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.github/workflows/deploy-on-tag.yml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/hg_oap.iml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    31435 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/assets/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/assets/asset.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/assets/commodities.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/assets/currency.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/dates/__init__.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/dates/calendar.py
+-rw-r--r--   0        0        0    29215 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/dates/dgen.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/dates/tenor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/cash.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/commodity.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/forward.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/future.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/fx.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/instrument.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/instruments/physical.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/orders/__init__.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/orders/order.py
+-rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/orders/order_service.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/orders/order_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/portfolio/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/position/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/position/position.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/pricing/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/pricing/price.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/quanity/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/default_unit_system.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/dimension.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/quantity.py
+-rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/unit.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/units/unit_system.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/utils/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/utils/exprclass.py
+-rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/utils/op.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hg_oap-0.1.2/src/hg_oap/utils/op_declarations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/example/__init__.py
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/example/test_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/orders/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/orders/test_order_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/quantity/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_calendar.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dataclassex.py
+-rw-r--r--   0        0        0     9575 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dgen.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dimension.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_magic.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_quantity.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_quantity_ts.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hg_oap-0.1.2/tests/unit/hg_oap/utils/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hg_oap-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hg_oap-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hg_oap-0.1.2/README.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hg_oap-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hg_oap-0.1.2/PKG-INFO
```

### Comparing `hg_oap-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `hg_oap-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `hg_oap-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/.github/workflows/deploy-on-tag.yml` & `hg_oap-0.1.2/.github/workflows/deploy-on-tag.yml`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/assets/asset.py` & `hg_oap-0.1.2/src/hg_oap/assets/asset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from decimal import Decimal
 
 from hg_oap.units import Quantity
 from hg_oap.units.unit import Unit
 from hg_oap.units.unit_system import UnitConversionContext
 from hg_oap.utils.exprclass import ExprClass
 from hgraph import CompoundScalar
 
@@ -21,16 +20,17 @@
 @dataclass(frozen=True)
 class PhysicalAsset(Asset):
     """
     A tangible thing, for example: raw materials, infrastructure, equipment, etc.
     """
     name: str
     unit: Unit  # The basic unit used to measure the asset
-    unit_conversion_factors: tuple[Quantity[Decimal]]  # Properties of the asset that can be used to convert between
-                                                       # units of different dimensions - i.e. density for mass/volume
+    unit_conversion_factors: tuple[Quantity[float]] = ()  # Properties of the asset that can be used to convert
+                                                            # between units of different dimensions - i.e. density
+                                                            # for mass/volume
 
 
 @dataclass(frozen=True)
 class FinancialAsset(Asset):
     """
     A financial asset is a thing of value that can be held. Examples include cash, cash equivalents, stocks
     and bonds. They are not instruments, but can be used in an instrument as an underlyer.
```

### Comparing `hg_oap-0.1.1/src/hg_oap/assets/commodities.py` & `hg_oap-0.1.2/src/hg_oap/assets/commodities.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/assets/currency.py` & `hg_oap-0.1.2/src/hg_oap/assets/currency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from decimal import Decimal
 from enum import Enum
 from typing import Optional
 
 from hg_oap.assets.asset import FinancialAsset
 from hg_oap.units import PrimaryUnit
 
 
@@ -12,20 +11,20 @@
     """
     The medium of exchange for goods and services, you may have used this. For example USD, EUR, GBP, etc.
     These represent the most commonly used currencies in the USA, Europe or the United Kingdom.
     """
     minor_currency_ratio: Optional[int] = None  # For example US cents rather than dollars
 
     def __post_init__(self):
-        from hg_oap.units import U
+        from hg_oap.units.default_unit_system import U
         setattr(U, f"currency.{self.symbol}", currency_dim := getattr(U.money, self.symbol))  # Add the currency to the unit system as a qualified dimansion
         setattr(U, self.symbol, unit := PrimaryUnit(dimension=currency_dim))
         if self.minor_currency_ratio is not None:
             minor_symbol = f"{self.symbol[:-1]}X"
-            setattr(U, minor_symbol, Decimal(1)/Decimal(self.minor_currency_ratio) * unit)
+            setattr(U, minor_symbol, 1.0/self.minor_currency_ratio * unit)
 
 
 @dataclass(frozen=True)
 class MinorCurrency(Currency):
     """
     A minor currency is the fractional unit, for example US cents, typically this is a 1:100 ratio, the ratio
     is stored as ratio.
```

### Comparing `hg_oap-0.1.1/src/hg_oap/dates/calendar.py` & `hg_oap-0.1.2/src/hg_oap/dates/calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 from bisect import bisect, bisect_left
 from datetime import date, timedelta
 from typing import Tuple, Set
 
-__all__ = ('Calendar',)
+__all__ = ('Calendar', 'WeekendCalendar', 'HolidayCalendar')
 
 
 class Calendar:
     @abstractmethod
     def weekend_days(self) -> Tuple[int, ...]: ...
 
     @abstractmethod
```

### Comparing `hg_oap-0.1.1/src/hg_oap/dates/dgen.py` & `hg_oap-0.1.2/src/hg_oap/dates/dgen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import date, timedelta
 from itertools import islice
 from typing import cast
 
 from hg_oap.dates.calendar import Calendar
-from hg_oap.utils.op import Item, Op, lazy
+from hg_oap.utils.op import Item, Op, lazy, is_op
 from hg_oap.dates.tenor import Tenor
 
 __all__ = ('is_dgen', 'make_date', 'make_dgen', 'years', 'months', 'weeks', 'weekdays', 'weekends', 'days',
-           'business_days', 'roll_fwd', 'roll_bwd')
+           'business_days', 'roll_fwd', 'roll_bwd', 'DGen', 'retain', 'DGenParameter')
 
 
 def is_dgen(obj):
     return isinstance(obj, DGen)
 
 
 def make_date(obj):
@@ -41,82 +41,108 @@
     return item.start is not None and item.start < 0 \
         or item.stop is not None and item.stop < 0 \
         or item.step is not None and item.step < 0
 
 
 class DGen(Item):
     def __call__(self, input_date=None, start: date = date.min, end: date = date.max, after: date = date.min,
-                 before: date = date.max, calendar: Calendar = None):
-        return self.__invoke__(make_date(start), make_date(end), make_date(after), make_date(before), calendar)
+                 before: date = date.max, calendar: Calendar = None, **kwargs):
+        return self.__invoke__(make_date(start), make_date(end), make_date(after), make_date(before), calendar, **kwargs)
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         raise StopIteration
 
     def is_single_date_gen(self):
         return False
 
     def cadence(self):
         return None
 
     def __iter__(self):
         return self
 
     def __or__(self, other):
-        return JoinDGen(self, make_dgen(other))
+        if is_op(other):
+            return lazy(self) | other
+        else:
+            return JoinDGen(self, make_dgen(other))
 
     def __ror__(self, other):
-        return JoinDGen(make_dgen(other), self)
+        if is_op(other):
+            return other | lazy(self)
+        else:
+            return JoinDGen(make_dgen(other), self)
 
     def __and__(self, other):
-        return CommonDatesDGen(self, make_dgen(other))
+        if is_op(other):
+            return lazy(self) & other
+        else:
+            return CommonDatesDGen(self, make_dgen(other))
 
     def __rand__(self, other):
-        return CommonDatesDGen(make_dgen(other), self)
+        if is_op(other):
+            return other & lazy(self)
+        else:
+            return CommonDatesDGen(make_dgen(other), self)
 
     def __gt__(self, other):
-        if not is_dgen(other):
+        if is_op(other):
+            return lazy(self) > other
+        elif not is_dgen(other):
             return AfterDGen(self, make_date(other))
         elif other.is_single_date_gen():
             return AfterDGen(self, other)
         else:
             raise ValueError('Comparing two date generators is not supported')
 
     def __lt__(self, other):
+        if is_op(other):
+            return lazy(self) < other
         if is_dgen(other) and self.is_single_date_gen():
             return other.__ge__(self)
         else:
             if lhs := getattr(self, '__compared__', None):
                 return BeforeDGen(lhs, make_date(other))
             if self.__expression__ is not None:
                 return self.__expression__ < other
             return BeforeDGen(self, make_date(other))
 
     def __ge__(self, other):
+        if is_op(other):
+            return lazy(self) >= other
         if not is_dgen(other):
             return AfterOrOnDGen(self, make_date(other))
         elif other.is_single_date_gen():
             return AfterOrOnDGen(self, other)
         else:
             raise ValueError('Comparing two dage generators is not supported')
 
     def __le__(self, other):
+        if is_op(other):
+            return lazy(self) <= other
         if is_dgen(other) and self.is_single_date_gen():
             return other.__gt__(self)
         else:
             if lhs := getattr(self, '__compared__', None):
                 return BeforeOrOnDGen(lhs, make_date(other))
             if self.__expression__ is not None:
                 return self.__expression__ <= other
             return BeforeOrOnDGen(self, make_date(other))
 
     def __add__(self, other):
-        return AddTenorDGen(self, Tenor(other))
+        if is_op(other):
+            return lazy(self) + other
+        else:
+            return AddTenorDGen(self, Tenor(other))
 
     def __sub__(self, other):
+        if is_op(other):
+            return lazy(self) - other
+
         try:
             tenor = Tenor(other)
             return SubTenorDGen(self, tenor)
         except:
             pass
 
         try:
@@ -124,315 +150,376 @@
             return RemoveDatesDGen(self, gen)
         except:
             pass
 
         raise ValueError(f'{other} is not a tenor or date generator')
 
     def __rsub__(self, other):
-        gen = make_dgen(other)
-        return RemoveDatesDGen(gen, self)
+        if is_op(other):
+            return other - lazy(self)
+        else:
+            gen = make_dgen(other)
+            return RemoveDatesDGen(gen, self)
 
     def __getitem__(self, item):
         if isinstance(item, int):
             if item >= 0:
                 return SliceDGen(self, slice(item, item + 1))
             else:
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
-        if isinstance(item, slice):
+        elif isinstance(item, slice):
             if is_negative_slice(item):
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
             return SliceDGen(self, item)
-        if isinstance(item, Op):
+        elif is_op(item):
             return lazy(self)[item]
 
     def over(self, calendar: Calendar):
-        return WithCalendarDGen(self, calendar)
+        if is_op(calendar):
+            return lazy(self).over(calendar)
+        else:
+            return WithCalendarDGen(self, calendar)
 
 
 class ConstDGen(DGen):
     def __init__(self, date):
         self.date = date
 
     def is_single_date_gen(self):
         return True
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         yield self.date
 
+    def __repr__(self):
+        return f"'{self.date}'"
+
 
 class SequenceDGen(DGen):
     def __init__(self, dates):
         self.dates = dates
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         yield from self.dates
 
+    def __repr__(self):
+        dates = ','.join(f"'{d}'" for d in self.dates)
+        return f"[{dates}]"
+
 
 class AfterDGen(DGen):
     def __init__(self, gen, date):
         self.gen = gen
         self.date = date
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         if is_dgen(self.date):
-            after = self.date(start, end, after, before, calendar)
+            after = next(self.date.__invoke__(start, end, after, before, calendar, **kwargs))
         else:
             after = self.date
 
         after = after + timedelta(days=1)
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d >= after)
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs) if d >= after)
 
     def __bool__(self):
         if is_dgen(self.date):
             self.date.__compared__ = self
         self.gen.__compared__ = self
         return True
 
+    def __repr__(self):
+        return f"{self.date} < '{self.gen}'"
+
 
 class AfterOrOnDGen(DGen):
     def __init__(self, gen, date):
         self.gen = gen
         self.date = date
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         if is_dgen(self.date):
-            after = self.date(start, end, after, before, calendar)
+            after = next(self.date.__invoke__(start, end, after, before, calendar, **kwargs))
         else:
             after = self.date
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d >= after)
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs) if d >= after)
 
     def __bool__(self):
         if is_dgen(self.date):
             self.date.__compared__ = self
         self.gen.__compared__ = self
         return True
 
+    def __repr__(self):
+        return f"{self.date} <= '{self.gen}'"
+
 
 class BeforeDGen(DGen):
     def __init__(self, gen, date):
         self.gen = gen
         self.date = date
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         if is_dgen(self.date):
-            before = self.date(start, end, after, before, calendar)
+            before = next(self.date.__invoke__(start, end, after, before, calendar, **kwargs))
         else:
             before = self.date
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d < before)
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs) if d < before)
+
+    def __repr__(self):
+        return f"'{self.gen}' < {self.date}"
 
 
 class BeforeOrOnDGen(DGen):
     def __init__(self, gen, date):
         self.gen = gen
         self.date = date
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         if is_dgen(self.date):
-            before = self.date(start, end, after, before, calendar)
+            before = next(self.date.__invoke__(start, end, after, before, calendar, **kwargs))
         else:
             before = self.date
 
         before = before + timedelta(days=1)
 
-        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar) if d < before)
+        yield from (d for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs) if d < before)
+
+    def __repr__(self):
+        return f"'{self.gen}' <= {self.date}"
 
 
 class EveryDayDGen(DGen):
     def cadence(self):
         return Tenor('1d')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         start = start if start is not date.min else after
         end = end if end is not date.max else before
 
         while start <= end:
             yield start
             start += timedelta(days=1)
 
+    def __repr__(self):
+        return 'days'
+
 
 days = EveryDayDGen()
 
 
 class WeekdaysDGen(DGen):
     def __init__(self, gen):
         self.gen = gen
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         we = calendar.weekend_days() if calendar else (5, 6)
         yield from (d for d in
-                    self.gen.__invoke__(start, end, after, before, calendar)
+                    self.gen.__invoke__(start, end, after, before, calendar, **kwargs)
                     if d.weekday() not in we)
 
+    def __repr__(self):
+        return 'weekdays'
+
 
 weekdays = WeekdaysDGen(days)
 
 
 class WeekendsDGen(DGen):
     def __init__(self, gen):
         self.gen = gen
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         we = calendar.weekend_days() if calendar else (5, 6)
         yield from (d for d in
-                    self.gen.__invoke__(start, end, after, before, calendar)
+                    self.gen.__invoke__(start, end, after, before, calendar, **kwargs)
                     if d.weekday() in we)
 
+    def __repr__(self):
+        return 'weekends'
+
 
 weekends = WeekendsDGen(EveryDayDGen())
 
 
 class BusinessDaysDGen(DGen):
     def __init__(self, gen):
         self.gen = gen
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         assert calendar, 'Business days calculation requires a calendar'
         yield from (d for d in
-                    self.gen.__invoke__(start, end, after, before, calendar)
+                    self.gen.__invoke__(start, end, after, before, calendar, **kwargs)
                     if not calendar.is_holiday_or_weekend(d))
 
+    def __repr__(self):
+        return 'business_days'
+
 
 business_days = BusinessDaysDGen(EveryDayDGen())
 
 
 class WeeksDGen(DGen):
     def cadence(self):
         return Tenor('1w')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         start = start if start is not date.min else after
         end = end if end is not date.max else before
 
         monday = start + timedelta(days=7 - start.weekday()) if start.weekday() > 0 else start
         while monday <= end:
             yield monday
             monday += timedelta(days=7)
 
     @property
     def mon(self):
-        return self
+        return DayOfWeekDGen(0, self)
 
     @property
     def tue(self):
-        return self + '1d'
+        return DayOfWeekDGen(1, self)
 
     @property
     def wed(self):
-        return self + '2d'
+        return DayOfWeekDGen(2, self)
 
     @property
     def thu(self):
-        return self + '3d'
+        return DayOfWeekDGen(3, self)
 
     @property
     def fri(self):
-        return self + '4d'
+        return DayOfWeekDGen(4, self)
 
     @property
     def sat(self):
-        return self + '5d'
+        return DayOfWeekDGen(5, self)
 
     @property
     def sun(self):
-        return self + '6d'
+        return DayOfWeekDGen(6, self)
+
+    def __repr__(self):
+        return 'weeks'
 
 
 weeks = WeeksDGen()
 
 
 class DayOfWeekDGen(DGen):
-    def __init__(self, weekday):
+    def __init__(self, weekday, gen=None):
+        self.gen = gen
         self.weekday = weekday
 
     def cadence(self):
         return Tenor('1w')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        d = after + timedelta(days=(self.weekday - after.weekday()) % 7)
-        while d < before:
-            yield d
-            d += timedelta(days=7)
+                   calendar: Calendar = None, **kwargs):
+        if self.gen is None:
+            d = after + timedelta(days=(self.weekday - after.weekday()) % 7)
+            while d < before:
+                yield d
+                d += timedelta(days=7)
+        else:
+            after -= timedelta(days=6)
+            for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs):
+                d_ = d + timedelta(days=(self.weekday - d.weekday()) % 7)
+                if d_ < before:
+                    yield d_
+
+    def __repr__(self):
+        weekday_name = ('mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun')[self.weekday]
+        if self.gen is not None:
+            return f'{self.gen}.{weekday_name}'
+        else:
+            return weekday_name
 
 
 class AddTenorDGen(DGen):
     def __init__(self, gen, tenor):
         self.gen = gen
         self.tenor = tenor
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         start = start if start is not date.min else after
-        start = self.tenor.sub_from(start, calendar) if not self.tenor.is_neg() else start
-        yield from (self.tenor.add_to(d, calendar) for d in self.gen.__invoke__(start, end, after, before, calendar))
+        start = self.tenor.sub_from(start, calendar) if not self.tenor.is_neg() and start is not date.min else start
+        yield from (self.tenor.add_to(d, calendar) for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs))
+
+    def __repr__(self):
+        return f'{self.gen} + {self.tenor}'
 
 
 class SubTenorDGen(DGen):
     def __init__(self, gen, tenor):
         self.gen = gen
         self.tenor = tenor
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         end = end if end is not date.max else before
         if end is not date.max:
             end = self.tenor.add_to(end, calendar) if not self.tenor.is_neg() else end
-        yield from (self.tenor.sub_from(d, calendar) for d in self.gen.__invoke__(start, end, after, before, calendar))
+        yield from (self.tenor.sub_from(d, calendar) for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs))
+
+    def __repr__(self):
+        return f'{self.gen} - {self.tenor}'
 
 
 class JoinDGen(DGen):
     def __init__(self, gen1, gen2):
         self.gen1 = gen1
         self.gen2 = gen2
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        g1 = self.gen1.__invoke__(start, end, after, before, calendar)
-        g2 = self.gen2.__invoke__(start, end, after, before, calendar)
+                   calendar: Calendar = None, **kwargs):
+        g1 = self.gen1.__invoke__(start, end, after, before, calendar, **kwargs)
+        g2 = self.gen2.__invoke__(start, end, after, before, calendar, **kwargs)
 
         d1 = next(g1, None)
         d2 = next(g2, None)
         while d1 is not None or d2 is not None:
             if d1 is None:
                 yield d2
                 while (d2 := next(g2, None)) is not None:
@@ -448,47 +535,53 @@
             elif d1 < d2:
                 yield d1
                 d1 = next(g1, None)
             else:
                 yield d2
                 d2 = next(g2, None)
 
+    def __repr__(self):
+        return f'{self.gen1} | {self.gen2}'
+
 
 class CommonDatesDGen(DGen):
     def __init__(self, gen1, gen2):
         self.gen1 = gen1
         self.gen2 = gen2
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        g1 = self.gen1.__invoke__(start, end, after, before, calendar)
-        g2 = self.gen2.__invoke__(start, end, after, before, calendar)
+                   calendar: Calendar = None, **kwargs):
+        g1 = self.gen1.__invoke__(start, end, after, before, calendar, **kwargs)
+        g2 = self.gen2.__invoke__(start, end, after, before, calendar, **kwargs)
 
         d1 = next(g1, None)
         d2 = next(g2, None)
         while d1 is not None and d2 is not None:
             if d1 == d2:
                 yield d1
                 d1 = next(g1, None)
                 d2 = next(g2, None)
             elif d1 < d2:
                 d1 = next(g1, None)
             else:
                 d2 = next(g2, None)
 
+    def __repr__(self):
+        return f'{self.gen1} & {self.gen2}'
+
 
 class RemoveDatesDGen(DGen):
     def __init__(self, gen1, gen2):
         self.gen1 = gen1
         self.gen2 = gen2
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        g1 = self.gen1.__invoke__(start, end, after, before, calendar)
-        g2 = self.gen2.__invoke__(start, end, after, before, calendar)
+                   calendar: Calendar = None, **kwargs):
+        g1 = self.gen1.__invoke__(start, end, after, before, calendar, **kwargs)
+        g2 = self.gen2.__invoke__(start, end, after, before, calendar, **kwargs)
 
         d1 = next(g1, None)
         d2 = next(g2, None)
         while d1 is not None and d2 is not None:
             if d1 == d2:
                 d1 = next(g1, None)
                 d2 = next(g2, None)
@@ -498,21 +591,24 @@
             else:
                 d2 = next(g2, None)
         if d2 is None:
             while d1 is not None:
                 yield d1
                 d1 = next(g1, None)
 
+    def __repr__(self):
+        return f'{self.gen1} - {self.gen2}'
+
 
 class MonthsDGen(DGen):
     def cadence(self):
         return Tenor('1m')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         start = start if start is not date.min else after
         end = end if end is not date.max else before
 
         first = date(start.year, start.month, 1)
         while first <= end:
             yield first
             year = first.year + first.month // 12
@@ -563,14 +659,17 @@
     def sat(self):
         return SubSequenceDGen(self, DayOfWeekDGen(5))
 
     @property
     def sun(self):
         return SubSequenceDGen(self, DayOfWeekDGen(6))
 
+    def __repr__(self):
+        return 'months'
+
 
 months = MonthsDGen()
 
 
 class SubSequenceDGen(DGen):
     def __init__(self, main_sequence, sub_sequence, slice = None):
         if main_sequence.cadence() in (None, Tenor('1d')):
@@ -584,16 +683,16 @@
         if isinstance(pr := getattr(type(self.sub_sequence),name),property):
             return pr.fget(self)
 
     def cadence(self):
         return self.sub_sequence.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        for begin in self.main_sequence.__invoke__(start, end, after, before, calendar):
+                   calendar: Calendar = None, **kwargs):
+        for begin in self.main_sequence.__invoke__(start, end, after, before, calendar, **kwargs):
             end = self.main_sequence.cadence().add_to(begin)
             sub_sequence = cast(DGen, begin <= self.sub_sequence < end)
             if self.slice is None:
                 yield from (d for d in sub_sequence() if d < before)
             else:
                 if is_negative_slice(self.slice):
                     yield from [d for d in sub_sequence() if d < before][self.slice]
@@ -604,32 +703,48 @@
         if isinstance(item, int):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, slice(item, item + 1))
         if isinstance(item, slice):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, item)
         if isinstance(item, Op):
             return lazy(self)[item]
 
+    def __repr__(self):
+        if self.slice is None:
+            sl_str = ""
+        else:
+            if self.slice.start == self.slice.stop - 1:
+                sl_str = f"[{self.slice.start}]"
+            elif self.slice.step is None:
+                sl_str = f"[{self.slice.start}:{self.slice.stop}]"
+            else:
+                sl_str = f"[{self.slice.start}:{self.slice.stop}:{self.slice.step}]"
+        return f'{self.main_sequence}.{self.sub_sequence}{sl_str}'
+
+
 class DaysOfMonthDGen(DGen):
     def __init__(self, months, days):
         self.months = months
         self.days = days
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        for month in self.months.__invoke__(start, end, after, before, calendar):
+                   calendar: Calendar = None, **kwargs):
+        for month in self.months.__invoke__(start, end, after, before, calendar, **kwargs):
             next_month = Tenor('1m').add_to(month)
             yield from (month <= self.days < next_month)()
 
+    def __repr__(self):
+        return f'{self.months}.{self.days}'
+
 
 class YearsDGen(DGen):
     def cadence(self):
         return Tenor('1y')
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         start = start if start is not date.min else after
         end = end if end is not date.max else before
 
         first = date(start.year, 1, 1)
         while first <= end:
             yield first
             first = date(first.year + 1, 1, 1)
@@ -702,74 +817,134 @@
     def weekdays(self):
         return SubSequenceDGen(self, weekdays)
 
     @property
     def weekends(self):
         return SubSequenceDGen(self, weekends)
 
+    def __repr__(self):
+        return 'years'
+
 
 years = YearsDGen()
 
 
 class SliceDGen(DGen):
     def __init__(self, gen, slice):
         self.gen = gen
         self.slice = slice
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
-        yield from islice(self.gen.__invoke__(start, end, after, before, calendar), self.slice.start, self.slice.stop, self.slice.step)
+                   calendar: Calendar = None, **kwargs):
+        yield from islice(self.gen.__invoke__(start, end, after, before, calendar, **kwargs), self.slice.start, self.slice.stop, self.slice.step)
+
+    def __repr__(self):
+        return f'{self.gen}[{self.slice}]'
 
 
 class WithCalendarDGen(DGen):
     def __init__(self, gen, calendar):
         self.gen = gen
         self.calendar = calendar
 
     def cadence(self):
         return self.gen.cadence
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         yield from (d for d in self.gen.__invoke__(start, end, after, before, self.calendar))
 
+    def __repr__(self):
+        return f'{self.gen}.over({self.calendar})'
+
 
 class RollFwdDGen(DGen):
     def __init__(self, gen, calendar=None):
         self.gen = gen
         self.calendar = calendar
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         c = self.calendar or calendar
         assert c, 'Business days calculation requires a calendar'
-        yield from (c.add_business_days(d, 0) for d in self.gen.__invoke__(start, end, after, before, calendar))
+        yield from (c.add_business_days(d, 0) for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs))
+
+    def __repr__(self):
+        return f'roll_fwd({self.gen})' if self.calendar is None else f'roll_fwd({self.gen}, {self.calendar})'
 
 
 def roll_fwd(x, calendar=None):
-    return RollFwdDGen(x, calendar)
+    if is_op(x) or is_op(calendar):
+        return lazy(roll_bwd)(x, calendar)
+    else:
+        return RollFwdDGen(x, calendar)
 
 
 class RollBwdDGen(DGen):
     def __init__(self, gen, calendar=None):
         self.gen = gen
         self.calendar = calendar
 
     def cadence(self):
         return self.gen.cadence()
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
-                   calendar: Calendar = None):
+                   calendar: Calendar = None, **kwargs):
         c = self.calendar or calendar
         assert c, 'Business days calculation requires a calendar'
-        yield from (c.sub_business_days(d, 0) for d in self.gen.__invoke__(start, end, after, before, calendar))
+        yield from (c.sub_business_days(d, 0) for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs))
+
+    def __repr__(self):
+        return f'roll_bwd({self.gen})' if self.calendar is None else f'roll_bwd({self.gen}, {self.calendar})'
 
 
 def roll_bwd(x, calendar=None):
-    return RollBwdDGen(x, calendar)
+    if is_op(x) or is_op(calendar):
+        return lazy(roll_bwd)(x, calendar)
+    else:
+        return RollBwdDGen(x, calendar)
+
+
+class DGenRetain(DGen):
+    def __init__(self, gen):
+        self.gen = gen
+        self.last = None
+
+    def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
+                   calendar: Calendar = None, **kwargs):
+        for d in self.gen.__invoke__(start, end, after, before, calendar, **kwargs):
+            self.last = d
+            yield d
+
+    def __repr__(self):
+        return f'retain({self.gen})'
+
+
+def retain(x):
+    if is_op(x):
+        return lazy(retain)(x)
+    else:
+        return DGenRetain(x)
+
+
+class DGenParameter(DGen):
+    def __init__(self, name):
+        self.name = name
+
+    def is_single_date_gen(self):
+        return True
+
+    def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
+                   calendar: Calendar = None, **kwargs):
+        if v := kwargs.get(self.name, None):
+            yield make_date(v)
+        else:
+            raise ValueError(f'Parameter {self.name} is not provided')
 
+    def __repr__(self):
+        return self.name
```

### Comparing `hg_oap-0.1.1/src/hg_oap/dates/tenor.py` & `hg_oap-0.1.2/src/hg_oap/dates/tenor.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,38 @@
 
 __all__ = ('Tenor',)
 
 
 class Tenor:
     ymwd_b: tuple[int, int, int, int, int]
 
-    def __init__(self, tenor):
-        if type(tenor) is str:
-            if m := re.match(r"^(-)?(?:(?:(\d+)y)?(?:(\d+)m)?(?:(\d+)w)?(?:(\d+)d)?|(?:(\d+)b)?)$", tenor):
-                sign, y, m, w, d, b = m.groups()
-                s, y, m, w, d, b = not sign, int(y or 0), int(m or 0), int(w or 0), int(d or 0), int(b or 0)
-                if sign:
-                    y, m, w, d, b = -y, -m, -w, -d, -b
-
-                self.ymwd_b = (y, m, w, d, b)
+    def __init__(self, tenor=None, /, *, y=0, m=0, w=0, d=0, b=0):
+        if tenor is not None:
+            assert not any((y, m, w, d, b)), 'cannot specify both a tenor and individual components'
+
+            if type(tenor) is str:
+                if m := re.match(r"^(-)?(?:(?:(\d+)y)?(?:(\d+)m)?(?:(\d+)w)?(?:(\d+)d)?|(?:(\d+)b)?)$", tenor):
+                    sign, y, m, w, d, b = m.groups()
+                    s, y, m, w, d, b = not sign, int(y or 0), int(m or 0), int(w or 0), int(d or 0), int(b or 0)
+                    if sign:
+                        y, m, w, d, b = -y, -m, -w, -d, -b
+
+                    self.ymwd_b = (y, m, w, d, b)
+                else:
+                    raise ValueError(f'"{tenor}" is a invalid tenor string')
+            elif type(tenor) is Tenor:
+                self.ymwd_b = tenor.ymwd_b
+            elif type(tenor) is timedelta:
+                self.ymwd_b = (0, 0, 0, tenor.days, 0)
+            elif type(tenor) is tuple and len(tenor) == 5 and all(isinstance(i, int) for i in tenor):
+                self.ymwd_b = tenor
             else:
-                raise ValueError(f'"{tenor}" is a invalid tenor string')
-        elif type(tenor) is Tenor:
-            self.ymwd_b = (tenor.y, tenor.m, tenor.w, tenor.d, tenor.b)
-        elif type(tenor) is timedelta:
-            self.ymwd_b = (0, 0, 0, tenor.days, 0)
-        elif type(tenor) is tuple and len(tenor) == 5 and all(isinstance(i, int) for i in tenor):
-            self.ymwd_b = tenor
+                raise ValueError(f'"{tenor}" is a invalid tenor value')
         else:
-            raise ValueError(f'"{tenor}" is a invalid tenor value')
+            self.ymwd_b = (y, m, w, d, b)
 
     def __str__(self):
         s = sum(self.ymwd_b)
         if s == 0:
             return '0d'
 
         sign = '-' if s < 0 else ''
```

### Comparing `hg_oap-0.1.1/src/hg_oap/instruments/commodity.py` & `hg_oap-0.1.2/src/hg_oap/instruments/commodity.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/instruments/future.py` & `hg_oap-0.1.2/src/hg_oap/instruments/future.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from dataclasses import dataclass
 from datetime import date
-from decimal import Decimal
 from enum import Enum
+from typing import Type, Callable
+
+from hg_oap.utils.op import Op, lazy
+from hgraph import CompoundScalar
 
 from hg_oap.assets.currency import Currency
 from hg_oap.dates.calendar import Calendar
-from hg_oap.dates.dgen import DGen
-from hg_oap.dates.tenor import Tenor
+from hg_oap.dates.dgen import DGen, DGenParameter, make_dgen
 from hg_oap.instruments.instrument import Instrument, INSTRUMENT_ID
-from hg_oap.units import U
+from hg_oap.units.default_unit_system import U
 from hg_oap.units.quantity import Quantity
 from hg_oap.units.unit import Unit
 from hg_oap.units.unit_system import UnitConversionContext
-from hg_oap.utils import ExprClass, SELF, ParameterOp, lazy
-from hgraph import CompoundScalar
+from hg_oap.utils import ExprClass, Expression, SELF, ParameterOp
 
 
 class SettlementMethod(Enum):
     Deliverable: str = "Deliverable"
     Financial: str = "Financial"
 
 
@@ -30,53 +31,58 @@
 
 
 @dataclass(frozen=True)
 class FutureContractSpec(CompoundScalar, ExprClass, UnitConversionContext):
     """
     The specification of a future contract.
     """
-    exchange: str
+    exchange_mic: str
     symbol: str
     underlying: Instrument
-    contract_size: Quantity[Decimal]
+    contract_size: Quantity[float]
     currency: Currency
 
     trading_calendar: Calendar
     settlement: Settlement
 
     quotation_currency_unit: Unit
     quotation_unit: Unit
-    tick_size: Quantity[Decimal]
+    tick_size: Quantity[float]
 
-    unit_conversion_factors: tuple[Quantity[Decimal]] = \
-        lambda self: self.underlying.unit_conversion_factors + (self.contract_size/(Decimal(1.)*U.lot),)
+    unit_conversion_factors: tuple[Quantity[float]] = \
+        lambda self: self.underlying.unit_conversion_factors + (self.contract_size/(1.*U.lot),)
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, kw_only=True)
 class FutureContractSeries(CompoundScalar, ExprClass, UnitConversionContext):
+    SELF: "FutureContractSeries" = SELF
     """
     A series of future contracts.
     """
 
     spec: FutureContractSpec
     name: str
-    symbol: INSTRUMENT_ID
+    symbol: str = SELF.spec.symbol + SELF.name
+    future_type: Type[Instrument] = lambda self: Future
     frequency: DGen  # a date generator that produces "contract base dates"
 
-    expiry: DGen # given a contract base date, produces the expiry date
+    symbol_expr: Expression[[Instrument], str]
+
+    expiry: Expression[[date], date]  # given a contract base date, produces the expiry date
 
-    first_trading_date: DGen  # given a contract base date, produces the first trading date
-    last_trading_date: DGen  # given a contract base date, produces the last trading date
+    first_trading_date: Expression[[date], date]  # given a contract base date, produces the first trading date
+    last_trading_date: Expression[[date], date]  # given a contract base date, produces the last trading date
 
 
-CONTRACT_BASE_DATE = ParameterOp(0, "contract_base_date")
+CONTRACT_BASE_DATE = lazy(make_dgen)(ParameterOp(_name="CONTRACT_BASE_DATE"))
 
 
-def month_code(d: date) -> str:
-    return ['F', 'G', 'H', 'J', 'K', 'M', 'N', 'Q', 'U', 'V', 'X', 'Z'][d.month - 1]
+def month_code(d: int | date) -> str:
+    m = (d.month if type(d) is date else d) - 1
+    return ['F', 'G', 'H', 'J', 'K', 'M', 'N', 'Q', 'U', 'V', 'X', 'Z'][m]
 
 
 @dataclass(frozen=True, kw_only=True)
 class Future(Instrument):
     SELF: "Future" = SELF
 
     """
@@ -84,14 +90,15 @@
     future.
     """
 
     series: FutureContractSeries
     contract_base_date: date
 
     name: str = lambda self: self.series.name + self.contract_base_date.strftime("%b %y")
-    symbol: str = lambda self: f"{self.series.symbol}{month_code(self.contract_base_date)}{self.contract_base_date.year % 10}"
+    symbol: str = SELF.series.symbol_expr(SELF)
+
 
-    expiry: date = SELF.series.expiry(SELF.contract_base_date)
-    first_trading_date: date = SELF.series.first_trading_date(SELF.contract_base_date)
-    last_trading_date: date = SELF.series.last_trading_date(SELF.contract_base_date)
+    expiry: date = SELF.series.expiry(CONTRACT_BASE_DATE=SELF.contract_base_date)
+    first_trading_date: date = SELF.series.first_trading_date(CONTRACT_BASE_DATE=SELF.contract_base_date)
+    last_trading_date: date = SELF.series.last_trading_date(CONTRACT_BASE_DATE=SELF.contract_base_date)
 
-    unit_conversion_factors: tuple[Quantity[Decimal]] = SELF.series.spec.unit_conversion_factors
+    unit_conversion_factors: tuple[Quantity[float]] = SELF.series.spec.unit_conversion_factors
```

### Comparing `hg_oap-0.1.1/src/hg_oap/instruments/instrument.py` & `hg_oap-0.1.2/src/hg_oap/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/orders/order.py` & `hg_oap-0.1.2/src/hg_oap/orders/order.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/orders/order_service.py` & `hg_oap-0.1.2/src/hg_oap/orders/order_service.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/orders/order_type.py` & `hg_oap-0.1.2/src/hg_oap/orders/order_type.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/portfolio/portfolio.py` & `hg_oap-0.1.2/src/hg_oap/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/pricing/price.py` & `hg_oap-0.1.2/src/hg_oap/pricing/price.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/units/U.py` & `hg_oap-0.1.2/src/hg_oap/units/default_unit_system.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,76 @@
 import math
-from decimal import Decimal
 
 from hg_oap.units.dimension import PrimaryDimension, Dimensionless
 from hg_oap.units.unit import PrimaryUnit, DerivedUnit, OffsetDerivedUnit
 from hg_oap.units.unit_system import UnitSystem
 
 __all__ = ("U")
 
 
-std_prefixes = {'k': Decimal('1000'), 'M': Decimal('1_000_000'), 'G': Decimal('1_000_000_000'), 'T': Decimal('1_000_000_000_000'),
-                'c': Decimal('0.01'), 'm': Decimal('0.001'), 'u': Decimal('0.000_001'), 'n': Decimal('0.000_000_001'), 'p': Decimal('0.000_000_000_001')}
+std_prefixes = {'k': 1000.0, 'M': 1_000_000.0, 'G': 1_000_000_000.0, 'T': 1_000_000_000_000.0,
+                'c': 0.01, 'm': 0.001, 'u': 0.000_001, 'n': 0.000_000_001, 'p': 0.000_000_000_001}
 
 U = UnitSystem(__prefixes__=std_prefixes)
-U.__enter__()  # on import this unit system becomes the implicit default.
-               # Tests can still create their own unit systems and use them as context managers.
-
+U.register()  # If this has been imported we can go ahead and register it.
 
 U.length = PrimaryDimension()
 U.m = PrimaryUnit(dimension=U.length, prefixes=('k', 'c', 'm', 'u', 'n'))
-U.mi = DerivedUnit(primary_unit=U.m, ratio=Decimal('1609.344'))
-U.nautical_mile = DerivedUnit(primary_unit=U.m, ratio=Decimal('1852'))
+U.mi = DerivedUnit(primary_unit=U.m, ratio=1609.344)
+U.nautical_mile = DerivedUnit(primary_unit=U.m, ratio=1852.0)
 
 U.area = U.length**2
-U.hectare = DerivedUnit(primary_unit=U.m**2, ratio=Decimal('10000'))
-U.acre = DerivedUnit(primary_unit=U.m**2, ratio=Decimal('4046.8564224'))
+U.hectare = DerivedUnit(primary_unit=U.m**2, ratio=10000.0)
+U.acre = DerivedUnit(primary_unit=U.m**2, ratio=4046.8564224)
 
 U.volume = U.length**3
-U.l = DerivedUnit(primary_unit=U.m**3, ratio=Decimal('0.001'))
-U.bushel = DerivedUnit(primary_unit=U.m**3, ratio=Decimal('0.03523907'))
+U.l = DerivedUnit(primary_unit=U.m**3, ratio=0.001)
+U.bushel = DerivedUnit(primary_unit=U.m**3, ratio=0.03523907)
 
 U.weight = PrimaryDimension()
 U.kg = PrimaryUnit(dimension=U.weight)
-U.g = DerivedUnit(primary_unit=U.kg, ratio=Decimal('0.001'), prefixes=('k', 'm'))
-U.mt = Decimal('1000') * U.kg
-U.pound = DerivedUnit(primary_unit=U.kg, ratio=Decimal('0.45359237'))
-U.toz = DerivedUnit(primary_unit=U.kg, ratio=Decimal(1)/Decimal('32.1507'))
+U.g = DerivedUnit(primary_unit=U.kg, ratio=0.001, prefixes=('k', 'm'))
+U.mt = 1000 * U.kg
+U.pound = DerivedUnit(primary_unit=U.kg, ratio=0.45359237)
+U.toz = DerivedUnit(primary_unit=U.kg, ratio=1.0/32.1507)
 
 U.time = PrimaryDimension()
 absolute_seconds = PrimaryUnit(dimension=U.time)
 U.seconds_since_epoch = OffsetDerivedUnit(primary_unit=absolute_seconds)
 U.s = U.seconds_since_epoch.diff
 U.add_prefixes(U.s, ('m', 'u', 'n'))
 
-U.min = Decimal('60') * U.s
-U.h = Decimal('60') * U.min
-U.day = Decimal('24') * U.h
-U.week = Decimal('7') * U.day
+U.min = 60.0 * U.s
+U.h = 60.0 * U.min
+U.day = 24.0 * U.h
+U.week = 7.0 * U.day
 
 U.velocity = U.length / U.time
 U.kph = U.km / U.h
 U.mph = U.mi / U.h
 
 U.temperature = PrimaryDimension()
 U.K = PrimaryUnit(dimension=U.temperature)
-U.degC = OffsetDerivedUnit(primary_unit=U.K, ratio=Decimal('1'), offset=Decimal('273.15'))
-U.degF = OffsetDerivedUnit(primary_unit=U.K, ratio=Decimal('5')/Decimal('9'), offset=Decimal('459.67'))
+U.degC = OffsetDerivedUnit(primary_unit=U.K, ratio=1.0, offset=273.15)
+U.degF = OffsetDerivedUnit(primary_unit=U.K, ratio=5.0/9.0, offset=459.67)
 
 U.energy = U.weight * U.length**2 / U.time**2
 U.J = PrimaryUnit(dimension=U.energy)
-U.cal = DerivedUnit(primary_unit=U.J, ratio=Decimal('4.184'))
+U.cal = DerivedUnit(primary_unit=U.J, ratio=4.184)
 
 U.power = U.energy / U.time
 U.W = PrimaryUnit(dimension=U.power, prefixes=('k', 'M', 'G', 'T', 'm'))
 
 U.Wh = U.W * U.h
 U.add_prefixes(U.Wh, ('k', 'M', 'G', 'T'))
 
 U.dimentionless = Dimensionless()
 U.turn = PrimaryUnit(dimension=U.dimentionless)
-U.rad = DerivedUnit(primary_unit=U.turn, ratio=Decimal(2)*Decimal(math.pi))
-U.deg = DerivedUnit(primary_unit=U.rad, ratio=Decimal(1)/Decimal(360))
+U.rad = DerivedUnit(primary_unit=U.turn, ratio=2.0*math.pi)
+U.deg = DerivedUnit(primary_unit=U.rad, ratio=1.0/360.0)
 
 U.rpm = U.turn / U.min
 
 U.contracts = PrimaryDimension()
 U.lot = PrimaryUnit(dimension=U.contracts)
 
 U.money = PrimaryDimension()
```

### Comparing `hg_oap-0.1.1/src/hg_oap/units/dimension.py` & `hg_oap-0.1.2/src/hg_oap/units/dimension.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/src/hg_oap/units/quantity.py` & `hg_oap-0.1.2/src/hg_oap/units/quantity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from dataclasses import dataclass
 from numbers import Number
 from typing import Generic
 
 from hg_oap.units.unit import Unit, NUMBER
-from hgraph import CompoundScalar
+from hgraph import CompoundScalar, compute_node, div_, TS
 
 __all__ = ("Quantity",)
 
 
+EPSILON = 1e-9
+
+
 @dataclass(frozen=True)
 class Quantity(CompoundScalar, Generic[NUMBER]):
     qty: NUMBER
     unit: Unit
 
     def __str__(self):
         return f"{self.qty} {self.unit}"
 
     def __repr__(self):
         return f"{self.qty}*{self.unit}"
 
     def __eq__(self, other):
         if isinstance(other, Quantity):
-            return self.qty == other.unit.convert(other.qty, to=self.unit)
+            other_qty = other.unit.convert(other.qty, to=self.unit)
+            return other_qty - EPSILON <= self.qty <= other_qty + EPSILON
 
         return NotImplemented
 
     def __add__(self, other):
         if isinstance(other, Quantity):
             ret, conv = self.unit + other.unit
             return Quantity[type(self.qty)](self.qty + other.unit.convert(other.qty, to=conv), ret)
@@ -106,7 +110,11 @@
 
     def __pos__(self):
         return Quantity[type(self.qty)](+self.qty, self.unit)
 
     def as_(self, unit):
         return Quantity[type(self.qty)](self.unit.convert(self.qty, to=unit), unit)
 
+
+@compute_node(overloads=div_)
+def div_qty(lhs: TS[Quantity], rhs: TS[Quantity]) -> TS[Quantity]:
+    return lhs.value / rhs.value
```

### Comparing `hg_oap-0.1.1/src/hg_oap/units/unit.py` & `hg_oap-0.1.2/src/hg_oap/units/unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import operator
 
 from abc import abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
-from decimal import Decimal
 from functools import reduce
 from typing import Tuple, ForwardRef, TypeVar, ClassVar
 
 from hg_oap.units.dimension import Dimension
 from hg_oap.utils.exprclass import ExprClass
 from hg_oap.units.unit_system import UnitSystem
 from hgraph import CompoundScalar
 
-NUMBER = TypeVar('NUMBER', int, float, Decimal)
+NUMBER = TypeVar('NUMBER', int, float)
 
 __all__ = ("Unit", "PrimaryUnit", "DerivedUnit", "OffsetDerivedUnit", "DiffDerivedUnit", "ComplexUnit", "UNIT")
 
 @dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class Unit(CompoundScalar, ExprClass):
     name: str = None
     dimension: Dimension
@@ -28,22 +27,22 @@
     def __repr__(self):
         return self.name
 
     def __hash__(self):
         return id(self)  # units are singletons within a UnitSystem by construction so this is safe
 
     def __rmul__(self, value):
-        if isinstance(value, (int, float, Decimal)):
+        if isinstance(value, (int, float)):
             from hg_oap.units.quantity import Quantity
             return Quantity(value, self)
 
         return NotImplemented
 
     def __rtruediv__(self, value):
-        if isinstance(value, (int, float, Decimal)):
+        if isinstance(value, (int, float)):
             from hg_oap.units.quantity import Quantity
             return Quantity(value, self**-1)
 
         return NotImplemented
 
     def __mul__(self, other) -> 'Unit':
         return NotImplemented
@@ -86,15 +85,15 @@
 
 
 UNIT = TypeVar("UNIT", bound=Unit)
 
 
 @dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class PrimaryUnit(Unit):
-    ratio: Decimal = Decimal(1)
+    ratio: float = 1.0
 
     def __new__(cls, name=None, dimension: Dimension = None, prefixes=None):
         if d := UnitSystem.instance().__primary_units__.get(dimension):
             assert d.dimension is dimension
             return d
 
         n = super().__new__(cls)
@@ -140,19 +139,19 @@
 
         assert False, f'conversion from {self} to {to} is not supported'
 
 
 @dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class DerivedUnit(Unit):
     primary_unit: Unit
-    ratio: Decimal
+    ratio: float
     dimension: Dimension = lambda s: s.primary_unit.dimension
     name: str = lambda s: f"{s.ratio}*{s.primary_unit.name}"
 
-    def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: Decimal = Decimal(1), name=None, prefixes=None):
+    def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: float = 1.0, name=None, prefixes=None):
         from .quantity import Quantity
         if type(primary_unit) is Quantity:
             ratio = primary_unit.qty
             primary_unit = primary_unit.unit
 
         if type(primary_unit) is DerivedUnit:
             ratio *= primary_unit.ratio
@@ -200,20 +199,20 @@
             return self.primary_unit._do_convert(primary_value, to)
         else:
             return primary_value
 
 
 @dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class OffsetDerivedUnit(DerivedUnit):
-    offset: Decimal
+    offset: float
     diff: Unit = field(default=lambda s: DiffDerivedUnit(offset_unit=s), hash=False)
 
     _is_multiplicative: ClassVar[bool] = False
 
-    def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: Decimal = Decimal(1), offset: Decimal = Decimal(0), name=None, prefixes=None):
+    def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: float = 1.0, offset: float = 0.0, name=None, prefixes=None):
         if type(primary_unit) is DerivedUnit:
             primary_unit = primary_unit.primary_unit
             ratio *= primary_unit.ratio
 
         if d := UnitSystem.instance().__derived_units__.get((primary_unit, ratio, offset)):
             return d
 
@@ -255,15 +254,15 @@
             return primary_value
 
 
 @dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class DiffDerivedUnit(DerivedUnit):
     offset_unit: Unit = None
     primary_unit: Unit = lambda s: s.offset_unit.primary_unit
-    ratio: Decimal = lambda s: s.offset_unit.ratio
+    ratio: float = lambda s: s.offset_unit.ratio
     name: str = lambda s: f"{s.offset_unit.name}_diff"
 
     _is_multiplicative: ClassVar[bool] = True
 
     def __new__(cls, offset_unit: OffsetDerivedUnit, name=None):
         if type(offset_unit) is not OffsetDerivedUnit:
             raise ValueError(f"cannot create a diff unit from {offset_unit}")
@@ -292,17 +291,17 @@
 
         return NotImplemented
 
 
 @dataclass(frozen=True, kw_only=True, init=False)
 class ComplexUnit(Unit):
     components: Tuple[Tuple[Unit, int], ...]
-    scale: Decimal = Decimal(1)
+    scale: float = 1.0
     dimension: Dimension = lambda s: reduce(operator.mul, (u.dimension**m for u, m in s.components))
-    ratio: Decimal = lambda s: reduce(operator.mul, (pow(u.ratio, m) for u, m in s.components)) * s.scale
+    ratio: float = lambda s: reduce(operator.mul, (pow(u.ratio, m) for u, m in s.components)) * s.scale
     name: str = lambda s: s._build_name()
 
     def __new__(cls, components, name=None, prefixes=None):
         from hg_oap.units.quantity import Quantity
         if isinstance(components, Quantity):
             scale = components.qty
             components = components.unit._to_components()
@@ -333,15 +332,15 @@
         scale = f"{self.scale}*" if self.scale != 1 else ''
         up = '*'.join(f"{d}**{p}" if p != 1 else str(d) for d, p in self.components if p > 0) or '1'
         dn = ('*'.join(f"{d}**{abs(p)}" if p != -1 else str(d) for d, p in self.components if p < 0))
         dn = ('/' + dn) if dn else ''
         return scale + up + dn
 
     def _to_components(self, power=1):
-        if type(self).name.__overriden__(self) or self.scale != Decimal(1):
+        if type(self).name.__overriden__(self) or self.scale != 1.0:
             return super()._to_components(power)
         else:
             return self.components if power == 1 else tuple((u, p * power) for u, p in self.components)
 
     def __pow__(self, power, modulo=None):
         return ComplexUnit(components=tuple((u, p * power) for u, p in self.components))
```

### Comparing `hg_oap-0.1.1/src/hg_oap/units/unit_system.py` & `hg_oap-0.1.2/src/hg_oap/units/unit_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import operator
 from dataclasses import dataclass, field
-from decimal import Decimal
 from functools import reduce
 from itertools import chain, combinations
-from typing import ClassVar, Tuple, Iterable
+from typing import ClassVar, Tuple, Iterable, Callable
 
 from hg_oap.utils.exprclass import CallableDescriptor
 
 
 __all__ = ("UnitSystem", "UnitConversionContext")
 
+
 @dataclass
 class UnitSystem:
     __instance__: ClassVar['UnitSystem'] = None
 
     __dimensions__: dict[str, "Dimension"] = field(default_factory=dict)
     __derived_dimensions__: dict[tuple[tuple["Dimension", int], ...], "Dimension"] = field(default_factory=dict)
 
     __primary_units__: dict[str, "Unit"] = field(default_factory=dict)
-    __derived_units__: dict[Tuple["Unit", Decimal], "Unit"] = field(default_factory=dict)
+    __derived_units__: dict[Tuple["Unit", float], "Unit"] = field(default_factory=dict)
     __complex_units__: dict[tuple[tuple["Unit", int], ...], "Unit"] = field(default_factory=dict)
 
     __contexts__: list["UnitConversionContext"] = field(default_factory=list)
-    __prefixes__: dict[str, Decimal] = field(default_factory=dict)
+    __prefixes__: dict[str, float] = field(default_factory=dict)
 
-    @classmethod
-    def instance(cls):
-        return cls.__instance__
+    @staticmethod
+    def instance():
+        if UnitSystem.__instance__ is None and UnitSystem.__default__ is not None:
+            from hg_oap.units import default_unit_system
+            UnitSystem.__instance__ = U
+        return UnitSystem.__instance__
+
+    def register(self):
+        """Register the unit system to make use of"""
+        UnitSystem.__instance__ = self
 
-    def __enter__(self):
-        if self.__class__.__instance__ is not None:
-            raise ValueError(f"UnitSystems are not stackable contexts")
+    @staticmethod
+    def de_register():
+        """De-register the unit system"""
+        UnitSystem.__instance__ = None
 
-        self.__class__.__instance__ = self
+    def __enter__(self):
+        """
+        Context manager enter, used largely for testing. This will replace any existing unit system.
+        """
+        self.register()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        assert self.__class__.__instance__ == self
-
-        self.__class__.__instance__ = None
+        self.de_register()
 
     def __setattr__(self, key, value):
         if key in self.__class__.__dataclass_fields__:
             object.__setattr__(self, key, value)
             return
 
         from hg_oap.units.quantity import Quantity
@@ -76,40 +86,40 @@
     def enter_context(self, context: "UnitConversionContext"):
         self.__contexts__.append(context)
 
     def exit_context(self, context: "UnitConversionContext"):
         assert self.__contexts__[-1] == context
         self.__contexts__.pop()
 
-    def conversion_factor(self, dimension: "Dimension") -> "Quantity[Decimal]":
+    def conversion_factor(self, dimension: "Dimension") -> "Quantity[float]":
         for context in reversed(self.__contexts__):
             if factor := context.conversion_factor(dimension):
                 return factor
 
         return None
 
 
 class UnitConversionContext:
-    def __init__(self, conversion_factors: tuple["Quantity[Decimal]"] = ()):
+    def __init__(self, conversion_factors: tuple["Quantity[float]"] = ()):
         self.unit_conversion_factors = conversion_factors
 
     def __enter__(self):
         UnitSystem.instance().enter_context(self)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         UnitSystem.instance().exit_context(self)
 
-    def conversion_factor(self, dimension: "Dimension") -> "Quantity[Decimal]":
+    def conversion_factor(self, dimension: float) -> "Quantity[float]":
         if (ucf := getattr(self, "_unit_conversion_factors_lookup", None)) is None:
             ucf = UnitConversionContext.make_conversion_factors(self.unit_conversion_factors)
             object.__setattr__(self, '_unit_conversion_factors_lookup', ucf)
 
         return ucf.get(dimension, None)
 
     @staticmethod
-    def make_conversion_factors(factors: Iterable["Quantity[Decimal]"]):
+    def make_conversion_factors(factors: Iterable["Quantity[float]"]):
         combination_factors = [[reduce(operator.mul, j)
                                 for j in combinations(factors, i)] for i in range(2, len(factors) + 1)]
 
-        all_factors = chain(*((f, Decimal(1)/f) for f in chain(factors, chain.from_iterable(combination_factors))))
+        all_factors = chain(*((f, 1.0/f) for f in chain(factors, chain.from_iterable(combination_factors))))
 
         return {q.unit.dimension: q for q in all_factors}
```

### Comparing `hg_oap-0.1.1/src/hg_oap/utils/exprclass.py` & `hg_oap-0.1.2/src/hg_oap/utils/exprclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import abstractmethod
 from dataclasses import dataclass, Field
 from datetime import date
 from inspect import isfunction, signature
 
-from hg_oap.dates.dgen import make_date, is_dgen
-from hg_oap.utils.op import Op, Expression, is_op
+from .op import Op, Expression, is_op, lazy
 
 __all__ = ("dataclassex", 'exprclass', 'ExprClass')
 
 
 class _BaseExDescriptor:
     def __init__(self, expr):
         self.expr = expr
@@ -49,46 +48,60 @@
 
 
 class CallableDescriptor(_BaseExDescriptor):
     def __calc__(self, instance):
         return self.expr(instance)
 
 
+class CallableExpressionDescriptor(_BaseExDescriptor):
+    def __calc__(self, instance):
+        expr = self.expr(SELF=instance, __partial__=True)
+        if is_op(expr):
+            return Expression(expr)
+        else:
+            return expr
+
+
 class DateDescriptor(_BaseExDescriptor):
     def __calc__(self, instance):
+        from hg_oap.dates import is_dgen, make_date
+
         r = self.expr(instance)
         if isinstance(r, date):
             return r
         elif is_dgen(r):
             return next(r())
         else:
             return make_date(r)
 
 
 class DateListDescriptor(_BaseExDescriptor):
     def __calc__(self, instance):
+        from hg_oap.dates import is_dgen, make_date
+
         r = self.expr(instance)
         if isinstance(r, date):
             return [r]
         elif is_dgen(r):
             return tuple(r())
         else:
             return make_date(r)
 
 
 def _process_ops_and_lambdas(cls):
     cls.__annotations__.pop('SELF', None)
 
     for k, a in cls.__annotations__.items():
         if (op := getattr(cls, k, None)) is not None:
-
             if a == date:  # special treatment for dates
                 descriptor_type = DateDescriptor
             elif a == list[date] or a == tuple[date]:
                 descriptor_type = DateListDescriptor
+            elif getattr(a, '__origin__', None) is Expression:
+                descriptor_type = CallableExpressionDescriptor
             else:
                 descriptor_type = CallableDescriptor
 
             if isinstance(op, Field) and op.default is not None:
                 d = _make_descriptor(a, cls, descriptor_type, k, op.default)
                 if d is not None:
                     op.default = d
@@ -97,21 +110,21 @@
                 if d is not None:
                     setattr(cls, k, d)
 
     return cls
 
 
 def _make_descriptor(annotation, cls, descriptor_type, name, op):
-    if isinstance(op, Op) and not is_op(annotation):
+    if isinstance(op, Op):
         descriptor = descriptor_type(Expression(op))
         descriptor.__set_name__(cls, name)
         return descriptor
     elif isfunction(op) and op.__name__ == '<lambda>':
         if len(signature(op).parameters) == 1:
-            descriptor = descriptor_type(op)
+            descriptor = descriptor_type(lambda SELF, __partial__=None: op(SELF) if __partial__ is None else op)
             descriptor.__set_name__(cls, name)
             return descriptor
 
 
 class ExprClass:
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
```

### Comparing `hg_oap-0.1.1/src/hg_oap/utils/op.py` & `hg_oap-0.1.2/src/hg_oap/utils/op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import itertools
 import operator
 from collections import defaultdict
 from typing import Callable, Union, Sequence, Mapping
 
-__all__ = ('lazy', 'calc', 'ParameterOp')
+__all__ = ('lazy', 'calc', 'ParameterOp', 'Expression')
 
 
 def is_op(obj):
     return isinstance(obj, Op)
 
 
 def make_op(obj):
@@ -463,15 +463,15 @@
         for a in self._args:
             a = a.__invoke__(*args, **kwargs) if isinstance(a, Op) else a
             if isinstance(a, FailedOp):
                 return a
             call_args.append(a)
 
         call_kwargs = {}
-        for k, v in self._kwargs:
+        for k, v in self._kwargs.items():
             v = v.__invoke__(*args, **kwargs) if isinstance(v, Op) else v
             if isinstance(v, FailedOp):
                 return v
             call_kwargs[k] = v
 
         fn: Callable = self._fn.__invoke__(*args, **kwargs)
         if isinstance(fn, FailedOp):
@@ -574,14 +574,16 @@
         return self._name if self._name else f"_{self._index}"
 
     def __invoke__(self, *args, **kwargs):
         if self._name is not None and self._name in kwargs:
             return kwargs[self._name]
         elif self._index is not None and len(args) > self._index:
             return args[self._index]
+        elif '__partial__' in kwargs:
+            return self
         else:
             return FailedOp(f"missing argument with {'name ' + self._name if self._name else ''}"
                             f"{' or ' if self._name and self._index is not None else ''}"
                             f"{'index ' + str(self._index) if self._index is not None else ''}")
 
     def __visit_operands__(self, fn):
         return None
@@ -772,15 +774,15 @@
     def __init__(self, op: Op):
         self._op = op
 
     def __call__(self, *args, **kwargs):
         return calc(self._op, *args, **kwargs)
 
     def __repr__(self):
-        return repr(self.op)
+        return repr(self._op)
 
     @property
     def __signature__(self):
         i_parameters = {}
         kw_parameters = []
         for p in find_parameters(self._op):
             if p._name is not None and p._index is not None:
@@ -795,8 +797,17 @@
         for i in range(last_index + 1):
             if i in i_parameters:
                 parametes.append(i_parameters[i])
             else:
                 parametes.append(inspect.Parameter(f'i{i}', inspect.Parameter.POSITIONAL_OR_KEYWORD))
 
         parametes.extend(kw_parameters)
-        return inspect.Signature(parametes)
+        return inspect.Signature(parametes)
+
+    def __class_getitem__(cls, params):
+        from typing import _SpecialGenericAlias
+        args, result = params
+        if isinstance(args, list):
+            params = tuple(args) + (result,)
+        else:
+            params = args + (result,)
+        return _SpecialGenericAlias(cls, 2)[params]
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/example/test_example.py` & `hg_oap-0.1.2/tests/unit/hg_oap/example/test_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from dataclasses import dataclass
 from datetime import date
-from decimal import Decimal
 from typing import Generic, TypeVar, Type
 
+import pytest
 from hgraph import CompoundScalar, TSB, TSD, Frame, graph, TS, map_, add_, switch_, compute_node, TSL, AUTO_RESOLVE, \
     subscription_service, request_reply_service, service_impl, CONTEXT, register_service
 from hgraph.nodes import merge, filter_, route_ref, tuple_from_ts, drop_dups, tsd_flip, make_tsd, const, cs_from_ts, \
     sample
 from hgraph.test import eval_node
 
 from hg_oap.assets.commodities import Commodity
 from hg_oap.assets.currency import Currencies
 from hg_oap.dates.calendar import WeekendCalendar
 from hg_oap.dates.dgen import roll_bwd, years
 from hg_oap.instruments.future import Settlement, SettlementMethod, FutureContractSpec, FutureContractSeries, \
-    CONTRACT_BASE_DATE, Future
+    CONTRACT_BASE_DATE, Future, month_code
 from hg_oap.instruments.fx import FXSpot
 from hg_oap.instruments.instrument import Instrument, INSTRUMENT_ID
 from hg_oap.instruments.physical import PhysicalCommodity
-from hg_oap.units import U
+from hg_oap.units.default_unit_system import U
 from hg_oap.units.quantity import Quantity
 from hg_oap.units.unit import Unit, NUMBER
 from hg_oap.units.unit_system import UnitConversionContext
 from hg_oap.utils import SELF, ExprClass
 
 
 #####################
@@ -211,42 +211,42 @@
 
 def test_example():
     @graph
     def g(prices: TSD[str, TSB[Price[float]]]) -> TS[Quantity[float]]:
         register_service("price_service", price_service)
         register_service("instrument_service", instrument_service)
 
-        corn = Agricultural(symbol='C', name="corn", unit=U.bushel, unit_conversion_factors=(Quantity(Decimal('0.75'), U.kg / U.l),))
+        corn = Agricultural(symbol='C', name="corn", unit=U.bushel, unit_conversion_factors=(Quantity(0.75, U.kg / U.l),))
         corn_future_months = FutureContractSeries(
             spec=FutureContractSpec(
-                exchange='CME',
+                exchange_mic='CME',
                 symbol='ZC',
                 underlying=PhysicalCommodity(symbol='Corn',asset=corn),
-                contract_size=Quantity(Decimal('5000'), U.bushel),
+                contract_size=Quantity(5000., U.bushel),
                 currency=Currencies.USD.value,
                 trading_calendar=WeekendCalendar(),
                 settlement=Settlement(SettlementMethod.Deliverable),
                 quotation_currency_unit=U.USX,
                 quotation_unit=U.bushel,
-                tick_size=Quantity(Decimal('0.25'), U.USX),
+                tick_size=Quantity(0.25, U.USX),
             ),
-            name='Corn Future',
-            symbol='ZC',
+            name='M',
+            symbol_expr=lambda future: f"{future.series.spec.symbol}{month_code(future.contract_base_date)}{future.contract_base_date.year % 10}",
             frequency=years.mar | years.may | years.jul | years.sep | years.dec,
             expiry=roll_bwd(CONTRACT_BASE_DATE + '15d').over(SELF.spec.trading_calendar),
             first_trading_date=CONTRACT_BASE_DATE - '3y' < years.dec.days[15],  # dec 15th 3 years before the expiry date (actual CME rules are more complex)
             last_trading_date=SELF.expiry(CONTRACT_BASE_DATE)
         )
-        zcm5 = Future(series=corn_future_months, contract_base_date=date(2025, 5, 1))
-        register_instrument(zcm5)
+        zck5 = Future(series=corn_future_months, contract_base_date=date(2025, 5, 1))
+        register_instrument(zck5)
 
         gbpusd = FXSpot(symbol='GBPUSD', base=Currencies.GBP.value, quote=Currencies.USD.value)
         register_instrument(gbpusd)
 
-        zcm5_position = Position[float](qty=100., unit=U.lot, instrument=zcm5)
+        zcm5_position = Position[float](qty=100., unit=U.lot, instrument=zck5)
         notional = calculate_notional(zcm5_position, currency=U.GBP)
 
         map_(lambda key, p: submit_price(key, p), prices)
 
         return cs_from_ts(Quantity[float], **notional.as_dict())
 
     assert eval_node(g, __trace__=dict(start=False, stop=False), prices=[None, {
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/orders/test_order_service.py` & `hg_oap-0.1.2/tests/unit/hg_oap/orders/test_order_service.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_calendar.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_calendar.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dataclassex.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dataclassex.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dgen.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import date, timedelta
 
 import holidays
 import pytest
 
 from hg_oap.dates.calendar import WeekendCalendar, HolidayCalendar
-from hg_oap.dates.dgen import make_date, make_dgen, days, weeks, weekdays, weekends, months, years, business_days, roll_fwd, \
-    roll_bwd
+from hg_oap.dates.dgen import make_date, make_dgen, days, weeks, weekdays, weekends, months, years, business_days, \
+    roll_fwd, \
+    roll_bwd, DGenParameter
 from hg_oap.utils.op import Expression
 from hg_oap.dates.tenor import Tenor
 
 
 @pytest.mark.parametrize(['s', 'valid'], [
         ('2y3m1w6d', True),
         ('3m', True),
@@ -206,7 +207,15 @@
     assert list(Expression(c)('2020-01-01', '2020-02-01')()) == [date(2020, 1, 3), date(2020, 1, 10), date(2020, 1, 17), date(2020, 1, 24), date(2020, 1, 31)]
 
     c = '2020-01-01' <= _0 < '2020-02-01'
     assert list(Expression(c)(months.fri)()) == [date(2020, 1, 3), date(2020, 1, 10), date(2020, 1, 17), date(2020, 1, 24), date(2020, 1, 31)]
 
     c = months.fri[_0]
     assert list(Expression(c)(1)(after='2020-01-01', before='2020-02-01')) == [date(2020, 1, 10)]
+
+
+def test_dgen_parameter():
+    _0 = DGenParameter('_0')
+    _1 = DGenParameter('_1')
+
+    c = _0 <= months.fri <= _1
+    assert list(c(_0='2020-01-01', _1='2020-02-01')) == [date(2020, 1, 3), date(2020, 1, 10), date(2020, 1, 17), date(2020, 1, 24), date(2020, 1, 31)]
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dimension.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_dimension.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from hg_oap.units.dimension import PrimaryDimension, DerivedDimension, Dimensionless
 from hg_oap.units.unit_system import UnitSystem
 
 
 def test_dimensions():
-    UnitSystem.__instance__ = None # TODO: Either make this stackable or only import U when requried
     with UnitSystem():
         length = PrimaryDimension(name='length')
         volume = length**3
         assert volume.name == 'length**3'
 
         weight = PrimaryDimension(name='weight')
         density = weight/volume
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_magic.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_magic.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_quantity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import math
-from decimal import Decimal
 
 from hg_oap.units.dimension import PrimaryDimension, Dimensionless
 from hg_oap.units.unit import PrimaryUnit, DerivedUnit, OffsetDerivedUnit
 from hg_oap.units.unit_system import UnitSystem
 
 def test_quantity_1():
-    from hg_oap.units.U import U
+    from hg_oap.units.default_unit_system import U
     with U:
         assert 1.*U.m == 1.*U.m
         assert 1.*U.m == 100.*U.cm
 
         assert 60.*U.s == 1.*U.min
 
         assert 1.*U.kWh == 3600000.*U.J
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity_ts.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_quantity_ts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from decimal import Decimal
 from typing import TypeVar, Type
 
 from hgraph import graph, TS, compute_node, TSB, TSL, AUTO_RESOLVE
 from hgraph.nodes import cs_from_ts, route_ref, filter_, merge
 from hgraph.test import eval_node
 
-from hg_oap.units import U
+from hg_oap.units.default_unit_system import U
 from hg_oap.units.quantity import Quantity
 from hg_oap.units.unit import Unit, NUMBER
 
 
 def test_quantity_ts():
 
     @compute_node
@@ -60,17 +59,17 @@
             return fr.value.convert(tp(1.), to=to.value)
 
     @compute_node
     def convert_units(qty: TS[NUMBER], fr: TS[Unit], to: TS[Unit]) -> TS[NUMBER]:
         return fr.value.convert(qty.value, to=to.value)
 
     @graph
-    def g(ts: TS[Decimal], u: TS[Unit], u1: TS[Unit]) -> TS[Quantity[Decimal]]:
-        v = TSB[Quantity[Decimal]].from_ts(qty=ts, unit=u)
+    def g(ts: TS[float], u: TS[Unit], u1: TS[Unit]) -> TS[Quantity[float]]:
+        v = TSB[Quantity[float]].from_ts(qty=ts, unit=u)
         return convert(v, u1).as_scalar_ts()
 
-    assert eval_node(g, ts=[Decimal(1.), None, Decimal(2.)], u=[U.kg, None, None], u1=[None, U.kg, U.g]) == [None, 1.*U.kg, 2000.*U.g]
+    assert eval_node(g, ts=[1.0, None, 2.0], u=[U.kg, None, None], u1=[None, U.kg, U.g]) == [None, 1.*U.kg, 2000.*U.g]
     assert eval_node(g,
-                     ts=[Decimal('274.15'), None, Decimal("273.15"), None],
+                     ts=[274.15, None, 273.15, None],
                      u=[U.K, None, None, None],
                      u1=[U.K, U.degC, U.degF, U.K]) == \
-    [Decimal('274.15')*U.K, 1.*U.degC, 32.*U.degF, Decimal("273.15")*U.K]
+    [274.15*U.K, 1.*U.degC, 32.*U.degF, 273.15*U.K]
```

### Comparing `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_units.py` & `hg_oap-0.1.2/tests/unit/hg_oap/utils/test_units.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from decimal import Decimal
 
 import pytest
 
 from hg_oap.units.unit import Unit
 from hg_oap.units.dimension import PrimaryDimension, DerivedDimension, Dimension
 from hg_oap.utils.exprclass import ExprClass
 from hg_oap.units.quantity import Quantity
@@ -56,55 +55,55 @@
 def test_unit_conversion_1():
     with UnitSystem() as U:
         U.length = PrimaryDimension()
         U.meter = PrimaryUnit(dimension=U.length)
 
         assert U.meter.convert(100., to=U.meter) == 100.
 
-        U.cm = DerivedUnit(primary_unit=U.meter, ratio=Decimal('0.01'))
+        U.cm = DerivedUnit(primary_unit=U.meter, ratio=0.01)
 
         assert U.cm.convert(100., to=U.meter) == 1.
-        assert U.cm.convert(Decimal(100), to=U.meter) == 1.
+        assert U.cm.convert(100.0, to=U.meter) == 1.
 
         assert U.meter.convert(100., to=U.cm) == 10000.
 
         U.meter_sq = U.meter**2
         U.cm_sq = U.cm**2
 
         assert U.meter_sq.convert(1., to=U.cm_sq) == 10000.
         assert U.cm_sq.convert(1., to=U.meter_sq) == 0.0001
 
         U.timespan = PrimaryDimension()
         U.second = PrimaryUnit(dimension=U.timespan)
-        U.minute = DerivedUnit(primary_unit=U.second, ratio=Decimal(60))
+        U.minute = DerivedUnit(primary_unit=U.second, ratio=60.0)
 
         U.velocity = U.length / U.timespan
 
         assert (U.meter/U.second).convert(1., to=U.cm / U.minute) == 6000.
         assert (U.cm/U.second).convert(1., to=U.meter / U.minute) == 60. / 100.
 
         with pytest.raises(ValueError):
             (U.meter/U.second).convert(1., to=U.meter_sq)
 
 
 def test_offset_units():
     with UnitSystem() as U:
         U.temperature = PrimaryDimension()
         U.kelvin = PrimaryUnit(dimension=U.temperature)
-        U.celsius = OffsetDerivedUnit(primary_unit=U.kelvin, ratio=Decimal('1'), offset=Decimal('273.15'))
+        U.celsius = OffsetDerivedUnit(primary_unit=U.kelvin, ratio=1.0, offset=273.15)
 
         assert U.celsius.convert(0., to=U.celsius) == 0.
         assert U.kelvin.convert(273.15, to=U.kelvin) == 273.15
 
         assert U.celsius.convert(0., to=U.kelvin) == 273.15
         assert U.kelvin.convert(273.15, to=U.celsius) == 0.
 
         assert U.celsius.convert(100., to=U.kelvin) == 373.15
 
-        U.fahrenheit = OffsetDerivedUnit(primary_unit=U.kelvin, ratio=Decimal('5')/Decimal('9'), offset=Decimal('459.67'))
+        U.fahrenheit = OffsetDerivedUnit(primary_unit=U.kelvin, ratio=5.0/9.0, offset=459.67)
 
         assert U.fahrenheit.convert(32., to=U.fahrenheit) == 32.
         assert round(U.fahrenheit.convert(32., to=U.celsius), 2) == 0.
         assert round(U.fahrenheit.convert(32., to=U.kelvin), 2) == 273.15
         assert round(U.celsius.convert(0., to=U.fahrenheit), 2) == 32.
         assert round(U.kelvin.convert(273.15, to=U.fahrenheit), 2) == 32.
 
@@ -137,69 +136,69 @@
 
 
 def test_qualified_units():
     with UnitSystem() as U:
         U.money = PrimaryDimension()
         U.us_dollars = U.money.us_dollars
         U.USD = PrimaryUnit(dimension=U.us_dollars)
-        U.USX = Decimal('0.01') * U.USD
+        U.USX = 0.01 * U.USD
 
         U.euros = U.money.euros
         U.EUR = PrimaryUnit(dimension=U.euros)
-        U.EUX = Decimal('0.01') * U.EUR
+        U.EUX = 0.01 * U.EUR
 
         U.bitcoins = U.money.bitcoins
         U.BTC = PrimaryUnit(dimension=U.bitcoins)
 
         assert U.USX.convert(100., to=U.USD) == 1.
         assert U.EUX.convert(100., to=U.EUR) == 1.
         assert (U.EUR/U.USD).name == 'EUR/USD'  # EUR/USD
 
-        with UnitConversionContext((Decimal(1.15) * (U.USD/U.EUR),)):
+        with UnitConversionContext((1.15 * (U.USD/U.EUR),)):
             assert U.EUR.convert(1., to=U.USD) == 1.15
 
 
 def test_contexts_and_conversion_factors():
     with UnitSystem() as U:
         U.length = PrimaryDimension()
         U.meter = PrimaryUnit(dimension=U.length)
 
         U.timespan = PrimaryDimension()
         U.second = PrimaryUnit(dimension=U.timespan)
-        U.minute = DerivedUnit(primary_unit=U.second, ratio=Decimal(60))
-        U.hour = DerivedUnit(primary_unit=U.minute, ratio=Decimal(60))
+        U.minute = DerivedUnit(primary_unit=U.second, ratio=60.)
+        U.hour = DerivedUnit(primary_unit=U.minute, ratio=60.)
 
         U.velocity = U.length / U.timespan
         U.meter_per_second = U.meter / U.second
 
-        my_speed = Decimal(2.) * U.meter_per_second
+        my_speed = 2. * U.meter_per_second
 
         with UnitConversionContext((my_speed,)):
             assert U.hour.convert(1., to=U.meter) == 7200.
 
 
 def test_contexts_and_conversion_factors_2():
     with UnitSystem() as U:
         U.currency = PrimaryDimension()
         U.currency_unit = PrimaryUnit(dimension=U.currency)
-        U.cent = DerivedUnit(primary_unit=U.currency_unit, ratio=Decimal('0.01'))
+        U.cent = DerivedUnit(primary_unit=U.currency_unit, ratio=0.01)
 
         U.length = PrimaryDimension()
         U.meter = PrimaryUnit(dimension=U.length)
 
         U.volume = U.length**3
         U.cubic_meter = U.meter**3
-        U.liter = Decimal('0.001') * U.cubic_meter
+        U.liter = 0.001 * U.cubic_meter
 
-        U.bushel = Decimal('35.2391') * U.liter
+        U.bushel = 35.2391 * U.liter
 
         U.weight = PrimaryDimension()
         U.kg = PrimaryUnit(dimension=U.weight)
-        U.mt = Decimal('1000') * U.kg
-        U.pound = Decimal('0.453592') * U.kg
+        U.mt = 1000. * U.kg
+        U.pound = 0.453592 * U.kg
 
         U.future_contract = PrimaryDimension()
         U.lot = PrimaryUnit(dimension=U.future_contract)
 
         @dataclass
         class MyAsset:
             name: str
@@ -207,26 +206,26 @@
 
         @dataclass
         class MyInstrument(CompoundScalar, ExprClass, UnitConversionContext):
             asset: MyAsset
             lot_size: int
             unit: Unit
             price_unit: Unit
-            price_tick_size: Decimal
+            price_tick_size: float
             price_currency: str
 
             unit_conversion_factors: tuple[Quantity] = \
                 lambda self: (
-                    Quantity(Decimal(self.lot_size), self.unit / U.lot),
+                    Quantity(self.lot_size, self.unit / U.lot),
                     self.asset.density,
                 )
 
 
-        asset = MyAsset('corn', Quantity(Decimal('0.75'), U.kg / U.liter))
-        instrument = MyInstrument(asset, 10000, U.bushel, U.cent, Decimal('0.25'), 'USD')
+        asset = MyAsset('corn', Quantity(0.75, U.kg / U.liter))
+        instrument = MyInstrument(asset, 10000, U.bushel, U.cent, 0.25, 'USD')
 
         with instrument:
             assert U.lot.convert(1., to=U.bushel) == 10000.
             assert U.lot.convert(1., to=U.cubic_meter) == 352.391
             assert U.lot.convert(1., to=U.mt) == 264.29325
 
             assert round(U.mt.convert(1., to=U.lot), 5) == 0.00378
```

### Comparing `hg_oap-0.1.1/.gitignore` & `hg_oap-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/LICENSE` & `hg_oap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/README.md` & `hg_oap-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.1/pyproject.toml` & `hg_oap-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hg_oap"
 dynamic = ["version"]
 dependencies = [
-    "hgraph>=0.2.17",
+    "hgraph>=0.2.27",
     "holidays>=0.46",
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "Howard Henson", email = "howard@henson.me.uk" },
 ]
 maintainers = [
```

### Comparing `hg_oap-0.1.1/PKG-INFO` & `hg_oap-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hg_oap
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to faciliate building order and pricing strategies
 Project-URL: Homepage, https://github.com/hhenson/hg_oap
 Project-URL: Repository, https://github.com/hhenson/hg_oap.git
 Author-email: Howard Henson <howard@henson.me.uk>
 License: MIT License
         
         Copyright (c) 2024 Howard Henson
@@ -29,15 +29,15 @@
 License-File: LICENSE
 Keywords: forward propogating graph,fpg,functional reactive programming,graph,oms,order,pricing,reactive,time series
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
-Requires-Dist: hgraph>=0.2.17
+Requires-Dist: hgraph>=0.2.27
 Requires-Dist: holidays>=0.46
 Description-Content-Type: text/markdown
 
 # HGraph Orders and Pricing Library
 
 Provides a library, based on the hgraph functional reactive framework to
 support creating order and pricing logic.
```

