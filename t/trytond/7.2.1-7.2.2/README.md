# Comparing `tmp/trytond-7.2.1.tar.gz` & `tmp/trytond-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-7.2.1.tar", last modified: Wed May  1 09:08:01 2024, max compression
+gzip compressed data, was "trytond-7.2.2.tar", last modified: Wed May 15 16:59:22 2024, max compression
```

## Comparing `trytond-7.2.1.tar` & `trytond-7.2.2.tar`

### file list

```diff
@@ -1,609 +1,609 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.671817 trytond-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)    41305 2024-05-01 09:07:58.000000 trytond-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-05-01 09:07:58.000000 trytond-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2024-04-30 17:21:00.000000 trytond-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-01 09:08:01.668483 trytond-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2024-04-30 17:21:00.000000 trytond-7.2.1/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2890 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond
--rwxr-xr-x   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-admin
--rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-console
--rwxr-xr-x   0 ced       (1000) ced       (1000)      949 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-cron
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-stat
--rwxr-xr-x   0 ced       (1000) ced       (1000)     1088 2024-04-30 17:21:00.000000 trytond-7.2.1/bin/trytond-worker
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/modules/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     3741 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/modules/res/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.625151 trytond-7.2.1/doc/ref/
--rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/backend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2656 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/cache.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/exceptions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    32469 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1171 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/filestore.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/i18n.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    33575 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/models.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/pool.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8787 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/pyson.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2640 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/sendmail.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4738 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tests.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/ref/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/barcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/immutabledict.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/logging.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/misc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/qrcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/singleton.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      608 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/tools/timezone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5550 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/transaction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6064 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/ref/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/
--rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/access_rights.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/actions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4014 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/backend_types.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14914 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1431 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/cron.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7848 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/domain.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/install.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1108 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/logs.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/models/
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/fields_default_value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/fields_on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1376 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/models/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)     6022 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/modules/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3887 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/pyson.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/reports/
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/reports/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/start_server.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/task_queue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2884 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/testing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/translation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/triggers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/user_errors_warnings.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/topics/views/
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/views/extension.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    25819 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/views/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1669 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/topics/wizard.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.628485 trytond-7.2.1/doc/tutorial/
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/doc/tutorial/module/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/anatomy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/default_values.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3334 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/domains.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2917 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/extend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/function_fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3949 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/model.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/states.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4746 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/table_query.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6258 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4727 2024-04-30 17:21:00.000000 trytond-7.2.1/doc/tutorial/module/workflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:08:01.671817 trytond-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5625 2024-04-30 17:21:00.000000 trytond-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      624 2024-04-30 17:21:00.000000 trytond-7.2.1/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-30 17:21:06.000000 trytond-7.2.1/trytond/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6968 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/admin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/application.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/backend/
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/database.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.631818 trytond-7.2.1/trytond/backend/postgresql/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26951 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4829 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    29327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/postgresql/table.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.635151 trytond-7.2.1/trytond/backend/sqlite/
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20807 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    15183 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/sqlite/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4248 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/backend/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9431 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7715 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/commandline.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2280 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/console.py
--rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31204 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/convert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2098 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/i18n.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/
--rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    40622 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10524 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/action.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/attachment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4282 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/calendar_.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1459 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7912 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/cron.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4502 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/email.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20520 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6087 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/error.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/error.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/export.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/export.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/fonts/
--rw-r--r--   0 ced       (1000) ced       (1000)     4384 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/fonts/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    58284 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/fonts/karla.ttf
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22311 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/lang.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27181 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/lang.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.638484 trytond-7.2.1/trytond/ir/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   104527 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103796 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90725 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   105509 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   104656 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85420 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97499 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   106723 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90400 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   105628 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100392 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90128 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100022 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    95895 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    95896 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103249 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103641 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100851 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103060 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   106898 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98720 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90532 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   115724 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100387 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/ir/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/message.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22606 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    64603 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15908 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/model.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    18462 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/module.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/note.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/queue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9479 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/queue_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10185 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12027 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    16164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4927 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/session.py
--rw-r--r--   0 ced       (1000) ced       (1000)    67671 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/translation.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7726 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/translation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11517 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/trigger.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.641817 trytond-7.2.1/trytond/ir/ui/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/board.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    18063 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/board.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/calendar.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     3508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/calendar.rng
--rw-r--r--   0 ced       (1000) ced       (1000)    10397 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/form.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    35542 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/form.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/graph.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/graph.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icon.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1521 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icon.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.641817 trytond-7.2.1/trytond/ir/ui/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-board.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-calendar.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-folder.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-form.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-graph.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-list.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-settings.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/icons/tryton-tree.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    10200 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2962 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/menu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3895 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/tree.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/tree.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/ui.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    26813 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/view.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8412 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/ui/view.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.648484 trytond-7.2.1/trytond/ir/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_domain_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_act_window_view_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      952 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1358 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_report_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_report_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_wizard_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/action_wizard_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_form_preview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/attachment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/email_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/error_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/error_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/icon_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/icon_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/lang_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      787 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_click_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_click_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_button_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_data_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_data_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_field_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      388 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_log_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_log_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/model_print_model_graph_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_activate_upgrade_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_activate_upgrade_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_first_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_item_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_config_wizard_other_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_dependency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_dependency_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/module_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/note_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/note_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/sequence_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_clean_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_clean_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_export_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_set_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_set_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/translation_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1035 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/trigger_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/trigger_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_favorite_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_favorite_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_menu_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_list_extension.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_search_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_optional_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_optional_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_state_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_state_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_width_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/ir/view/ui_view_tree_width_list.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/model/
--rw-r--r--   0 ced       (1000) ced       (1000)     1199 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/active.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1050 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/dictschema.py
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/digits.py
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/model/fields/
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9426 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7052 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26432 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/fmany2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8403 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18816 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14114 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16101 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8415 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7508 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3439 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/fields/text.py
--rw-r--r--   0 ced       (1000) ced       (1000)      899 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/match.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17673 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    90408 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    84791 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    38145 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/order.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/symbol.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/union.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/model/workflow.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.651817 trytond-7.2.1/trytond/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)    13764 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/modules/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8803 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/pool.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/protocols/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9185 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/dispatcher.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5827 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/jsonrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10447 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/wrappers.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/protocols/xmlrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/report/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/report/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20078 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/report/report.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     1235 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1496 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/group.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8327 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22621 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.655151 trytond-7.2.1/trytond/res/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    13763 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14164 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12042 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14493 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14297 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    11652 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13112 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14122 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14674 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13523 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12552 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12870 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15494 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13624 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14229 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14286 2024-04-30 17:21:59.000000 trytond-7.2.1/trytond/res/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13963 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13969 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15820 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13532 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2458 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)    43182 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7748 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.658484 trytond-7.2.1/trytond/res/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1153 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_application_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_application_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1527 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1386 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_form_preferences.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_warning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/res/view/user_warning_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3973 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/security.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5662 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3227 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/status.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/copy_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2023 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/export_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_function.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7491 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3161 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1489 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1224 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)        9 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/forbidden.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5599 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/import_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/import_data.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1069 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1083 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4719 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8936 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7720 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8965 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/modelview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/path.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)      971 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36123 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6920 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_backend.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12678 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_copy.py
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15266 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_exportdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7404 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22837 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1021 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13633 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15520 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7608 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_depends.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27461 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13029 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3641 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10446 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25088 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15103 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12677 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17303 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23590 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9827 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20622 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9360 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19472 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15036 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17308 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3794 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_i18n.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20525 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_importdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19232 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_mixins.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17190 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_index.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4808 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_model_match.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    61345 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31037 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31080 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3450 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_path.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3726 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_protocols.py
--rw-r--r--   0 ced       (1000) ced       (1000)    36764 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2413 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6365 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4377 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25750 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4299 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)    48966 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12469 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15386 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)    45182 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_tryton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_union.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11366 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5406 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3171 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/test_wsgi.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1180 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tests/workflow.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/barcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/decimal_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2562 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/gevent.py
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/immutabledict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/logging.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9631 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/misc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1595 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/qrcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/singleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/string_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tools/timezone.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12819 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tryton.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/tryton.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/url.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond/wizard/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wizard/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15037 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wizard/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/worker.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9735 2024-04-30 17:21:00.000000 trytond-7.2.1/trytond/wsgi.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:08:01.668483 trytond-7.2.1/trytond.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:08:01.000000 trytond-7.2.1/trytond.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.844849 trytond-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41406 2024-05-15 16:59:19.000000 trytond-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2024-05-15 16:59:19.000000 trytond-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2024-04-30 17:21:00.000000 trytond-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-15 16:59:22.844849 trytond-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2024-04-30 17:21:00.000000 trytond-7.2.2/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.678187 trytond-7.2.2/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2890 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond-admin
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond-console
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      949 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond-cron
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond-stat
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     1088 2024-04-30 17:21:00.000000 trytond-7.2.2/bin/trytond-worker
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.678187 trytond-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2367 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1185 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.681520 trytond-7.2.2/doc/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)      169 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/modules/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.681520 trytond-7.2.2/doc/modules/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3741 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/modules/res/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/modules/res/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1546 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/modules/res/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3146 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/modules/res/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.684853 trytond-7.2.2/doc/ref/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10444 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/backend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/cache.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/exceptions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    32469 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1171 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/filestore.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/i18n.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    33575 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/models.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2149 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/pool.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8787 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/pyson.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2640 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/sendmail.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4738 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tests.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.688187 trytond-7.2.2/doc/ref/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/barcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      642 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/immutabledict.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      184 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      613 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/logging.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1959 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/misc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/qrcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/singleton.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      608 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/tools/timezone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5550 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/transaction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6064 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/ref/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/topics/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4008 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/access_rights.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/actions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4014 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/backend_types.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14914 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1431 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/cron.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7848 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/domain.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      986 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/install.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/logs.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/topics/models/
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/models/fields_default_value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/models/fields_on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1376 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/models/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/topics/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6022 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/modules/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/pyson.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/topics/reports/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/reports/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/start_server.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/task_queue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2884 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/testing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/translation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/triggers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/user_errors_warnings.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/topics/views/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/views/extension.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    25819 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/views/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1669 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/topics/wizard.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.694853 trytond-7.2.2/doc/tutorial/
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.701519 trytond-7.2.2/doc/tutorial/module/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/anatomy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/default_values.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3334 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/domains.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/extend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3524 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/function_fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3949 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/model.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2662 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1769 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/states.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4746 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/table_query.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6258 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4727 2024-04-30 17:21:00.000000 trytond-7.2.2/doc/tutorial/module/workflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-15 16:59:22.844849 trytond-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5625 2024-04-30 17:21:00.000000 trytond-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      624 2024-04-30 17:21:00.000000 trytond-7.2.2/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.708186 trytond-7.2.2/trytond/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-05-01 09:08:17.000000 trytond-7.2.2/trytond/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6968 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/admin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1455 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/application.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.708186 trytond-7.2.2/trytond/backend/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4455 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/database.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.711519 trytond-7.2.2/trytond/backend/postgresql/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/postgresql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26951 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/postgresql/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4829 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/postgresql/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    29327 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/postgresql/table.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.711519 trytond-7.2.2/trytond/backend/sqlite/
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/sqlite/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20807 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/sqlite/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4030 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/sqlite/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    15183 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/sqlite/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4248 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/backend/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9431 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16924 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7715 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/commandline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6318 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2280 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/console.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      441 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31204 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/convert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1500 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2098 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/i18n.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.724852 trytond-7.2.2/trytond/ir/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3372 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    40622 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10524 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/action.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2865 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/attachment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6508 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4282 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/calendar_.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7912 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/cron.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4502 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/email.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20520 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6087 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/error.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3523 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/error.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4213 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/export.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.724852 trytond-7.2.2/trytond/ir/fonts/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4384 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/fonts/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    58284 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/fonts/karla.ttf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22311 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/lang.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27181 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/lang.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.741518 trytond-7.2.2/trytond/ir/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   104527 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103796 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90725 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   105509 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   104656 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85420 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97499 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   106723 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90400 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   105628 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100392 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90128 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100022 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95895 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95896 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103249 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103641 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100851 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103060 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   106898 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98720 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90532 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   115724 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100387 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/ir/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/message.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22606 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    64603 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15908 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/model.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    18462 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8238 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/module.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4199 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/note.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/queue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9479 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/queue_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7910 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10189 2024-05-11 10:33:02.000000 trytond-7.2.2/trytond/ir/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12027 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    16164 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4927 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5562 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/session.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    67671 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/translation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/translation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11517 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/trigger.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.748185 trytond-7.2.2/trytond/ir/ui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/board.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    18063 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/board.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/calendar.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     3508 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/calendar.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)    10397 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/form.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    35542 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/form.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/graph.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5214 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/graph.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icon.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icon.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.751518 trytond-7.2.2/trytond/ir/ui/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-board.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-calendar.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-folder.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-form.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-graph.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-list.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-settings.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/icons/tryton-tree.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    10200 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2962 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/menu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3895 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/tree.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    13567 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/tree.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/ui.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    26813 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/view.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8412 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/ui/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.778184 trytond-7.2.2/trytond/ir/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_domain_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_domain_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_domain_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1136 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_act_window_view_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      952 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1358 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_report_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_report_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      455 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_wizard_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/action_wizard_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/attachment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/attachment_form_preview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/attachment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/email_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/error_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/error_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/export_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/export_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      510 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/icon_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/icon_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/lang_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/lang_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/lang_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      787 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_click_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_click_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      684 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_button_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_data_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_data_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      848 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_field_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_field_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      682 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_field_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      501 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_field_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      560 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      388 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_log_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_log_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/model_print_model_graph_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_activate_upgrade_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_activate_upgrade_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_config_wizard_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_config_wizard_first_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_config_wizard_item_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_config_wizard_other_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_dependency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_dependency_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/module_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/note_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/note_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1072 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/rule_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/rule_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/sequence_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_clean_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_clean_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_export_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      802 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      576 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_set_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_set_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/translation_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1035 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/trigger_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/trigger_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_menu_favorite_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_menu_favorite_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      575 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_menu_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_menu_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_menu_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      859 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      438 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_list_extension.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_search_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_optional_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_optional_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_state_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_state_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      408 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_width_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/ir/view/ui_view_tree_width_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.784851 trytond-7.2.2/trytond/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1199 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/active.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1050 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9327 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/dictschema.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/digits.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.791517 trytond-7.2.2/trytond/model/fields/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4592 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9426 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7052 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8365 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26432 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2603 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3164 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/fmany2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8403 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18816 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14114 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16101 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8415 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7508 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3439 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/fields/text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      899 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17673 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    90408 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    84791 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    38145 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2712 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/symbol.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7250 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/model/workflow.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.791517 trytond-7.2.2/trytond/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13764 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/modules/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8803 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/pool.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.791517 trytond-7.2.2/trytond/protocols/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/protocols/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9185 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/protocols/dispatcher.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5827 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/protocols/jsonrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10447 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/protocols/wrappers.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/protocols/xmlrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24260 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.791517 trytond-7.2.2/trytond/report/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/report/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20078 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/report/report.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.798184 trytond-7.2.2/trytond/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1235 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1496 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3392 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2430 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/group.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8327 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22621 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.804850 trytond-7.2.2/trytond/res/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13763 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14164 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/res/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12042 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14493 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/res/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14297 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/res/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    11652 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13112 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14122 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14674 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13523 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12552 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12870 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15494 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13624 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14229 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/res/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14286 2024-04-30 17:21:59.000000 trytond-7.2.2/trytond/res/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13151 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13963 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13949 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13969 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12003 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15820 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13532 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1570 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2458 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)    43182 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7748 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.808183 trytond-7.2.2/trytond/res/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1153 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_application_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_application_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1527 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1386 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_form_preferences.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_warning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/res/view/user_warning_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3973 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6000 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/security.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5662 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3227 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/status.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.838183 trytond-7.2.2/trytond/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2433 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/copy_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2023 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/export_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_function.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7491 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3161 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1981 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1224 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)        9 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/forbidden.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5599 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/import_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/import_data.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1069 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1083 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4719 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8936 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7720 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8965 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/modelview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      971 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36123 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6920 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_backend.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10720 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12678 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_copy.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15266 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_exportdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7404 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22837 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1021 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13633 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15520 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7608 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_depends.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27461 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13029 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3641 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10446 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25088 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15103 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12677 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17303 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23590 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9827 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20622 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19472 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15036 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3019 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17308 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3794 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_i18n.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20525 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_importdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19232 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_mixins.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17190 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6973 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_model_index.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4808 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_model_match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    61345 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31037 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31080 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8733 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3726 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_protocols.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    36764 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2413 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3214 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25750 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4299 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5462 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    48966 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5859 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12469 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15386 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    45182 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_tryton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3353 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11366 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5406 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3171 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/test_wsgi.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1307 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1180 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tests/workflow.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.841516 trytond-7.2.2/trytond/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/barcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/decimal_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/gevent.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/immutabledict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3677 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/logging.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9631 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/misc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1595 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/qrcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/singleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/string_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tools/timezone.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12819 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tryton.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/tryton.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/url.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.841516 trytond-7.2.2/trytond/wizard/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/wizard/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15037 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/wizard/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7318 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/worker.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9735 2024-04-30 17:21:00.000000 trytond-7.2.2/trytond/wsgi.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-15 16:59:22.841516 trytond-7.2.2/trytond.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3982 2024-05-15 16:59:22.000000 trytond-7.2.2/trytond.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    16565 2024-05-15 16:59:22.000000 trytond-7.2.2/trytond.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-15 16:59:22.000000 trytond-7.2.2/trytond.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:08:01.000000 trytond-7.2.2/trytond.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      598 2024-05-15 16:59:22.000000 trytond-7.2.2/trytond.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-15 16:59:22.000000 trytond-7.2.2/trytond.egg-info/top_level.txt
```

### Comparing `trytond-7.2.1/CHANGELOG` & `trytond-7.2.2/CHANGELOG`

 * *Files 0% similar despite different names*

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

### Comparing `trytond-7.2.1/COPYRIGHT` & `trytond-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/LICENSE` & `trytond-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/PKG-INFO` & `trytond-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-7.2.1/bin/trytond` & `trytond-7.2.2/bin/trytond`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/bin/trytond-admin` & `trytond-7.2.2/bin/trytond-admin`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/bin/trytond-console` & `trytond-7.2.2/bin/trytond-console`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/bin/trytond-cron` & `trytond-7.2.2/bin/trytond-cron`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/bin/trytond-stat` & `trytond-7.2.2/bin/trytond-stat`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/bin/trytond-worker` & `trytond-7.2.2/bin/trytond-worker`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/conf.py` & `trytond-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/index.rst` & `trytond-7.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/modules/res/design.rst` & `trytond-7.2.2/doc/modules/res/design.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/modules/res/setup.rst` & `trytond-7.2.2/doc/modules/res/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/modules/res/usage.rst` & `trytond-7.2.2/doc/modules/res/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/backend.rst` & `trytond-7.2.2/doc/ref/backend.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/bus.rst` & `trytond-7.2.2/doc/ref/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/cache.rst` & `trytond-7.2.2/doc/ref/cache.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/exceptions.rst` & `trytond-7.2.2/doc/ref/exceptions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/fields.rst` & `trytond-7.2.2/doc/ref/fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/filestore.rst` & `trytond-7.2.2/doc/ref/filestore.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/i18n.rst` & `trytond-7.2.2/doc/ref/i18n.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/models.rst` & `trytond-7.2.2/doc/ref/models.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/pool.rst` & `trytond-7.2.2/doc/ref/pool.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/pyson.rst` & `trytond-7.2.2/doc/ref/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/rpc.rst` & `trytond-7.2.2/doc/ref/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/sendmail.rst` & `trytond-7.2.2/doc/ref/sendmail.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tests.rst` & `trytond-7.2.2/doc/ref/tests.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tools/barcode.rst` & `trytond-7.2.2/doc/ref/tools/barcode.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tools/email.rst` & `trytond-7.2.2/doc/ref/tools/email.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tools/logging.rst` & `trytond-7.2.2/doc/ref/tools/logging.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tools/misc.rst` & `trytond-7.2.2/doc/ref/tools/misc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/tools/timezone.rst` & `trytond-7.2.2/doc/ref/tools/timezone.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/transaction.rst` & `trytond-7.2.2/doc/ref/transaction.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/ref/wizard.rst` & `trytond-7.2.2/doc/ref/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/access_rights.rst` & `trytond-7.2.2/doc/topics/access_rights.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/actions.rst` & `trytond-7.2.2/doc/topics/actions.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/backend_types.rst` & `trytond-7.2.2/doc/topics/backend_types.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/bus.rst` & `trytond-7.2.2/doc/topics/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/configuration.rst` & `trytond-7.2.2/doc/topics/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/cron.rst` & `trytond-7.2.2/doc/topics/cron.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/domain.rst` & `trytond-7.2.2/doc/topics/domain.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/index.rst` & `trytond-7.2.2/doc/topics/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/install.rst` & `trytond-7.2.2/doc/topics/install.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/logs.rst` & `trytond-7.2.2/doc/topics/logs.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/models/fields_default_value.rst` & `trytond-7.2.2/doc/topics/models/fields_default_value.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/models/fields_on_change.rst` & `trytond-7.2.2/doc/topics/models/fields_on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/models/index.rst` & `trytond-7.2.2/doc/topics/models/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/modules/index.rst` & `trytond-7.2.2/doc/topics/modules/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/pyson.rst` & `trytond-7.2.2/doc/topics/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/reports/index.rst` & `trytond-7.2.2/doc/topics/reports/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/rpc.rst` & `trytond-7.2.2/doc/topics/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/setup_database.rst` & `trytond-7.2.2/doc/topics/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/start_server.rst` & `trytond-7.2.2/doc/topics/start_server.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/task_queue.rst` & `trytond-7.2.2/doc/topics/task_queue.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/testing.rst` & `trytond-7.2.2/doc/topics/testing.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/translation.rst` & `trytond-7.2.2/doc/topics/translation.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/triggers.rst` & `trytond-7.2.2/doc/topics/triggers.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/user_application.rst` & `trytond-7.2.2/doc/topics/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/user_errors_warnings.rst` & `trytond-7.2.2/doc/topics/user_errors_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/views/extension.rst` & `trytond-7.2.2/doc/topics/views/extension.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/views/index.rst` & `trytond-7.2.2/doc/topics/views/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/topics/wizard.rst` & `trytond-7.2.2/doc/topics/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/anatomy.rst` & `trytond-7.2.2/doc/tutorial/module/anatomy.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/default_values.rst` & `trytond-7.2.2/doc/tutorial/module/default_values.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/domains.rst` & `trytond-7.2.2/doc/tutorial/module/domains.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/extend.rst` & `trytond-7.2.2/doc/tutorial/module/extend.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/function_fields.rst` & `trytond-7.2.2/doc/tutorial/module/function_fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/index.rst` & `trytond-7.2.2/doc/tutorial/module/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/model.rst` & `trytond-7.2.2/doc/tutorial/module/model.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/on_change.rst` & `trytond-7.2.2/doc/tutorial/module/on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/report.rst` & `trytond-7.2.2/doc/tutorial/module/report.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/setup.rst` & `trytond-7.2.2/doc/tutorial/module/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/setup_database.rst` & `trytond-7.2.2/doc/tutorial/module/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/states.rst` & `trytond-7.2.2/doc/tutorial/module/states.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/table_query.rst` & `trytond-7.2.2/doc/tutorial/module/table_query.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/view.rst` & `trytond-7.2.2/doc/tutorial/module/view.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/wizard.rst` & `trytond-7.2.2/doc/tutorial/module/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/doc/tutorial/module/workflow.rst` & `trytond-7.2.2/doc/tutorial/module/workflow.rst`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/setup.py` & `trytond-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/tox.ini` & `trytond-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/__init__.py` & `trytond-7.2.2/trytond/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from lxml import etree, objectify
 
 try:
     from requests import utils as requests_utils
 except ImportError:
     requests_utils = None
 
-__version__ = "7.2.1"
+__version__ = "7.2.2"
 
 os.environ.setdefault(
     'TRYTOND_APPNAME',
     os.path.basename(getattr(__main__, '__file__', 'trytond')))
 os.environ.setdefault('TRYTOND_TZ', os.environ.get('TZ', 'UTC'))
 os.environ['TZ'] = 'UTC'
 if hasattr(time, 'tzset'):
```

