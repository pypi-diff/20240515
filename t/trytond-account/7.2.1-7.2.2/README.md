# Comparing `tmp/trytond_account-7.2.1.tar.gz` & `tmp/trytond_account-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account-7.2.1.tar", last modified: Wed May  1 12:38:35 2024, max compression
+gzip compressed data, was "trytond_account-7.2.2.tar", last modified: Wed May 15 17:11:58 2024, max compression
```

## Comparing `trytond_account-7.2.1.tar` & `trytond_account-7.2.2.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)    10838 2024-05-01 12:38:32.000000 trytond_account-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:38:32.000000 trytond_account-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-01 12:38:35.875851 trytond_account-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:20:59.000000 trytond_account-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)   129467 2024-04-30 17:20:59.000000 trytond_account-7.2.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)    46672 2024-04-30 17:20:59.000000 trytond_account-7.2.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    51736 2024-04-30 17:20:59.000000 trytond_account-7.2.1/aged_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.1/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6045 2024-04-30 17:20:59.000000 trytond_account-7.2.1/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3024 2024-04-30 17:20:59.000000 trytond_account-7.2.1/company.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8831 2024-04-30 17:20:59.000000 trytond_account-7.2.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-30 17:20:59.000000 trytond_account-7.2.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      957 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/configuration.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/account.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/configuration.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/fiscal-year.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2246 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/journal.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/move.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/tax.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/design/template.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1558 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/close.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/create.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/report.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/structure.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-30 17:20:59.000000 trytond_account-7.2.1/doc/usage/view.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-30 17:20:59.000000 trytond_account-7.2.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26581 2024-04-30 17:20:59.000000 trytond_account-7.2.1/fiscalyear.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7424 2024-04-30 17:20:59.000000 trytond_account-7.2.1/fiscalyear.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    52160 2024-04-30 17:20:59.000000 trytond_account-7.2.1/general_journal.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    81559 2024-04-30 17:20:59.000000 trytond_account-7.2.1/general_ledger.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.859184 trytond_account-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-block.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-30 17:20:59.000000 trytond_account-7.2.1/icons/tryton-account.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    13491 2024-04-30 17:20:59.000000 trytond_account-7.2.1/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12289 2024-04-30 17:20:59.000000 trytond_account-7.2.1/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.862517 trytond_account-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   131048 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130583 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114241 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   134193 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   130891 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118935 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)   127139 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   138558 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)   118048 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   132823 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125558 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)   117226 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122882 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)   143189 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)   134790 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   131232 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   122265 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   125426 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   129848 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   133001 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)   123107 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   114073 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   148010 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   126059 2024-04-30 17:21:59.000000 trytond_account-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1494 2024-04-30 17:20:59.000000 trytond_account-7.2.1/localize.xsl
--rw-r--r--   0 ced       (1000) ced       (1000)    17448 2024-04-30 17:21:06.000000 trytond_account-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22110 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11303 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11058 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11004 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11069 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11050 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11083 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11090 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11405 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11056 2024-04-30 17:20:59.000000 trytond_account-7.2.1/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   116642 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26295 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    15750 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move_template.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6717 2024-04-30 17:20:59.000000 trytond_account-7.2.1/move_template.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13726 2024-04-30 17:20:59.000000 trytond_account-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4156 2024-04-30 17:20:59.000000 trytond_account-7.2.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16319 2024-04-30 17:20:59.000000 trytond_account-7.2.1/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4083 2024-04-30 17:20:59.000000 trytond_account-7.2.1/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:38:35.875851 trytond_account-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-04-30 17:20:59.000000 trytond_account-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    70885 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24263 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tax.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.865851 trytond_account-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4618 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_active.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3995 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconcile_automatic.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.json
--rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.json
--rw-r--r--   0 ced       (1000) ced       (1000)     4420 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4736 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_close_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_cancel.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_delegate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5021 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_group.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4907 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_line_reschedule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4796 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_move_template.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    10860 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_reports.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/scenario_tax_code.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    80138 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4788 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)    47972 2024-04-30 17:20:59.000000 trytond_account-7.2.1/trial_balance.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:06.000000 trytond_account-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/trytond_account.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    12499 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:38:35.000000 trytond_account-7.2.1/trytond_account.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    54595 2024-04-30 17:20:59.000000 trytond_account-7.2.1/type_statement.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:38:35.875851 trytond_account-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_balance_sheet_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_deferral_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_deferral_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_income_statement_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_list_balance_sheet.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1074 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1283 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1103 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/account_type_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/aged_balance_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/aged_balance_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/balance_sheet_context_comparison_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/balance_sheet_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/company_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1353 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_account_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_properties_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/create_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_balance_non_deferral_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_create_periods_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      910 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/fiscalyear_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_account_party_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_line_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/general_ledger_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1138 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/income_statement_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_list_cash.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_list_matching_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_open_cash_context.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_cancel_default_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_delegate_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1753 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1241 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_form_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_group_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_list_payable_receivable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_list_reconcile.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_receivable_payable_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_preview_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_reschedule_term_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1026 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      636 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_line_tree_move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_reconciliation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_reconciliation_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_create_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      857 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_keyword_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/open_journal_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1161 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_list_close.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/period_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_lines_writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      755 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_show_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/reconcile_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/renew_fiscalyear_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1122 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      843 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_code_tree_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2193 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_group_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      516 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      655 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_template_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_rule_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2101 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/tax_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      250 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/update_chart_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/update_chart_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/writeoff_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account-7.2.1/view/writeoff_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.335090 trytond_account-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10939 2024-05-15 17:11:54.000000 trytond_account-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-15 17:11:54.000000 trytond_account-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-15 17:11:58.335090 trytond_account-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:20:59.000000 trytond_account-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   129467 2024-04-30 17:20:59.000000 trytond_account-7.2.2/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    46672 2024-04-30 17:20:59.000000 trytond_account-7.2.2/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    51736 2024-04-30 17:20:59.000000 trytond_account-7.2.2/aged_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.2/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6045 2024-04-30 17:20:59.000000 trytond_account-7.2.2/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3024 2024-04-30 17:20:59.000000 trytond_account-7.2.2/company.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8831 2024-04-30 17:20:59.000000 trytond_account-7.2.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1998 2024-04-30 17:20:59.000000 trytond_account-7.2.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.311757 trytond_account-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3070 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      957 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/configuration.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.315090 trytond_account-7.2.2/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6585 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/account.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      548 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/configuration.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3062 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/fiscal-year.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2246 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/journal.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6739 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/move.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4330 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/tax.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4793 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/design/template.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1558 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2929 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.318423 trytond_account-7.2.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/close.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1984 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/create.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      770 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2858 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/report.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/structure.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2092 2024-04-30 17:20:59.000000 trytond_account-7.2.2/doc/usage/view.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1808 2024-04-30 17:20:59.000000 trytond_account-7.2.2/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26581 2024-04-30 17:20:59.000000 trytond_account-7.2.2/fiscalyear.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7424 2024-04-30 17:20:59.000000 trytond_account-7.2.2/fiscalyear.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    52160 2024-04-30 17:20:59.000000 trytond_account-7.2.2/general_journal.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    81559 2024-04-30 17:20:59.000000 trytond_account-7.2.2/general_ledger.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.318423 trytond_account-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.2/icons/tryton-account-block.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:20:59.000000 trytond_account-7.2.2/icons/tryton-account-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:20:59.000000 trytond_account-7.2.2/icons/tryton-account-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-04-30 17:20:59.000000 trytond_account-7.2.2/icons/tryton-account.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    13491 2024-04-30 17:20:59.000000 trytond_account-7.2.2/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12289 2024-04-30 17:20:59.000000 trytond_account-7.2.2/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.321757 trytond_account-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   131048 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130583 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114241 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134193 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   130891 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118935 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   127139 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   138558 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   118048 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   132823 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125558 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   117226 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122882 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   143189 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   134790 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   131232 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   122265 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   125426 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   129848 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   133001 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   123107 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   114073 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   148010 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   126059 2024-04-30 17:21:59.000000 trytond_account-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1494 2024-04-30 17:20:59.000000 trytond_account-7.2.2/localize.xsl
+-rw-r--r--   0 ced       (1000) ced       (1000)    17448 2024-04-30 17:21:06.000000 trytond_account-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22110 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11303 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11052 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11058 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11004 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11069 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11050 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11083 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11090 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11405 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11056 2024-04-30 17:20:59.000000 trytond_account-7.2.2/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   116694 2024-05-11 10:33:53.000000 trytond_account-7.2.2/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26295 2024-04-30 17:20:59.000000 trytond_account-7.2.2/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    15750 2024-04-30 17:20:59.000000 trytond_account-7.2.2/move_template.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6717 2024-04-30 17:20:59.000000 trytond_account-7.2.2/move_template.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13753 2024-05-11 10:31:31.000000 trytond_account-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4156 2024-04-30 17:20:59.000000 trytond_account-7.2.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16319 2024-04-30 17:20:59.000000 trytond_account-7.2.2/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4083 2024-04-30 17:20:59.000000 trytond_account-7.2.2/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 17:11:58.335090 trytond_account-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4586 2024-04-30 17:20:59.000000 trytond_account-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    70885 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24263 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tax.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.321757 trytond_account-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4618 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_active.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       64 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconcile.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3995 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconcile.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2442 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconcile_automatic.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconciliation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     3706 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       56 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency_write_off.json
+-rw-r--r--   0 ced       (1000) ced       (1000)     4420 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency_write_off.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4736 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_close_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4270 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_move_cancel.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2951 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_move_line_delegate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5021 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_move_line_group.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4907 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_move_line_reschedule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5018 2024-05-11 10:33:53.000000 trytond_account-7.2.2/tests/scenario_move_template.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2223 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    10860 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_reports.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2658 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/scenario_tax_code.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    80138 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4788 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)    47972 2024-04-30 17:20:59.000000 trytond_account-7.2.2/trial_balance.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-05-01 12:38:46.000000 trytond_account-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.335090 trytond_account-7.2.2/trytond_account.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2846 2024-05-15 17:11:57.000000 trytond_account-7.2.2/trytond_account.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    12499 2024-05-15 17:11:58.000000 trytond_account-7.2.2/trytond_account.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 17:11:57.000000 trytond_account-7.2.2/trytond_account.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       52 2024-05-15 17:11:57.000000 trytond_account-7.2.2/trytond_account.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:38:35.000000 trytond_account-7.2.2/trytond_account.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-05-15 17:11:57.000000 trytond_account-7.2.2/trytond_account.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 17:11:57.000000 trytond_account-7.2.2/trytond_account.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    54595 2024-04-30 17:20:59.000000 trytond_account-7.2.2/type_statement.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 17:11:58.335090 trytond_account-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_balance_sheet_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_deferral_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_deferral_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2841 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_income_statement_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_list_balance_sheet.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1074 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1283 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1103 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/account_type_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/aged_balance_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/aged_balance_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/balance_sheet_context_comparison_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/balance_sheet_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      710 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/company_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1353 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      362 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/create_chart_account_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/create_chart_properties_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/create_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/fiscalyear_balance_non_deferral_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/fiscalyear_create_periods_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      910 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      413 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/fiscalyear_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/fiscalyear_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      750 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/general_ledger_account_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/general_ledger_account_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/general_ledger_account_party_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/general_ledger_line_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      784 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/general_ledger_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1138 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/income_statement_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_list_cash.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_list_matching_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_open_cash_context.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      272 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_cancel_default_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_delegate_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1753 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1241 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_form_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_group_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      665 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_list_payable_receivable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      475 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_list_reconcile.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_receivable_payable_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_reschedule_preview_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_reschedule_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      262 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_reschedule_term_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1026 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      636 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_line_tree_move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_reconciliation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_reconciliation_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_create_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      857 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_keyword_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/open_journal_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1161 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/period_list_close.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/period_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      476 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/reconcile_lines_writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      755 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/reconcile_show_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/reconcile_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/renew_fiscalyear_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1122 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      338 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      843 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_code_tree_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2193 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_group_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_line_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      516 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      716 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      655 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_line_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_line_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      417 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      401 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      380 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_template_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_rule_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2101 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      371 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/tax_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      250 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/update_chart_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/update_chart_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/writeoff_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account-7.2.2/view/writeoff_tree.xml
```

### Comparing `trytond_account-7.2.1/CHANGELOG` & `trytond_account-7.2.2/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_account-7.2.1/COPYRIGHT` & `trytond_account-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/LICENSE` & `trytond_account-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/PKG-INFO` & `trytond_account-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-7.2.1/__init__.py` & `trytond_account-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/account.py` & `trytond_account-7.2.2/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/account.xml` & `trytond_account-7.2.2/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/aged_balance.fodt` & `trytond_account-7.2.2/aged_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/common.py` & `trytond_account-7.2.2/common.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/company.py` & `trytond_account-7.2.2/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/company.xml` & `trytond_account-7.2.2/company.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/configuration.py` & `trytond_account-7.2.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/configuration.xml` & `trytond_account-7.2.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/conf.py` & `trytond_account-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/configuration.rst` & `trytond_account-7.2.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/account.inc.rst` & `trytond_account-7.2.2/doc/design/account.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/configuration.inc.rst` & `trytond_account-7.2.2/doc/design/configuration.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/fiscal-year.inc.rst` & `trytond_account-7.2.2/doc/design/fiscal-year.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/journal.inc.rst` & `trytond_account-7.2.2/doc/design/journal.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/move.inc.rst` & `trytond_account-7.2.2/doc/design/move.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/tax.inc.rst` & `trytond_account-7.2.2/doc/design/tax.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/design/template.inc.rst` & `trytond_account-7.2.2/doc/design/template.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/reference.rst` & `trytond_account-7.2.2/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/setup.rst` & `trytond_account-7.2.2/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/close.inc.rst` & `trytond_account-7.2.2/doc/usage/close.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/create.inc.rst` & `trytond_account-7.2.2/doc/usage/create.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/process.inc.rst` & `trytond_account-7.2.2/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/report.inc.rst` & `trytond_account-7.2.2/doc/usage/report.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/structure.inc.rst` & `trytond_account-7.2.2/doc/usage/structure.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/doc/usage/view.inc.rst` & `trytond_account-7.2.2/doc/usage/view.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/exceptions.py` & `trytond_account-7.2.2/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/fiscalyear.py` & `trytond_account-7.2.2/fiscalyear.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/fiscalyear.xml` & `trytond_account-7.2.2/fiscalyear.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/general_journal.fodt` & `trytond_account-7.2.2/general_journal.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/general_ledger.fodt` & `trytond_account-7.2.2/general_ledger.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/icons/LICENSE` & `trytond_account-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/journal.py` & `trytond_account-7.2.2/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/journal.xml` & `trytond_account-7.2.2/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/bg.po` & `trytond_account-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/ca.po` & `trytond_account-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/cs.po` & `trytond_account-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/de.po` & `trytond_account-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/es.po` & `trytond_account-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/es_419.po` & `trytond_account-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/et.po` & `trytond_account-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/fa.po` & `trytond_account-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/fi.po` & `trytond_account-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/fr.po` & `trytond_account-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/hu.po` & `trytond_account-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/id.po` & `trytond_account-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/it.po` & `trytond_account-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/lo.po` & `trytond_account-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/lt.po` & `trytond_account-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/nl.po` & `trytond_account-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/pl.po` & `trytond_account-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/pt.po` & `trytond_account-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/ro.po` & `trytond_account-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/ru.po` & `trytond_account-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/sl.po` & `trytond_account-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/tr.po` & `trytond_account-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/uk.po` & `trytond_account-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/locale/zh_CN.po` & `trytond_account-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/localize.xsl` & `trytond_account-7.2.2/localize.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/message.xml` & `trytond_account-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart.xml` & `trytond_account-7.2.2/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_bg.xml` & `trytond_account-7.2.2/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_ca.xml` & `trytond_account-7.2.2/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_de.xml` & `trytond_account-7.2.2/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_en.xml` & `trytond_account-7.2.2/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_es.xml` & `trytond_account-7.2.2/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_fr.xml` & `trytond_account-7.2.2/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_nl.xml` & `trytond_account-7.2.2/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_pt.xml` & `trytond_account-7.2.2/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_ru.xml` & `trytond_account-7.2.2/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/minimal_chart_sl.xml` & `trytond_account-7.2.2/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/move.py` & `trytond_account-7.2.2/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -1451,40 +1451,40 @@
         Move.validate_move(list(set(l.move for l in all_lines) | set(moves)))
 
     @classmethod
     def create(cls, vlist):
         pool = Pool()
         Move = pool.get('account.move')
 
