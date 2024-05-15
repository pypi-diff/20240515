# Comparing `tmp/trytond_purchase_request_quotation-7.2.1.tar.gz` & `tmp/trytond_purchase_request_quotation-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request_quotation-7.2.1.tar", last modified: Wed May  1 11:34:48 2024, max compression
+gzip compressed data, was "trytond_purchase_request_quotation-7.2.2.tar", last modified: Wed May 15 17:03:15 2024, max compression
```

## Comparing `trytond_purchase_request_quotation-7.2.1.tar` & `trytond_purchase_request_quotation-7.2.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.335472 trytond_purchase_request_quotation-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1512 2024-05-01 11:34:45.000000 trytond_purchase_request_quotation-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2024-05-01 11:34:44.000000 trytond_purchase_request_quotation-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-05-01 11:34:48.335472 trytond_purchase_request_quotation-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.328806 trytond_purchase_request_quotation-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.332139 trytond_purchase_request_quotation-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10041 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9941 2024-04-30 17:21:59.000000 trytond_purchase_request_quotation-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10057 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8380 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9454 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10663 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9878 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8625 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9186 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8876 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9807 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8416 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8364 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23676 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10879 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2096 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    65135 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/quotation.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:34:48.335472 trytond_purchase_request_quotation-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4539 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.332139 trytond_purchase_request_quotation-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7770 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/tests/scenario_purchase_request_quotation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      488 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-30 17:21:06.000000 trytond_purchase_request_quotation-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.335472 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2499 2024-05-01 11:34:48.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:34:48.335472 trytond_purchase_request_quotation-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_create_ask_suppliers_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_create_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1456 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      980 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_line_list_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.248771 trytond_purchase_request_quotation-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1613 2024-05-15 17:03:12.000000 trytond_purchase_request_quotation-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2024-05-15 17:03:11.000000 trytond_purchase_request_quotation-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-05-15 17:03:15.248771 trytond_purchase_request_quotation-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.242104 trytond_purchase_request_quotation-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      237 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.245437 trytond_purchase_request_quotation-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10041 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9941 2024-04-30 17:21:59.000000 trytond_purchase_request_quotation-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10057 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8380 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9454 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10663 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9878 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8625 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9186 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8876 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9807 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8416 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8364 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8824 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23621 2024-05-11 10:30:08.000000 trytond_purchase_request_quotation-7.2.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10879 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2096 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    65135 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/quotation.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 17:03:15.248771 trytond_purchase_request_quotation-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4539 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.245437 trytond_purchase_request_quotation-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7770 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/tests/scenario_purchase_request_quotation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      488 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-05-01 11:34:54.000000 trytond_purchase_request_quotation-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.248771 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3838 2024-05-15 17:03:14.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2499 2024-05-15 17:03:15.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 17:03:14.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-15 17:03:14.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:34:47.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-05-15 17:03:14.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 17:03:14.000000 trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:03:15.248771 trytond_purchase_request_quotation-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_create_ask_suppliers_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_create_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1456 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      980 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      452 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_line_list_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_list.xml
```

### Comparing `trytond_purchase_request_quotation-7.2.1/CHANGELOG` & `trytond_purchase_request_quotation-7.2.2/CHANGELOG`

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

### Comparing `trytond_purchase_request_quotation-7.2.1/COPYRIGHT` & `trytond_purchase_request_quotation-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/LICENSE` & `trytond_purchase_request_quotation-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/PKG-INFO` & `trytond_purchase_request_quotation-7.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request_quotation
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase request quotation
 Home-page: http://www.tryton.org
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request_quotation-7.2.1/README.rst` & `trytond_purchase_request_quotation-7.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/__init__.py` & `trytond_purchase_request_quotation-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/doc/conf.py` & `trytond_purchase_request_quotation-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/doc/index.rst` & `trytond_purchase_request_quotation-7.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/bg.po` & `trytond_purchase_request_quotation-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/ca.po` & `trytond_purchase_request_quotation-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/cs.po` & `trytond_purchase_request_quotation-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/de.po` & `trytond_purchase_request_quotation-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/es.po` & `trytond_purchase_request_quotation-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/es_419.po` & `trytond_purchase_request_quotation-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/et.po` & `trytond_purchase_request_quotation-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/fa.po` & `trytond_purchase_request_quotation-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/fi.po` & `trytond_purchase_request_quotation-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/fr.po` & `trytond_purchase_request_quotation-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/hu.po` & `trytond_purchase_request_quotation-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/id.po` & `trytond_purchase_request_quotation-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/it.po` & `trytond_purchase_request_quotation-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/lo.po` & `trytond_purchase_request_quotation-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/lt.po` & `trytond_purchase_request_quotation-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/nl.po` & `trytond_purchase_request_quotation-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/pl.po` & `trytond_purchase_request_quotation-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/pt.po` & `trytond_purchase_request_quotation-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/ro.po` & `trytond_purchase_request_quotation-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/ru.po` & `trytond_purchase_request_quotation-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/sl.po` & `trytond_purchase_request_quotation-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/tr.po` & `trytond_purchase_request_quotation-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/uk.po` & `trytond_purchase_request_quotation-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/locale/zh_CN.po` & `trytond_purchase_request_quotation-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/purchase.py` & `trytond_purchase_request_quotation-7.2.2/purchase.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,14 @@
     def copy(cls, groups, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
         default.setdefault('number', None)
         default.setdefault('revision', cls.default_revision())
-        default.setdefault('request_quotations', None)
         return super(Quotation, cls).copy(groups, default=default)
 
     @property
     def delivery_full_address(self):
         if self.warehouse and self.warehouse.address:
             return self.warehouse.address.full_address
         return ''
```

### Comparing `trytond_purchase_request_quotation-7.2.1/purchase.xml` & `trytond_purchase_request_quotation-7.2.2/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/purchase_request.xml` & `trytond_purchase_request_quotation-7.2.2/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/quotation.fodt` & `trytond_purchase_request_quotation-7.2.2/quotation.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/setup.py` & `trytond_purchase_request_quotation-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/tests/scenario_purchase_request_quotation.rst` & `trytond_purchase_request_quotation-7.2.2/tests/scenario_purchase_request_quotation.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/tox.ini` & `trytond_purchase_request_quotation-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/PKG-INFO` & `trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request_quotation
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase request quotation
 Home-page: http://www.tryton.org
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request_quotation-7.2.1/trytond_purchase_request_quotation.egg-info/SOURCES.txt` & `trytond_purchase_request_quotation-7.2.2/trytond_purchase_request_quotation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/view/purchase_request_form.xml` & `trytond_purchase_request_quotation-7.2.2/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_form.xml` & `trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request_quotation-7.2.1/view/purchase_request_quotation_line_form.xml` & `trytond_purchase_request_quotation-7.2.2/view/purchase_request_quotation_line_form.xml`

 * *Files identical despite different names*

