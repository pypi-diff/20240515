# Comparing `tmp/django-payments-payu-1.4.1.tar.gz` & `tmp/django-payments-payu-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-payments-payu-1.4.1.tar", last modified: Tue May 14 08:24:50 2024, max compression
+gzip compressed data, was "django-payments-payu-1.4.2.tar", last modified: Tue May 14 08:28:26 2024, max compression
```

## Comparing `django-payments-payu-1.4.1.tar` & `django-payments-payu-1.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.545273 django-payments-payu-1.4.1/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      349 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.545273 django-payments-payu-1.4.1/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      264 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2530 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      181 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/Makefile
--rw-r--r--   0 petr      (1000) petr      (1000)     9519 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     6133 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/django_payments_payu.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     9519 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      230 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/payments_payu/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/payments_payu/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    29190 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/payments_payu/provider.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      129 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-05-14 08:24:50.553273 django-payments-payu-1.4.1/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      629 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    78613 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/test_payu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      258 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      537 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.384542 django-payments-payu-1.4.2/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      349 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.384542 django-payments-payu-1.4.2/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      264 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2797 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      181 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     9786 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6133 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/django_payments_payu.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     9786 2024-05-14 08:28:26.000000 django-payments-payu-1.4.2/django_payments_payu.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-05-14 08:28:26.000000 django-payments-payu-1.4.2/django_payments_payu.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:28:26.000000 django-payments-payu-1.4.2/django_payments_payu.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:28:26.000000 django-payments-payu-1.4.2/django_payments_payu.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-05-14 08:28:26.000000 django-payments-payu-1.4.2/django_payments_payu.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      230 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/payments_payu/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/payments_payu/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    30384 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/payments_payu/provider.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      129 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-05-14 08:28:26.392542 django-payments-payu-1.4.2/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:26.388542 django-payments-payu-1.4.2/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      629 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    78597 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/test_payu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      258 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      537 2024-05-14 08:28:25.000000 django-payments-payu-1.4.2/tox.ini
```

### Comparing `django-payments-payu-1.4.1/.github/workflows/main.yml` & `django-payments-payu-1.4.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/CONTRIBUTING.rst` & `django-payments-payu-1.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/HISTORY.rst` & `django-payments-payu-1.4.2/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+
+1.4.2 (2024-05-14)
+******************
+* fix multiple deduction of the refund amount from `payment.captured_amount`
+* change statuses of payments refunded with an amount greater than `payment.captured_amount` to `REFUNDED` instead of just deducing `captured_amount`
+
 1.4.1 (2024-05-14)
 ******************
 * fix captured_amount not being saved when processing data
 
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
```

### Comparing `django-payments-payu-1.4.1/LICENSE` & `django-payments-payu-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/Makefile` & `django-payments-payu-1.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/PKG-INFO` & `django-payments-payu-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.4.1
+Version: 1.4.2
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -139,14 +139,20 @@
 
 
 
 
 History
 -------
 
+
+1.4.2 (2024-05-14)
+******************
+* fix multiple deduction of the refund amount from `payment.captured_amount`
+* change statuses of payments refunded with an amount greater than `payment.captured_amount` to `REFUNDED` instead of just deducing `captured_amount`
+
 1.4.1 (2024-05-14)
 ******************
 * fix captured_amount not being saved when processing data
 
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
```

### Comparing `django-payments-payu-1.4.1/README.rst` & `django-payments-payu-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/django_payments_payu.egg-info/PKG-INFO` & `django-payments-payu-1.4.2/django_payments_payu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.4.1
+Version: 1.4.2
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -139,14 +139,20 @@
 
 
 
 
 History
 -------
 
+
+1.4.2 (2024-05-14)
+******************
+* fix multiple deduction of the refund amount from `payment.captured_amount`
+* change statuses of payments refunded with an amount greater than `payment.captured_amount` to `REFUNDED` instead of just deducing `captured_amount`
+
 1.4.1 (2024-05-14)
 ******************
 * fix captured_amount not being saved when processing data
 
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
```

### Comparing `django-payments-payu-1.4.1/django_payments_payu.egg-info/SOURCES.txt` & `django-payments-payu-1.4.2/django_payments_payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/docs/Makefile` & `django-payments-payu-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/docs/conf.py` & `django-payments-payu-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/docs/make.bat` & `django-payments-payu-1.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/payments_payu/provider.py` & `django-payments-payu-1.4.2/payments_payu/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,24 @@
                     refunded_price = dequantize_price(
                         data["refund"]["amount"],
                         data["refund"]["currencyCode"],
                     )
                     print(refunded_price, payment.total)
                     if data["refund"]["status"] == "FINALIZED":
                         payment.message += data["refund"]["reasonDescription"]