-        def move_fields():
+        def move_fields(move_name):
             for fname, field in cls._fields.items():
                 if (isinstance(field, fields.Function)
                         and field.setter == 'set_move_field'):
-                    if fname.startswith('move_'):
+                    if move_name and fname.startswith('move_'):
                         fname = fname[5:]
                     yield fname
 
         moves = {}
         context = Transaction().context
         vlist = [x.copy() for x in vlist]
         for vals in vlist:
             if not vals.get('move'):
                 move_values = {}
-                for fname in move_fields():
+                for fname in move_fields(move_name=True):
                     move_values[fname] = vals.get(fname) or context.get(fname)
                 key = tuple(sorted(move_values.items()))
                 move = moves.get(key)
                 if move is None:
                     move = Move(**move_values)
                     move.save()
                     moves[key] = move
                 vals['move'] = move.id
             else:
                 # prevent default value for field with set_move_field
-                for fname in move_fields():
+                for fname in move_fields(move_name=False):
                     vals.setdefault(fname, None)
         lines = super(Line, cls).create(vlist)
         period_and_journals = set((line.period, line.journal)
             for line in lines)
         for period, journal in period_and_journals:
             cls.check_journal_period_modify(period, journal)
         # Re-browse for cache alignment
```

### Comparing `trytond_account-7.2.1/move.xml` & `trytond_account-7.2.2/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/move_template.py` & `trytond_account-7.2.2/move_template.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/move_template.xml` & `trytond_account-7.2.2/move_template.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/party.py` & `trytond_account-7.2.2/party.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     def default_supplier_tax_rule(cls, **pattern):
         return cls._default_tax_rule('supplier', **pattern)
 
     def get_currency(self, name):
         pool = Pool()
         Company = pool.get('company.company')
         company_id = Transaction().context.get('company')
