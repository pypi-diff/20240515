# Comparing `tmp/trytond_production-7.2.1.tar.gz` & `tmp/trytond_production-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production-7.2.1.tar", last modified: Wed May  1 11:52:43 2024, max compression
+gzip compressed data, was "trytond_production-7.2.2.tar", last modified: Wed May 15 17:09:00 2024, max compression
```

## Comparing `trytond_production-7.2.1.tar` & `trytond_production-7.2.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.790678 trytond_production-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-05-01 11:52:40.000000 trytond_production-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 11:52:40.000000 trytond_production-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_production-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_production-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-01 11:52:43.790678 trytond_production-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond_production-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9434 2024-04-30 17:20:59.000000 trytond_production-7.2.1/bom.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6250 2024-04-30 17:21:00.000000 trytond_production-7.2.1/bom.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1826 2024-04-30 17:21:00.000000 trytond_production-7.2.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond_production-7.2.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.780678 trytond_production-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond_production-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3141 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_production-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_production-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-30 17:21:00.000000 trytond_production-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.780678 trytond_production-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_production-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:21:00.000000 trytond_production-7.2.1/icons/tryton-production.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      951 2024-04-30 17:21:00.000000 trytond_production-7.2.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.784011 trytond_production-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14469 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14254 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12571 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14121 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11753 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13125 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14267 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12558 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14177 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13234 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12183 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13781 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14185 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12631 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14004 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13174 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13709 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13934 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14626 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13454 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11736 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12626 2024-04-30 17:21:59.000000 trytond_production-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      811 2024-04-30 17:21:00.000000 trytond_production-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4297 2024-04-30 17:20:59.000000 trytond_production-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4152 2024-04-30 17:21:00.000000 trytond_production-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32160 2024-04-30 17:20:59.000000 trytond_production-7.2.1/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12522 2024-04-30 17:21:00.000000 trytond_production-7.2.1/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:52:43.790678 trytond_production-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-04-30 17:21:00.000000 trytond_production-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6212 2024-04-30 17:21:00.000000 trytond_production-7.2.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-30 17:21:00.000000 trytond_production-7.2.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7298 2024-04-30 17:20:59.000000 trytond_production-7.2.1/tests/scenario_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2722 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_by_product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-04-30 17:20:59.000000 trytond_production-7.2.1/tests/scenario_production_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2908 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_lot_trace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_no_list_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2454 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_rounding.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3137 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_set_cost.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/scenario_production_waste.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_production-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-04-30 17:21:06.000000 trytond_production-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/trytond_production.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:52:43.000000 trytond_production-7.2.1/trytond_production.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:52:43.787345 trytond_production-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_input_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_input_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_output_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_output_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_open_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_open_tree_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/bom_tree_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      605 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_bom_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_calendar.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_lead_time_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/production_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/stock_move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      309 2024-04-30 17:21:00.000000 trytond_production-7.2.1/view/template_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.633071 trytond_production-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4371 2024-05-15 17:08:57.000000 trytond_production-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-15 17:08:57.000000 trytond_production-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_production-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_production-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-15 17:09:00.633071 trytond_production-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond_production-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9434 2024-04-30 17:20:59.000000 trytond_production-7.2.2/bom.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6250 2024-04-30 17:21:00.000000 trytond_production-7.2.2/bom.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1826 2024-04-30 17:21:00.000000 trytond_production-7.2.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond_production-7.2.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.626404 trytond_production-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond_production-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3141 2024-04-30 17:20:59.000000 trytond_production-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:20:59.000000 trytond_production-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_production-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_production-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-30 17:21:00.000000 trytond_production-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.626404 trytond_production-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_production-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:21:00.000000 trytond_production-7.2.2/icons/tryton-production.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      951 2024-04-30 17:21:00.000000 trytond_production-7.2.2/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.629737 trytond_production-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14469 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14254 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12571 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14237 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14121 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11753 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13125 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14267 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12558 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14177 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13234 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12183 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13781 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14185 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12631 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14004 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13174 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13709 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13934 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14626 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13454 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11736 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12626 2024-04-30 17:21:59.000000 trytond_production-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      811 2024-04-30 17:21:00.000000 trytond_production-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4297 2024-04-30 17:20:59.000000 trytond_production-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4152 2024-04-30 17:21:00.000000 trytond_production-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32160 2024-04-30 17:20:59.000000 trytond_production-7.2.2/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12522 2024-04-30 17:21:00.000000 trytond_production-7.2.2/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 17:09:00.633071 trytond_production-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4602 2024-04-30 17:21:00.000000 trytond_production-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6212 2024-04-30 17:21:00.000000 trytond_production-7.2.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1917 2024-04-30 17:21:00.000000 trytond_production-7.2.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.629737 trytond_production-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7298 2024-04-30 17:20:59.000000 trytond_production-7.2.2/tests/scenario_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2722 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_by_product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-05-14 15:42:58.000000 trytond_production-7.2.2/tests/scenario_production_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2908 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_lot_trace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2156 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_no_list_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_rounding.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3137 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_set_cost.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2923 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/scenario_production_waste.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_production-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      214 2024-05-01 11:52:50.000000 trytond_production-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.633071 trytond_production-7.2.2/trytond_production.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2836 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:52:43.000000 trytond_production-7.2.2/trytond_production.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 17:09:00.000000 trytond_production-7.2.2/trytond_production.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:09:00.633071 trytond_production-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_input_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_input_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_output_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_output_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_tree_open_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      215 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_tree_open_tree_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/bom_tree_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      266 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      605 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      394 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/product_bom_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/product_bom_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/product_bom_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_calendar.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_lead_time_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/production_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/stock_move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      309 2024-04-30 17:21:00.000000 trytond_production-7.2.2/view/template_list.xml
```

### Comparing `trytond_production-7.2.1/CHANGELOG` & `trytond_production-7.2.2/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.2 - 2024-05-15
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.1 - 2024-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.2.0 - 2024-04-29
 --------------------------
