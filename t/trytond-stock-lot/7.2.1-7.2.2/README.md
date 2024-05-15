# Comparing `tmp/trytond_stock_lot-7.2.1.tar.gz` & `tmp/trytond_stock_lot-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock_lot-7.2.1.tar", last modified: Wed May  1 10:04:39 2024, max compression
+gzip compressed data, was "trytond_stock_lot-7.2.2.tar", last modified: Wed May 15 17:00:00 2024, max compression
```

## Comparing `trytond_stock_lot-7.2.1.tar` & `trytond_stock_lot-7.2.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.718521 trytond_stock_lot-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     3281 2024-05-01 10:04:36.000000 trytond_stock_lot-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-01 10:04:36.000000 trytond_stock_lot-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-01 10:04:39.718521 trytond_stock_lot-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.711855 trytond_stock_lot-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      849 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.715188 trytond_stock_lot-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    11800 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12336 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10542 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12685 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12391 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10244 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10911 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12709 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12453 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11312 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10317 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10765 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11352 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10596 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12424 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10768 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11627 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10139 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11687 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11462 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10007 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11899 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1014 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4666 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 10:04:39.718521 trytond_stock_lot-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4423 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31049 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20380 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.715188 trytond_stock_lot-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_assign_try.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_move_add.json
--rw-r--r--   0 ced       (1000) ced       (1000)     2741 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_move_add.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2548 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4550 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_out_internal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2200 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/scenario_stock_lot_trace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12516 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:06.000000 trytond_stock_lot-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.718521 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2997 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 10:04:39.718521 trytond_stock_lot-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lot_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lot_by_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lot_trace_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lot_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/lots_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/period_cache_lot_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      332 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/period_cache_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      718 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/stock_move_add_lots_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/stock_move_add_lots_start_lot_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.1/view/template_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.717192 trytond_stock_lot-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3382 2024-05-15 16:59:56.000000 trytond_stock_lot-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-05-15 16:59:56.000000 trytond_stock_lot-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-15 17:00:00.717192 trytond_stock_lot-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.710525 trytond_stock_lot-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3072 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      849 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.713858 trytond_stock_lot-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11800 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12336 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10542 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12685 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12391 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10244 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10911 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12709 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12453 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11312 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10317 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10765 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11352 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10596 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12424 2024-04-30 17:21:59.000000 trytond_stock_lot-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10768 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11627 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10139 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11687 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11462 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10533 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10007 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11899 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1014 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4778 2024-05-11 10:34:43.000000 trytond_stock_lot-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      772 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 17:00:00.717192 trytond_stock_lot-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4423 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31049 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20380 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.713858 trytond_stock_lot-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3461 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_assign_try.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_move_add.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     2741 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_move_add.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1610 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2548 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4550 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3964 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_out_internal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2200 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/scenario_stock_lot_trace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12516 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-05-01 10:04:46.000000 trytond_stock_lot-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.717192 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2808 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2997 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 10:04:39.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      135 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 17:00:00.000000 trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:00:00.717192 trytond_stock_lot-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lot_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lot_by_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lot_trace_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lot_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/lots_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/period_cache_lot_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      332 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/period_cache_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      718 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/stock_move_add_lots_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/stock_move_add_lots_start_lot_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2024-04-30 17:21:00.000000 trytond_stock_lot-7.2.2/view/template_form.xml
```

### Comparing `trytond_stock_lot-7.2.1/CHANGELOG` & `trytond_stock_lot-7.2.2/CHANGELOG`

 * *Files 7% similar despite different names*

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

### Comparing `trytond_stock_lot-7.2.1/COPYRIGHT` & `trytond_stock_lot-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/LICENSE` & `trytond_stock_lot-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/PKG-INFO` & `trytond_stock_lot-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for lot of products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_lot-7.2.1/__init__.py` & `trytond_stock_lot-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/doc/conf.py` & `trytond_stock_lot-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/ir.xml` & `trytond_stock_lot-7.2.2/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/bg.po` & `trytond_stock_lot-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/ca.po` & `trytond_stock_lot-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/cs.po` & `trytond_stock_lot-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/de.po` & `trytond_stock_lot-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/es.po` & `trytond_stock_lot-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/es_419.po` & `trytond_stock_lot-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/et.po` & `trytond_stock_lot-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/fa.po` & `trytond_stock_lot-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/fi.po` & `trytond_stock_lot-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/fr.po` & `trytond_stock_lot-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/hu.po` & `trytond_stock_lot-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/id.po` & `trytond_stock_lot-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/it.po` & `trytond_stock_lot-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/lo.po` & `trytond_stock_lot-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/lt.po` & `trytond_stock_lot-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/nl.po` & `trytond_stock_lot-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/pl.po` & `trytond_stock_lot-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/pt.po` & `trytond_stock_lot-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/ro.po` & `trytond_stock_lot-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/ru.po` & `trytond_stock_lot-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/sl.po` & `trytond_stock_lot-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/tr.po` & `trytond_stock_lot-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/uk.po` & `trytond_stock_lot-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/locale/zh_CN.po` & `trytond_stock_lot-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/message.xml` & `trytond_stock_lot-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/product.py` & `trytond_stock_lot-7.2.2/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 
     default_lot_sequence = fields.MultiValue(
         fields.Many2One(
             'ir.sequence', "Default Lot Sequence",
             domain=[
                 ('sequence_type', '=',
                     Id('stock_lot', 'sequence_type_stock_lot')),
+                ('company', '=', None),
                 ]))
 
 
 class ConfigurationDefaultLotSequence(ModelSQL, ValueMixin):
     "Product Configuration Default Lot Sequence"
     __name__ = 'product.configuration.default_lot_sequence'
     default_lot_sequence = fields.Many2One(
         'ir.sequence', "Default Lot Sequence",
         domain=[
             ('sequence_type', '=',
                 Id('stock_lot', 'sequence_type_stock_lot')),
+            ('company', '=', None),
             ])
 
 
 class Template(metaclass=PoolMeta):
     __name__ = 'product.template'
 
     lot_required = fields.MultiSelection([
@@ -46,14 +48,15 @@
         states={
             'invisible': ~Eval('type').in_(['goods', 'assets']),
             })
     lot_sequence = fields.Many2One(
         'ir.sequence', "Lot Sequence",
         domain=[
             ('sequence_type', '=', Id('stock_lot', 'sequence_type_stock_lot')),
+            ('company', '=', None),
             ],
         states={
             'invisible': ~Eval('type').in_(['goods', 'assets']),
             },
         help="The sequence used to automatically number lots.")
 
     @classmethod
```

### Comparing `trytond_stock_lot-7.2.1/product.xml` & `trytond_stock_lot-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/setup.py` & `trytond_stock_lot-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/stock.py` & `trytond_stock_lot-7.2.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/stock.xml` & `trytond_stock_lot-7.2.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_assign_try.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_assign_try.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_move_add.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_move_add.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_number.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_number.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_in.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_in.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_out.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_out.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_shipment_out_internal.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_shipment_out_internal.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/scenario_stock_lot_trace.rst` & `trytond_stock_lot-7.2.2/tests/scenario_stock_lot_trace.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tests/test_module.py` & `trytond_stock_lot-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/tox.ini` & `trytond_stock_lot-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/PKG-INFO` & `trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_stock_lot
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for lot of products
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_stock_lot-7.2.1/trytond_stock_lot.egg-info/SOURCES.txt` & `trytond_stock_lot-7.2.2/trytond_stock_lot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/view/lot_by_warehouse_context_form.xml` & `trytond_stock_lot-7.2.2/view/lot_by_warehouse_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/view/lot_form.xml` & `trytond_stock_lot-7.2.2/view/lot_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock_lot-7.2.1/view/stock_move_add_lots_start_form.xml` & `trytond_stock_lot-7.2.2/view/stock_move_add_lots_start_form.xml`

 * *Files identical despite different names*