-        if company_id >= 0:
+        if company_id is not None and company_id >= 0:
             company = Company(company_id)
             return company.currency
 
     @classmethod
     def get_receivable_payable(cls, parties, names):
         '''
         Function to compute receivable, payable (today or not) for party ids.
```

### Comparing `trytond_account-7.2.1/party.xml` & `trytond_account-7.2.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/period.py` & `trytond_account-7.2.2/period.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/period.xml` & `trytond_account-7.2.2/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/setup.py` & `trytond_account-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tax.py` & `trytond_account-7.2.2/tax.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tax.xml` & `trytond_account-7.2.2/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_active.rst` & `trytond_account-7.2.2/tests/scenario_account_active.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_reconcile.rst` & `trytond_account-7.2.2/tests/scenario_account_reconcile.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_reconcile_automatic.rst` & `trytond_account-7.2.2/tests/scenario_account_reconcile_automatic.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_reconciliation.rst` & `trytond_account-7.2.2/tests/scenario_account_reconciliation.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency.rst` & `trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_account_reconciliation_alternate_currency_write_off.rst` & `trytond_account-7.2.2/tests/scenario_account_reconciliation_alternate_currency_write_off.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_close_fiscalyear.rst` & `trytond_account-7.2.2/tests/scenario_close_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_move_cancel.rst` & `trytond_account-7.2.2/tests/scenario_move_cancel.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_move_line_delegate.rst` & `trytond_account-7.2.2/tests/scenario_move_line_delegate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_move_line_group.rst` & `trytond_account-7.2.2/tests/scenario_move_line_group.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_move_line_reschedule.rst` & `trytond_account-7.2.2/tests/scenario_move_line_reschedule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_move_template.rst` & `trytond_account-7.2.2/tests/scenario_move_template.rst`

 * *Files 3% similar despite different names*

```diff
@@ -72,26 +72,29 @@
     ...     type_='numeric', digits=2)
     >>> template.description = '{party} - {description}'
     >>> line = template.lines.new()
     >>> line.operation = 'credit'
     >>> line.account = payable
     >>> line.party = 'party'
     >>> line.amount = 'amount'
+    >>> line.description = "{description} 1"
     >>> line = template.lines.new()
     >>> line.operation = 'debit'
     >>> line.account = expense
     >>> line.amount = 'amount / 1.1'
     >>> ttax = line.taxes.new()
     >>> ttax.amount = line.amount
     >>> ttax.tax = tax
     >>> ttax.type = 'base'
+    >>> line.description = "{description} 2"
     >>> line = template.lines.new()
     >>> line.operation = 'debit'
     >>> line.account = tax.invoice_account
     >>> line.amount = 'amount * (1 - 1/1.1)'
+    >>> line.description = "{description} 3"
     >>> ttax = line.taxes.new()
     >>> ttax.amount = line.amount
     >>> ttax.tax = tax
     >>> ttax.type = 'tax'
     >>> template.save()
 
 Create Move::
@@ -128,14 +131,16 @@
 
     >>> Move = Model.get('account.move')
     >>> move, = Move.find([])
     >>> len(move.lines)
     3
     >>> sorted((l.debit, l.credit) for l in move.lines)
     [(Decimal('0'), Decimal('12.24')), (Decimal('1.11'), Decimal('0')), (Decimal('11.13'), Decimal('0'))]
+    >>> sorted([l.description for l in move.lines])
+    ['Test 1', 'Test 2', 'Test 3']
     >>> move.description
     'Supplier - Test'
     >>> with config.set_context(periods=period_ids):
     ...     base_code = TaxCode(base_code.id)
     ...     base_code.amount
     Decimal('11.13')
     >>> with config.set_context(periods=period_ids):
```

### Comparing `trytond_account-7.2.1/tests/scenario_renew_fiscalyear.rst` & `trytond_account-7.2.2/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_reports.rst` & `trytond_account-7.2.2/tests/scenario_reports.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/scenario_tax_code.rst` & `trytond_account-7.2.2/tests/scenario_tax_code.rst`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/test_module.py` & `trytond_account-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tests/tools.py` & `trytond_account-7.2.2/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tox.ini` & `trytond_account-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/trial_balance.fodt` & `trytond_account-7.2.2/trial_balance.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/tryton.cfg` & `trytond_account-7.2.2/tryton.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tryton]
-version=7.2.1
+version=7.2.2
 depends:
     company
     currency
     ir
     party
     res
 xml:
```

### Comparing `trytond_account-7.2.1/trytond_account.egg-info/PKG-INFO` & `trytond_account-7.2.2/trytond_account.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for accounting
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account-7.2.1/trytond_account.egg-info/SOURCES.txt` & `trytond_account-7.2.2/trytond_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/type_statement.fodt` & `trytond_account-7.2.2/type_statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/account_deferral_form.xml` & `trytond_account-7.2.2/view/account_deferral_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/account_form.xml` & `trytond_account-7.2.2/view/account_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/account_template_form.xml` & `trytond_account-7.2.2/view/account_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/account_type_form.xml` & `trytond_account-7.2.2/view/account_type_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/account_type_template_form.xml` & `trytond_account-7.2.2/view/account_type_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/aged_balance_context_form.xml` & `trytond_account-7.2.2/view/aged_balance_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/company_form.xml` & `trytond_account-7.2.2/view/company_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/configuration_form.xml` & `trytond_account-7.2.2/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/fiscalyear_balance_non_deferral_start_form.xml` & `trytond_account-7.2.2/view/fiscalyear_balance_non_deferral_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/fiscalyear_create_periods_start_form.xml` & `trytond_account-7.2.2/view/fiscalyear_create_periods_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/fiscalyear_form.xml` & `trytond_account-7.2.2/view/fiscalyear_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/general_ledger_account_context_form.xml` & `trytond_account-7.2.2/view/general_ledger_account_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/general_ledger_line_list.xml` & `trytond_account-7.2.2/view/general_ledger_line_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/income_statement_context_form.xml` & `trytond_account-7.2.2/view/income_statement_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/journal_form.xml` & `trytond_account-7.2.2/view/journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/journal_period_form.xml` & `trytond_account-7.2.2/view/journal_period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_form.xml` & `trytond_account-7.2.2/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_form.xml` & `trytond_account-7.2.2/view/move_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_form_move.xml` & `trytond_account-7.2.2/view/move_line_form_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_list_payable_receivable.xml` & `trytond_account-7.2.2/view/move_line_list_payable_receivable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_reschedule_start_form.xml` & `trytond_account-7.2.2/view/move_line_reschedule_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_template_form.xml` & `trytond_account-7.2.2/view/move_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_tree.xml` & `trytond_account-7.2.2/view/move_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_line_tree_move.xml` & `trytond_account-7.2.2/view/move_line_tree_move.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_template_form.xml` & `trytond_account-7.2.2/view/move_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_template_keyword_form.xml` & `trytond_account-7.2.2/view/move_template_keyword_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/move_tree.xml` & `trytond_account-7.2.2/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/party_form.xml` & `trytond_account-7.2.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/period_form.xml` & `trytond_account-7.2.2/view/period_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/reconcile_show_form.xml` & `trytond_account-7.2.2/view/reconcile_show_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/renew_fiscalyear_start_form.xml` & `trytond_account-7.2.2/view/renew_fiscalyear_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_code_context_form.xml` & `trytond_account-7.2.2/view/tax_code_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_code_form.xml` & `trytond_account-7.2.2/view/tax_code_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_code_template_form.xml` & `trytond_account-7.2.2/view/tax_code_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_form.xml` & `trytond_account-7.2.2/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_rule_form.xml` & `trytond_account-7.2.2/view/tax_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_rule_line_form.xml` & `trytond_account-7.2.2/view/tax_rule_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_rule_line_template_form.xml` & `trytond_account-7.2.2/view/tax_rule_line_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_template_form.xml` & `trytond_account-7.2.2/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/tax_test_form.xml` & `trytond_account-7.2.2/view/tax_test_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account-7.2.1/view/writeoff_form.xml` & `trytond_account-7.2.2/view/writeoff_form.xml`

 * *Files identical despite different names*