```

### Comparing `trytond_production-7.2.1/COPYRIGHT` & `trytond_production-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/LICENSE` & `trytond_production-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/PKG-INFO` & `trytond_production-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production-7.2.1/__init__.py` & `trytond_production-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/bom.py` & `trytond_production-7.2.2/bom.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/bom.xml` & `trytond_production-7.2.2/bom.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/configuration.py` & `trytond_production-7.2.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/configuration.xml` & `trytond_production-7.2.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/doc/conf.py` & `trytond_production-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/doc/design.rst` & `trytond_production-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/icons/LICENSE` & `trytond_production-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/ir.py` & `trytond_production-7.2.2/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/bg.po` & `trytond_production-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/ca.po` & `trytond_production-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/cs.po` & `trytond_production-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/de.po` & `trytond_production-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/es.po` & `trytond_production-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/es_419.po` & `trytond_production-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/et.po` & `trytond_production-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/fa.po` & `trytond_production-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/fi.po` & `trytond_production-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/fr.po` & `trytond_production-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/hu.po` & `trytond_production-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/id.po` & `trytond_production-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/it.po` & `trytond_production-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/lo.po` & `trytond_production-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/lt.po` & `trytond_production-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/nl.po` & `trytond_production-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/pl.po` & `trytond_production-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/pt.po` & `trytond_production-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/ro.po` & `trytond_production-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/ru.po` & `trytond_production-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/sl.po` & `trytond_production-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/tr.po` & `trytond_production-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/uk.po` & `trytond_production-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/locale/zh_CN.po` & `trytond_production-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/message.xml` & `trytond_production-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/product.py` & `trytond_production-7.2.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/product.xml` & `trytond_production-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/production.py` & `trytond_production-7.2.2/production.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/production.xml` & `trytond_production-7.2.2/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/setup.py` & `trytond_production-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/stock.py` & `trytond_production-7.2.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/stock.xml` & `trytond_production-7.2.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production.rst` & `trytond_production-7.2.2/tests/scenario_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_by_product.rst` & `trytond_production-7.2.2/tests/scenario_production_by_product.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_lot_number.rst` & `trytond_production-7.2.2/tests/scenario_production_lot_number.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> _ = create_company()
     >>> company = get_company()
 
 Create lot sequence::
 
     >>> sequence_type, = SequenceType.find(
     ...     [('name', '=', "Stock Lot")], limit=1)
-    >>> sequence = Sequence(name="Lot", sequence_type=sequence_type)
+    >>> sequence = Sequence(name="Lot", sequence_type=sequence_type, company=None)
     >>> sequence.save()
 
 Create product::
 
     >>> unit, = UoM.find([('name', '=', 'Unit')])
 
     >>> template = ProductTemplate()
```

### Comparing `trytond_production-7.2.1/tests/scenario_production_lot_trace.rst` & `trytond_production-7.2.2/tests/scenario_production_lot_trace.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_no_list_price.rst` & `trytond_production-7.2.2/tests/scenario_production_no_list_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_rounding.rst` & `trytond_production-7.2.2/tests/scenario_production_rounding.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_set_cost.rst` & `trytond_production-7.2.2/tests/scenario_production_set_cost.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/scenario_production_waste.rst` & `trytond_production-7.2.2/tests/scenario_production_waste.rst`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tests/test_module.py` & `trytond_production-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/tox.ini` & `trytond_production-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/trytond_production.egg-info/PKG-INFO` & `trytond_production-7.2.2/trytond_production.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production-7.2.1/trytond_production.egg-info/SOURCES.txt` & `trytond_production-7.2.2/trytond_production.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/view/location_form.xml` & `trytond_production-7.2.2/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/view/production_form.xml` & `trytond_production-7.2.2/view/production_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/view/production_list.xml` & `trytond_production-7.2.2/view/production_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_production-7.2.1/view/template_form.xml` & `trytond_production-7.2.2/view/template_form.xml`

 * *Files identical despite different names*

