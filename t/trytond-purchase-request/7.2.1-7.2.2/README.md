# Comparing `tmp/trytond_purchase_request-7.2.1.tar.gz` & `tmp/trytond_purchase_request-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_request-7.2.1.tar", last modified: Wed May  1 11:35:57 2024, max compression
+gzip compressed data, was "trytond_purchase_request-7.2.2.tar", last modified: Wed May 15 17:07:53 2024, max compression
```

## Comparing `trytond_purchase_request-7.2.1.tar` & `trytond_purchase_request-7.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.163672 trytond_purchase_request-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     2330 2024-05-01 11:35:53.000000 trytond_purchase_request-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-05-01 11:35:53.000000 trytond_purchase_request-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.157006 trytond_purchase_request-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6930 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7361 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7439 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7326 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6246 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6482 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7341 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6883 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7286 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6898 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6236 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6479 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7029 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7393 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7053 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6954 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      400 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3855 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1086 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    19606 2024-04-30 17:21:06.000000 trytond_purchase_request-7.2.1/purchase_request.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9229 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/purchase_request.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:35:57.163672 trytond_purchase_request-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8378 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/scenario_purchase_request.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-04-30 17:21:06.000000 trytond_purchase_request-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-05-01 11:35:57.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:35:57.160339 trytond_purchase_request-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/handle_purchase_cancellation_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_create_purchase_ask_party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.1/view/purchase_request_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.801485 trytond_purchase_request-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2432 2024-05-15 17:07:50.000000 trytond_purchase_request-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-05-15 17:07:50.000000 trytond_purchase_request-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-15 17:07:53.801485 trytond_purchase_request-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.798152 trytond_purchase_request-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      244 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.798152 trytond_purchase_request-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6930 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7361 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7439 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7326 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6246 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6482 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7783 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7341 2024-04-30 17:21:59.000000 trytond_purchase_request-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6883 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6225 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7286 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6898 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6236 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7289 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6479 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7029 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7393 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7053 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6951 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6200 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5929 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6954 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3855 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1086 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    19606 2024-04-30 17:21:06.000000 trytond_purchase_request-7.2.2/purchase_request.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9229 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/purchase_request.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 17:07:53.801485 trytond_purchase_request-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4454 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.798152 trytond_purchase_request-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8378 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/tests/scenario_purchase_request.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      127 2024-05-01 11:36:03.000000 trytond_purchase_request-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.801485 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3673 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2013 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:35:56.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 17:07:53.000000 trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:07:53.801485 trytond_purchase_request-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/view/handle_purchase_cancellation_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/view/purchase_request_create_purchase_ask_party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1817 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/view/purchase_request_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      602 2024-04-30 17:21:00.000000 trytond_purchase_request-7.2.2/view/purchase_request_tree.xml
```

### Comparing `trytond_purchase_request-7.2.1/CHANGELOG` & `trytond_purchase_request-7.2.2/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 
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
 * Bug fixes (see mercurial logs for details)
-
-Open purchases created from requests
+* Open purchases created from requests
 
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 * Rename UOM to Unit for purchase request
```

### Comparing `trytond_purchase_request-7.2.1/COPYRIGHT` & `trytond_purchase_request-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/LICENSE` & `trytond_purchase_request-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/PKG-INFO` & `trytond_purchase_request-7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request-7.2.1/README.rst` & `trytond_purchase_request-7.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/__init__.py` & `trytond_purchase_request-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/doc/conf.py` & `trytond_purchase_request-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/doc/index.rst` & `trytond_purchase_request-7.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/bg.po` & `trytond_purchase_request-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/ca.po` & `trytond_purchase_request-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/cs.po` & `trytond_purchase_request-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/de.po` & `trytond_purchase_request-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/es.po` & `trytond_purchase_request-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/es_419.po` & `trytond_purchase_request-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/et.po` & `trytond_purchase_request-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/fa.po` & `trytond_purchase_request-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/fi.po` & `trytond_purchase_request-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/fr.po` & `trytond_purchase_request-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/hu.po` & `trytond_purchase_request-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/id.po` & `trytond_purchase_request-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/it.po` & `trytond_purchase_request-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/lo.po` & `trytond_purchase_request-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/lt.po` & `trytond_purchase_request-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/nl.po` & `trytond_purchase_request-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/pl.po` & `trytond_purchase_request-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/pt.po` & `trytond_purchase_request-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/ro.po` & `trytond_purchase_request-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/ru.po` & `trytond_purchase_request-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/sl.po` & `trytond_purchase_request-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/tr.po` & `trytond_purchase_request-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/uk.po` & `trytond_purchase_request-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/locale/zh_CN.po` & `trytond_purchase_request-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/message.xml` & `trytond_purchase_request-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/purchase.py` & `trytond_purchase_request-7.2.2/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/purchase.xml` & `trytond_purchase_request-7.2.2/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/purchase_request.py` & `trytond_purchase_request-7.2.2/purchase_request.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/purchase_request.xml` & `trytond_purchase_request-7.2.2/purchase_request.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/setup.py` & `trytond_purchase_request-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/tests/scenario_purchase_request.rst` & `trytond_purchase_request-7.2.2/tests/scenario_purchase_request.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/tox.ini` & `trytond_purchase_request-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/PKG-INFO` & `trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_request
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase requests
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_request-7.2.1/trytond_purchase_request.egg-info/SOURCES.txt` & `trytond_purchase_request-7.2.2/trytond_purchase_request.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/view/purchase_request_form.xml` & `trytond_purchase_request-7.2.2/view/purchase_request_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_request-7.2.1/view/purchase_request_tree.xml` & `trytond_purchase_request-7.2.2/view/purchase_request_tree.xml`

 * *Files identical despite different names*