### Comparing `trytond-7.2.1/trytond/admin.py` & `trytond-7.2.2/trytond/admin.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/application.py` & `trytond-7.2.2/trytond/application.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/__init__.py` & `trytond-7.2.2/trytond/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/database.py` & `trytond-7.2.2/trytond/backend/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/postgresql/database.py` & `trytond-7.2.2/trytond/backend/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/postgresql/init.sql` & `trytond-7.2.2/trytond/backend/postgresql/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/postgresql/table.py` & `trytond-7.2.2/trytond/backend/postgresql/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/sqlite/database.py` & `trytond-7.2.2/trytond/backend/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/sqlite/init.sql` & `trytond-7.2.2/trytond/backend/sqlite/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/sqlite/table.py` & `trytond-7.2.2/trytond/backend/sqlite/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/backend/table.py` & `trytond-7.2.2/trytond/backend/table.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/bus.py` & `trytond-7.2.2/trytond/bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/cache.py` & `trytond-7.2.2/trytond/cache.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/commandline.py` & `trytond-7.2.2/trytond/commandline.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/config.py` & `trytond-7.2.2/trytond/config.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/console.py` & `trytond-7.2.2/trytond/console.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/convert.py` & `trytond-7.2.2/trytond/convert.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/cron.py` & `trytond-7.2.2/trytond/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/exceptions.py` & `trytond-7.2.2/trytond/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/filestore.py` & `trytond-7.2.2/trytond/filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/i18n.py` & `trytond-7.2.2/trytond/i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/__init__.py` & `trytond-7.2.2/trytond/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/action.py` & `trytond-7.2.2/trytond/ir/action.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/action.xml` & `trytond-7.2.2/trytond/ir/action.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/attachment.py` & `trytond-7.2.2/trytond/ir/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/attachment.xml` & `trytond-7.2.2/trytond/ir/attachment.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/avatar.py` & `trytond-7.2.2/trytond/ir/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/calendar_.py` & `trytond-7.2.2/trytond/ir/calendar_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/calendar_.xml` & `trytond-7.2.2/trytond/ir/calendar_.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/configuration.py` & `trytond-7.2.2/trytond/ir/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/cron.py` & `trytond-7.2.2/trytond/ir/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/cron.xml` & `trytond-7.2.2/trytond/ir/cron.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/date.py` & `trytond-7.2.2/trytond/ir/date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/email.xml` & `trytond-7.2.2/trytond/ir/email.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/email_.py` & `trytond-7.2.2/trytond/ir/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/error.py` & `trytond-7.2.2/trytond/ir/error.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/error.xml` & `trytond-7.2.2/trytond/ir/error.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/exceptions.py` & `trytond-7.2.2/trytond/ir/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/export.py` & `trytond-7.2.2/trytond/ir/export.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/export.xml` & `trytond-7.2.2/trytond/ir/export.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/fonts/LICENSE` & `trytond-7.2.2/trytond/ir/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/fonts/karla.ttf` & `trytond-7.2.2/trytond/ir/fonts/karla.ttf`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ir.xml` & `trytond-7.2.2/trytond/ir/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/lang.py` & `trytond-7.2.2/trytond/ir/lang.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/lang.xml` & `trytond-7.2.2/trytond/ir/lang.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/bg.po` & `trytond-7.2.2/trytond/ir/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/ca.po` & `trytond-7.2.2/trytond/ir/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/cs.po` & `trytond-7.2.2/trytond/ir/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/de.po` & `trytond-7.2.2/trytond/ir/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/es.po` & `trytond-7.2.2/trytond/ir/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/es_419.po` & `trytond-7.2.2/trytond/ir/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/et.po` & `trytond-7.2.2/trytond/ir/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/fa.po` & `trytond-7.2.2/trytond/ir/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/fi.po` & `trytond-7.2.2/trytond/ir/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/fr.po` & `trytond-7.2.2/trytond/ir/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/hu.po` & `trytond-7.2.2/trytond/ir/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/id.po` & `trytond-7.2.2/trytond/ir/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/it.po` & `trytond-7.2.2/trytond/ir/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/lo.po` & `trytond-7.2.2/trytond/ir/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/lt.po` & `trytond-7.2.2/trytond/ir/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/nl.po` & `trytond-7.2.2/trytond/ir/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/pl.po` & `trytond-7.2.2/trytond/ir/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/pt.po` & `trytond-7.2.2/trytond/ir/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/ro.po` & `trytond-7.2.2/trytond/ir/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/ru.po` & `trytond-7.2.2/trytond/ir/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/sl.po` & `trytond-7.2.2/trytond/ir/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/tr.po` & `trytond-7.2.2/trytond/ir/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/uk.po` & `trytond-7.2.2/trytond/ir/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/locale/zh_CN.po` & `trytond-7.2.2/trytond/ir/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/message.py` & `trytond-7.2.2/trytond/ir/message.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/message.xml` & `trytond-7.2.2/trytond/ir/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/model.py` & `trytond-7.2.2/trytond/ir/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/model.xml` & `trytond-7.2.2/trytond/ir/model.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/module.py` & `trytond-7.2.2/trytond/ir/module.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/module.xml` & `trytond-7.2.2/trytond/ir/module.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/note.py` & `trytond-7.2.2/trytond/ir/note.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/note.xml` & `trytond-7.2.2/trytond/ir/note.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/queue_.py` & `trytond-7.2.2/trytond/ir/queue_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/resource.py` & `trytond-7.2.2/trytond/ir/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/routes.py` & `trytond-7.2.2/trytond/ir/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 text = text.decode('utf-8')
             except UnicodeDecodeError as e:
                 error = str(e).replace("'", "\\'")
                 text = ''
         elif not isinstance(text, str):
             abort(HTTPStatus.BAD_REQUEST)
         title = '%(model)s "%(name)s" %(field)s - %(title)s' % {
-            'model': field.model.name,
+            'model': field.model_ref.name,
             'name': record.rec_name,
             'field': field.field_description,
             'title': request.args.get('title', "Tryton"),
             }
 
         return Response(TEMPLATE % {
                 'source': SOURCE,
```

### Comparing `trytond-7.2.1/trytond/ir/rule.py` & `trytond-7.2.2/trytond/ir/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/rule.xml` & `trytond-7.2.2/trytond/ir/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/sequence.py` & `trytond-7.2.2/trytond/ir/sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/sequence.xml` & `trytond-7.2.2/trytond/ir/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/session.py` & `trytond-7.2.2/trytond/ir/session.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/translation.py` & `trytond-7.2.2/trytond/ir/translation.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/translation.xml` & `trytond-7.2.2/trytond/ir/translation.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/trigger.py` & `trytond-7.2.2/trytond/ir/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/trigger.xml` & `trytond-7.2.2/trytond/ir/trigger.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/board.rnc` & `trytond-7.2.2/trytond/ir/ui/board.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/board.rng` & `trytond-7.2.2/trytond/ir/ui/board.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/calendar.rnc` & `trytond-7.2.2/trytond/ir/ui/calendar.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/calendar.rng` & `trytond-7.2.2/trytond/ir/ui/calendar.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/form.rnc` & `trytond-7.2.2/trytond/ir/ui/form.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/form.rng` & `trytond-7.2.2/trytond/ir/ui/form.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/graph.rnc` & `trytond-7.2.2/trytond/ir/ui/graph.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/graph.rng` & `trytond-7.2.2/trytond/ir/ui/graph.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/icon.py` & `trytond-7.2.2/trytond/ir/ui/icon.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/icon.xml` & `trytond-7.2.2/trytond/ir/ui/icon.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/icons/LICENSE` & `trytond-7.2.2/trytond/ir/ui/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/icons/tryton-settings.svg` & `trytond-7.2.2/trytond/ir/ui/icons/tryton-settings.svg`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/menu.py` & `trytond-7.2.2/trytond/ir/ui/menu.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/menu.xml` & `trytond-7.2.2/trytond/ir/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/tree.rnc` & `trytond-7.2.2/trytond/ir/ui/tree.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/tree.rng` & `trytond-7.2.2/trytond/ir/ui/tree.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/ui.xml` & `trytond-7.2.2/trytond/ir/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/view.py` & `trytond-7.2.2/trytond/ir/ui/view.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/ui/view.xml` & `trytond-7.2.2/trytond/ir/ui/view.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/action_act_window_domain_form.xml` & `trytond-7.2.2/trytond/ir/view/action_act_window_domain_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/action_act_window_form.xml` & `trytond-7.2.2/trytond/ir/view/action_act_window_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/action_form.xml` & `trytond-7.2.2/trytond/ir/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/action_report_form.xml` & `trytond-7.2.2/trytond/ir/view/action_report_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/attachment_form.xml` & `trytond-7.2.2/trytond/ir/view/attachment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/attachment_list.xml` & `trytond-7.2.2/trytond/ir/view/attachment_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/cron_form.xml` & `trytond-7.2.2/trytond/ir/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/cron_list.xml` & `trytond-7.2.2/trytond/ir/view/cron_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/email_form.xml` & `trytond-7.2.2/trytond/ir/view/email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/email_template_form.xml` & `trytond-7.2.2/trytond/ir/view/email_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/error_form.xml` & `trytond-7.2.2/trytond/ir/view/error_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/lang_form.xml` & `trytond-7.2.2/trytond/ir/view/lang_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_access_form.xml` & `trytond-7.2.2/trytond/ir/view/model_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_button_form.xml` & `trytond-7.2.2/trytond/ir/view/model_button_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_button_rule_form.xml` & `trytond-7.2.2/trytond/ir/view/model_button_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_data_form.xml` & `trytond-7.2.2/trytond/ir/view/model_data_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_field_access_form.xml` & `trytond-7.2.2/trytond/ir/view/model_field_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_field_form.xml` & `trytond-7.2.2/trytond/ir/view/model_field_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/model_form.xml` & `trytond-7.2.2/trytond/ir/view/model_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/module_activate_upgrade_start_form.xml` & `trytond-7.2.2/trytond/ir/view/module_activate_upgrade_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/module_form.xml` & `trytond-7.2.2/trytond/ir/view/module_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/module_list.xml` & `trytond-7.2.2/trytond/ir/view/module_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/note_form.xml` & `trytond-7.2.2/trytond/ir/view/note_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/note_list.xml` & `trytond-7.2.2/trytond/ir/view/note_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/rule_group_form.xml` & `trytond-7.2.2/trytond/ir/view/rule_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/sequence_form.xml` & `trytond-7.2.2/trytond/ir/view/sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/translation_form.xml` & `trytond-7.2.2/trytond/ir/view/translation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/translation_list.xml` & `trytond-7.2.2/trytond/ir/view/translation_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/trigger_form.xml` & `trytond-7.2.2/trytond/ir/view/trigger_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/ui_menu_form.xml` & `trytond-7.2.2/trytond/ir/view/ui_menu_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/ui_view_form.xml` & `trytond-7.2.2/trytond/ir/view/ui_view_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/ir/view/ui_view_tree_state_form.xml` & `trytond-7.2.2/trytond/ir/view/ui_view_tree_state_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/__init__.py` & `trytond-7.2.2/trytond/model/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/active.py` & `trytond-7.2.2/trytond/model/active.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/avatar.py` & `trytond-7.2.2/trytond/model/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/descriptors.py` & `trytond-7.2.2/trytond/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/dictschema.py` & `trytond-7.2.2/trytond/model/dictschema.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/digits.py` & `trytond-7.2.2/trytond/model/digits.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/exceptions.py` & `trytond-7.2.2/trytond/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/__init__.py` & `trytond-7.2.2/trytond/model/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/binary.py` & `trytond-7.2.2/trytond/model/fields/binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/boolean.py` & `trytond-7.2.2/trytond/model/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/char.py` & `trytond-7.2.2/trytond/model/fields/char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/date.py` & `trytond-7.2.2/trytond/model/fields/date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/dict.py` & `trytond-7.2.2/trytond/model/fields/dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/field.py` & `trytond-7.2.2/trytond/model/fields/field.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/float.py` & `trytond-7.2.2/trytond/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/fmany2one.py` & `trytond-7.2.2/trytond/model/fields/fmany2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/function.py` & `trytond-7.2.2/trytond/model/fields/function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/many2many.py` & `trytond-7.2.2/trytond/model/fields/many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/many2one.py` & `trytond-7.2.2/trytond/model/fields/many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/multiselection.py` & `trytond-7.2.2/trytond/model/fields/multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/numeric.py` & `trytond-7.2.2/trytond/model/fields/numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/one2many.py` & `trytond-7.2.2/trytond/model/fields/one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/one2one.py` & `trytond-7.2.2/trytond/model/fields/one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/reference.py` & `trytond-7.2.2/trytond/model/fields/reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/selection.py` & `trytond-7.2.2/trytond/model/fields/selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/fields/text.py` & `trytond-7.2.2/trytond/model/fields/text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/match.py` & `trytond-7.2.2/trytond/model/match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/model.py` & `trytond-7.2.2/trytond/model/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/modelsingleton.py` & `trytond-7.2.2/trytond/model/modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/modelsql.py` & `trytond-7.2.2/trytond/model/modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/modelstorage.py` & `trytond-7.2.2/trytond/model/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/modelview.py` & `trytond-7.2.2/trytond/model/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/multivalue.py` & `trytond-7.2.2/trytond/model/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/order.py` & `trytond-7.2.2/trytond/model/order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/symbol.py` & `trytond-7.2.2/trytond/model/symbol.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/tree.py` & `trytond-7.2.2/trytond/model/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/union.py` & `trytond-7.2.2/trytond/model/union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/model/workflow.py` & `trytond-7.2.2/trytond/model/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/modules/__init__.py` & `trytond-7.2.2/trytond/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/pool.py` & `trytond-7.2.2/trytond/pool.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/protocols/dispatcher.py` & `trytond-7.2.2/trytond/protocols/dispatcher.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/protocols/jsonrpc.py` & `trytond-7.2.2/trytond/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/protocols/wrappers.py` & `trytond-7.2.2/trytond/protocols/wrappers.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/protocols/xmlrpc.py` & `trytond-7.2.2/trytond/protocols/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/pyson.py` & `trytond-7.2.2/trytond/pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/report/report.py` & `trytond-7.2.2/trytond/report/report.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/__init__.py` & `trytond-7.2.2/trytond/res/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/email_reset_password.html` & `trytond-7.2.2/trytond/res/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/group.py` & `trytond-7.2.2/trytond/res/group.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/group.xml` & `trytond-7.2.2/trytond/res/group.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/ir.py` & `trytond-7.2.2/trytond/res/ir.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/ir.xml` & `trytond-7.2.2/trytond/res/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/bg.po` & `trytond-7.2.2/trytond/res/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/ca.po` & `trytond-7.2.2/trytond/res/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/cs.po` & `trytond-7.2.2/trytond/res/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/de.po` & `trytond-7.2.2/trytond/res/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/es.po` & `trytond-7.2.2/trytond/res/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/es_419.po` & `trytond-7.2.2/trytond/res/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/et.po` & `trytond-7.2.2/trytond/res/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/fa.po` & `trytond-7.2.2/trytond/res/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/fi.po` & `trytond-7.2.2/trytond/res/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/fr.po` & `trytond-7.2.2/trytond/res/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/hu.po` & `trytond-7.2.2/trytond/res/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/id.po` & `trytond-7.2.2/trytond/res/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/it.po` & `trytond-7.2.2/trytond/res/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/lo.po` & `trytond-7.2.2/trytond/res/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/lt.po` & `trytond-7.2.2/trytond/res/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/nl.po` & `trytond-7.2.2/trytond/res/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/pl.po` & `trytond-7.2.2/trytond/res/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/pt.po` & `trytond-7.2.2/trytond/res/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/ro.po` & `trytond-7.2.2/trytond/res/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/ru.po` & `trytond-7.2.2/trytond/res/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/sl.po` & `trytond-7.2.2/trytond/res/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/tr.po` & `trytond-7.2.2/trytond/res/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/uk.po` & `trytond-7.2.2/trytond/res/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/locale/zh_CN.po` & `trytond-7.2.2/trytond/res/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/message.xml` & `trytond-7.2.2/trytond/res/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/routes.py` & `trytond-7.2.2/trytond/res/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/user.py` & `trytond-7.2.2/trytond/res/user.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/user.xml` & `trytond-7.2.2/trytond/res/user.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/view/group_form.xml` & `trytond-7.2.2/trytond/res/view/group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/view/user_application_form.xml` & `trytond-7.2.2/trytond/res/view/user_application_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/view/user_config_start_form.xml` & `trytond-7.2.2/trytond/res/view/user_config_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/view/user_form.xml` & `trytond-7.2.2/trytond/res/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/res/view/user_form_preferences.xml` & `trytond-7.2.2/trytond/res/view/user_form_preferences.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/rpc.py` & `trytond-7.2.2/trytond/rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/security.py` & `trytond-7.2.2/trytond/security.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/sendmail.py` & `trytond-7.2.2/trytond/sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/status.py` & `trytond-7.2.2/trytond/status.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/__init__.py` & `trytond-7.2.2/trytond/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/access.py` & `trytond-7.2.2/trytond/tests/access.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/copy_.py` & `trytond-7.2.2/trytond/tests/copy_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/export_data.py` & `trytond-7.2.2/trytond/tests/export_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_binary.py` & `trytond-7.2.2/trytond/tests/field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_boolean.py` & `trytond-7.2.2/trytond/tests/field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_char.py` & `trytond-7.2.2/trytond/tests/field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_context.py` & `trytond-7.2.2/trytond/tests/field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_date.py` & `trytond-7.2.2/trytond/tests/field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_datetime.py` & `trytond-7.2.2/trytond/tests/field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_dict.py` & `trytond-7.2.2/trytond/tests/field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_float.py` & `trytond-7.2.2/trytond/tests/field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_function.py` & `trytond-7.2.2/trytond/tests/field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_integer.py` & `trytond-7.2.2/trytond/tests/field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_many2many.py` & `trytond-7.2.2/trytond/tests/field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_many2one.py` & `trytond-7.2.2/trytond/tests/field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_multiselection.py` & `trytond-7.2.2/trytond/tests/field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_numeric.py` & `trytond-7.2.2/trytond/tests/field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_one2many.py` & `trytond-7.2.2/trytond/tests/field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_one2one.py` & `trytond-7.2.2/trytond/tests/field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_reference.py` & `trytond-7.2.2/trytond/tests/field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_selection.py` & `trytond-7.2.2/trytond/tests/field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_text.py` & `trytond-7.2.2/trytond/tests/field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_time.py` & `trytond-7.2.2/trytond/tests/field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/field_timedelta.py` & `trytond-7.2.2/trytond/tests/field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/history.py` & `trytond-7.2.2/trytond/tests/history.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/import_data.py` & `trytond-7.2.2/trytond/tests/import_data.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/import_data.xml` & `trytond-7.2.2/trytond/tests/import_data.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/message.xml` & `trytond-7.2.2/trytond/tests/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/mixin.py` & `trytond-7.2.2/trytond/tests/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/model.py` & `trytond-7.2.2/trytond/tests/model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/model_log.py` & `trytond-7.2.2/trytond/tests/model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/modelsql.py` & `trytond-7.2.2/trytond/tests/modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/modelstorage.py` & `trytond-7.2.2/trytond/tests/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/modelview.py` & `trytond-7.2.2/trytond/tests/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/modelview.xml` & `trytond-7.2.2/trytond/tests/modelview.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/mptt.py` & `trytond-7.2.2/trytond/tests/mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/multivalue.py` & `trytond-7.2.2/trytond/tests/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/path.py` & `trytond-7.2.2/trytond/tests/path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/resource.py` & `trytond-7.2.2/trytond/tests/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/rule.py` & `trytond-7.2.2/trytond/tests/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/sequence.xml` & `trytond-7.2.2/trytond/tests/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_access.py` & `trytond-7.2.2/trytond/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_backend.py` & `trytond-7.2.2/trytond/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_bus.py` & `trytond-7.2.2/trytond/tests/test_bus.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_cache.py` & `trytond-7.2.2/trytond/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_copy.py` & `trytond-7.2.2/trytond/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_exportdata.py` & `trytond-7.2.2/trytond/tests/test_exportdata.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_binary.py` & `trytond-7.2.2/trytond/tests/test_field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_boolean.py` & `trytond-7.2.2/trytond/tests/test_field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_char.py` & `trytond-7.2.2/trytond/tests/test_field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_context.py` & `trytond-7.2.2/trytond/tests/test_field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_date.py` & `trytond-7.2.2/trytond/tests/test_field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_datetime.py` & `trytond-7.2.2/trytond/tests/test_field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_depends.py` & `trytond-7.2.2/trytond/tests/test_field_depends.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_dict.py` & `trytond-7.2.2/trytond/tests/test_field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_float.py` & `trytond-7.2.2/trytond/tests/test_field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_function.py` & `trytond-7.2.2/trytond/tests/test_field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_integer.py` & `trytond-7.2.2/trytond/tests/test_field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_many2many.py` & `trytond-7.2.2/trytond/tests/test_field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_many2one.py` & `trytond-7.2.2/trytond/tests/test_field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_multiselection.py` & `trytond-7.2.2/trytond/tests/test_field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_numeric.py` & `trytond-7.2.2/trytond/tests/test_field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_one2many.py` & `trytond-7.2.2/trytond/tests/test_field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_one2one.py` & `trytond-7.2.2/trytond/tests/test_field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_reference.py` & `trytond-7.2.2/trytond/tests/test_field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_selection.py` & `trytond-7.2.2/trytond/tests/test_field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_text.py` & `trytond-7.2.2/trytond/tests/test_field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_time.py` & `trytond-7.2.2/trytond/tests/test_field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_field_timedelta.py` & `trytond-7.2.2/trytond/tests/test_field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_filestore.py` & `trytond-7.2.2/trytond/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_history.py` & `trytond-7.2.2/trytond/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_i18n.py` & `trytond-7.2.2/trytond/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_importdata.py` & `trytond-7.2.2/trytond/tests/test_importdata.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_ir.py` & `trytond-7.2.2/trytond/tests/test_ir.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_mixins.py` & `trytond-7.2.2/trytond/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_model.py` & `trytond-7.2.2/trytond/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_model_index.py` & `trytond-7.2.2/trytond/tests/test_model_index.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_model_log.py` & `trytond-7.2.2/trytond/tests/test_model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_model_match.py` & `trytond-7.2.2/trytond/tests/test_model_match.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_modelsingleton.py` & `trytond-7.2.2/trytond/tests/test_modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_modelsql.py` & `trytond-7.2.2/trytond/tests/test_modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_modelstorage.py` & `trytond-7.2.2/trytond/tests/test_modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_modelview.py` & `trytond-7.2.2/trytond/tests/test_modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_mptt.py` & `trytond-7.2.2/trytond/tests/test_mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_multivalue.py` & `trytond-7.2.2/trytond/tests/test_multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_order.py` & `trytond-7.2.2/trytond/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_path.py` & `trytond-7.2.2/trytond/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_protocols.py` & `trytond-7.2.2/trytond/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_pyson.py` & `trytond-7.2.2/trytond/tests/test_pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_report.py` & `trytond-7.2.2/trytond/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_res.py` & `trytond-7.2.2/trytond/tests/test_res.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_resource.py` & `trytond-7.2.2/trytond/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_routes.py` & `trytond-7.2.2/trytond/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_rpc.py` & `trytond-7.2.2/trytond/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_rule.py` & `trytond-7.2.2/trytond/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_sendmail.py` & `trytond-7.2.2/trytond/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_sequence.py` & `trytond-7.2.2/trytond/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_tools.py` & `trytond-7.2.2/trytond/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_transaction.py` & `trytond-7.2.2/trytond/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_tree.py` & `trytond-7.2.2/trytond/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_trigger.py` & `trytond-7.2.2/trytond/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_tryton.py` & `trytond-7.2.2/trytond/tests/test_tryton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_union.py` & `trytond-7.2.2/trytond/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_user.py` & `trytond-7.2.2/trytond/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_wizard.py` & `trytond-7.2.2/trytond/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_workflow.py` & `trytond-7.2.2/trytond/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/test_wsgi.py` & `trytond-7.2.2/trytond/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/tools.py` & `trytond-7.2.2/trytond/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/tree.py` & `trytond-7.2.2/trytond/tests/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/trigger.py` & `trytond-7.2.2/trytond/tests/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/wizard.py` & `trytond-7.2.2/trytond/tests/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/wizard.xml` & `trytond-7.2.2/trytond/tests/wizard.xml`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tests/workflow.py` & `trytond-7.2.2/trytond/tests/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/__init__.py` & `trytond-7.2.2/trytond/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/barcode.py` & `trytond-7.2.2/trytond/tools/barcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/decimal_.py` & `trytond-7.2.2/trytond/tools/decimal_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/domain_inversion.py` & `trytond-7.2.2/trytond/tools/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/email_.py` & `trytond-7.2.2/trytond/tools/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/immutabledict.py` & `trytond-7.2.2/trytond/tools/immutabledict.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/logging.py` & `trytond-7.2.2/trytond/tools/logging.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/misc.py` & `trytond-7.2.2/trytond/tools/misc.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/qrcode.py` & `trytond-7.2.2/trytond/tools/qrcode.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/singleton.py` & `trytond-7.2.2/trytond/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/string_.py` & `trytond-7.2.2/trytond/tools/string_.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tools/timezone.py` & `trytond-7.2.2/trytond/tools/timezone.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/transaction.py` & `trytond-7.2.2/trytond/transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tryton.rnc` & `trytond-7.2.2/trytond/tryton.rnc`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/tryton.rng` & `trytond-7.2.2/trytond/tryton.rng`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/url.py` & `trytond-7.2.2/trytond/url.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/wizard/wizard.py` & `trytond-7.2.2/trytond/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/worker.py` & `trytond-7.2.2/trytond/worker.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond/wsgi.py` & `trytond-7.2.2/trytond/wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond.egg-info/PKG-INFO` & `trytond-7.2.2/trytond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-7.2.1/trytond.egg-info/SOURCES.txt` & `trytond-7.2.2/trytond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond-7.2.1/trytond.egg-info/requires.txt` & `trytond-7.2.2/trytond.egg-info/requires.txt`

 * *Files identical despite different names*