-                        if refunded_price == payment.captured_amount:
+                        if refunded_price >= payment.captured_amount:
+                            if refunded_price > payment.captured_amount:
+                                logger.error(
+                                    "refund %s of payment %s has amount greater than the payment's captured_amount: "
+                                    "%f > %f",
+                                    data["refund"].get("refundId", "???"),
+                                    payment.id,
+                                    refunded_price,
+                                    payment.captured_amount,
+                                )
                             payment.change_status(PaymentStatus.REFUNDED)
                         else:
                             payment.captured_amount -= refunded_price
                             payment.save()
                         return HttpResponse("ok", status=200)
                     else:
                         raise Exception("Refund was not finelized", data)
@@ -688,24 +697,35 @@
         if refund_order_id != payment.transaction_id:
             raise NotImplementedError(
                 f"response of refund {refund_id} of payment {payment.id} containing a different order_id "
                 f"not supported yet: {refund_order_id}"
             )
         if refund_status == "CANCELED":
             raise ValueError(f"refund {refund_id} of payment {payment.id} canceled")
-        elif refund_status not in {"PENDING", "FINALIZED"}:
+        elif refund_status == "FINALIZED":
+            raise NotImplementedError(
+                f"refund {refund_id} of payment {payment.id} being FINALIZED already is not supported yet"
+            )
+        elif refund_status not in {"PENDING"}:
             raise PayuApiError(
                 f"invalid status of refund {refund_id} of payment {payment.id}"
             )
         if refund_currency != payment.currency:
             raise NotImplementedError(
                 f"refund {refund_id} of payment {payment.id} in different currency not supported yet: "
                 f"{refund_currency}"
             )
-        return refund_amount
+        if amount is not None and refund_amount != amount:
+            raise NotImplementedError(
+                f"refund {refund_id} of payment {payment.id} having a different amount than requested not supported "
+                f"yet: {refund_amount}"
+            )
+        # Return 0 in order not to change captured_amount yet. If we returned the amount, captured_amount would change
+        # twice (now and once we get a notification from PayU).
+        return Decimal(0)
 
 
 class PaymentProcessor(object):
     "Payment processor"
 
     def __init__(
         self,
```

### Comparing `django-payments-payu-1.4.1/runtests.py` & `django-payments-payu-1.4.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/setup.py` & `django-payments-payu-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/tests/README.md` & `django-payments-payu-1.4.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/tests/settings.py` & `django-payments-payu-1.4.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.1/tests/test_payu.py` & `django-payments-payu-1.4.2/tests/test_payu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1350,15 +1350,15 @@
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
         self.assertEqual(refund_request_mock.call_count, 1)
-        self.assertEqual(amount, Decimal(110))
+        self.assertEqual(amount, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(210))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [payment_extra_data_refund_response_previous, refund_request_response_body],
         )
@@ -1413,15 +1413,15 @@
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment)
 
         self.assertEqual(refund_request_mock.call_count, 1)
-        self.assertEqual(amount, Decimal(220))
+        self.assertEqual(amount, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body],
         )
@@ -1478,15 +1478,15 @@
         with refund_request_patch as refund_request_mock:
             with patch(
                 "uuid.uuid4", return_value="caf231c5-cbc1-4af3-96b7-95798b1cb846"
             ):
                 amount = self.provider.refund(self.payment, Decimal(110))
 
         self.assertEqual(refund_request_mock.call_count, 1)
-        self.assertEqual(amount, Decimal(110))
+        self.assertEqual(amount, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body],
         )
@@ -1540,15 +1540,15 @@
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
         self.assertEqual(refund_request_mock.call_count, 1)
-        self.assertEqual(amount, Decimal(110))
+        self.assertEqual(amount, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body],
         )
@@ -1604,15 +1604,15 @@
 
         with refund_request_patch as refund_request_mock:
             amount1 = self.provider.refund(self.payment, Decimal(200))
             amount2 = self.provider.refund(self.payment, Decimal(200))
 
         self.assertEqual(refund_request_mock.call_count, 2)
         self.assertEqual(amount2, amount1)
-        self.assertEqual(amount2, Decimal(200))
+        self.assertEqual(amount2, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body, refund_request_response_body],
         )
@@ -1622,15 +1622,15 @@
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body, refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
-    def test_refund_finalized(self):
+    def test_refund_pending(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
                 True,
                 True,
                 get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
                 get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
@@ -1644,15 +1644,15 @@
             "refund": {
                 "refundId": "5000009987",
                 "extRefundId": "ext 1234 110",
                 "amount": "11000",
                 "currencyCode": "USD",
                 "description": "desc 1234 110",
                 "creationDateTime": "2020-07-02T09:19:03.896+02:00",
-                "status": "FINALIZED",
+                "status": "PENDING",
                 "statusDateTime": "2020-07-02T09:19:04.013+02:00",
             },
             "status": {
                 "statusCode": "SUCCESS",
                 "statusDesc": "Refund queued for processing",
             },
         }
@@ -1667,15 +1667,15 @@
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
         self.assertEqual(refund_request_mock.call_count, 1)
-        self.assertEqual(amount, Decimal(110))
+        self.assertEqual(amount, Decimal(0))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body],
         )
```

### Comparing `django-payments-payu-1.4.1/tox.ini` & `django-payments-payu-1.4.2/tox.ini`

 * *Files identical despite different names*

