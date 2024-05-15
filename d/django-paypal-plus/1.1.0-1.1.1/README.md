# Comparing `tmp/django-paypal-plus-1.1.0.tar.gz` & `tmp/django-paypal-plus-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-paypal-plus-1.1.0.tar", last modified: Fri Apr 26 10:25:21 2024, max compression
+gzip compressed data, was "django-paypal-plus-1.1.1.tar", last modified: Wed May 15 02:58:30 2024, max compression
```

## Comparing `django-paypal-plus-1.1.0.tar` & `django-paypal-plus-1.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.502114 django-paypal-plus-1.1.0/
--rw-r--r--   0 timtam     (502) staff       (20)     1113 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/LICENSE
--rw-r--r--   0 timtam     (502) staff       (20)       23 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/MANIFEST.in
--rw-r--r--   0 timtam     (502) staff       (20)      975 2024-04-26 10:25:21.501831 django-paypal-plus-1.1.0/PKG-INFO
--rw-r--r--   0 timtam     (502) staff       (20)     2341 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/README.md
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.492431 django-paypal-plus-1.1.0/django_paypal/
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.492783 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/.gitignore
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.493025 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/0.1.15/
--rw-r--r--   0 timtam     (502) staff       (20)      740 2024-04-24 05:35:37.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/0.1.15/10239535276270870560
--rw-r--r--   0 timtam     (502) staff       (20)       43 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.0/django_paypal/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0 timtam     (502) staff       (20)       22 2024-04-26 10:23:00.000000 django-paypal-plus-1.1.0/django_paypal/__init__.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.497383 django-paypal-plus-1.1.0/django_paypal/__pycache__/
--rw-r--r--   0 timtam     (502) staff       (20)      193 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      205 2024-04-26 04:51:50.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      667 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/admin.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    22441 2024-02-05 07:54:49.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    15871 2024-04-24 03:34:04.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      692 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/exceptions.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     8411 2024-04-26 04:51:50.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1614 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1097 2024-04-26 04:51:51.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      348 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/signals.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      362 2024-02-02 06:09:52.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      447 2024-01-31 06:16:42.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     2588 2024-04-26 05:07:15.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/webhooks.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)    15560 2024-02-05 07:54:18.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-311.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     8464 2024-04-26 04:51:51.000000 django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      315 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/admin.py
--rw-r--r--   0 timtam     (502) staff       (20)     9971 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/api_types.py
--rw-r--r--   0 timtam     (502) staff       (20)      207 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/exceptions.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.498825 django-paypal-plus-1.1.0/django_paypal/migrations/
--rw-r--r--   0 timtam     (502) staff       (20)     7840 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0001_initial.py
--rw-r--r--   0 timtam     (502) staff       (20)     1495 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0002_auto_20171002_1551.py
--rw-r--r--   0 timtam     (502) staff       (20)     1573 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0003_auto_20200124_1528.py
--rw-r--r--   0 timtam     (502) staff       (20)     1446 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0004_paypalpayment_related_resource_state.py
--rw-r--r--   0 timtam     (502) staff       (20)     4611 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0005_auto_20240207_0630.py
--rw-r--r--   0 timtam     (502) staff       (20)      755 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/migrations/0006_auto_20240424_0727.py
--rw-r--r--   0 timtam     (502) staff       (20)        0 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__init__.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.500497 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/
--rw-r--r--   0 timtam     (502) staff       (20)     4088 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1162 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1319 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     1347 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     2713 2024-04-24 03:34:09.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      835 2024-04-24 05:27:44.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)      195 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 timtam     (502) staff       (20)     9617 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/models.py
--rw-r--r--   0 timtam     (502) staff       (20)     1304 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/ruff.toml
--rw-r--r--   0 timtam     (502) staff       (20)     1293 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/settings.py
--rw-r--r--   0 timtam     (502) staff       (20)      192 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/signals.py
--rw-r--r--   0 timtam     (502) staff       (20)      174 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/django_paypal/urls.py
--rw-r--r--   0 timtam     (502) staff       (20)      213 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.0/django_paypal/utils.py
--rw-r--r--   0 timtam     (502) staff       (20)     2383 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/webhooks.py
--rw-r--r--   0 timtam     (502) staff       (20)    11435 2024-04-26 10:20:15.000000 django-paypal-plus-1.1.0/django_paypal/wrappers.py
-drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-04-26 10:25:21.501460 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/
--rw-r--r--   0 timtam     (502) staff       (20)      975 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/PKG-INFO
--rw-r--r--   0 timtam     (502) staff       (20)     2343 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/SOURCES.txt
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/dependency_links.txt
--rw-r--r--   0 timtam     (502) staff       (20)        1 2024-02-20 08:20:44.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/not-zip-safe
--rw-r--r--   0 timtam     (502) staff       (20)       73 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/requires.txt
--rw-r--r--   0 timtam     (502) staff       (20)       39 2024-04-26 10:25:21.000000 django-paypal-plus-1.1.0/django_paypal_plus.egg-info/top_level.txt
--rw-r--r--   0 timtam     (502) staff       (20)       38 2024-04-26 10:25:21.502159 django-paypal-plus-1.1.0/setup.cfg
--rwxr-xr-x   0 timtam     (502) staff       (20)     2698 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.0/setup.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.353663 django-paypal-plus-1.1.1/
+-rw-r--r--   0 timtam     (502) staff       (20)     1113 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/LICENSE
+-rw-r--r--   0 timtam     (502) staff       (20)       23 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/MANIFEST.in
+-rw-r--r--   0 timtam     (502) staff       (20)      975 2024-05-15 02:58:30.353431 django-paypal-plus-1.1.1/PKG-INFO
+-rw-r--r--   0 timtam     (502) staff       (20)     3074 2024-05-14 09:01:09.000000 django-paypal-plus-1.1.1/README.md
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.344797 django-paypal-plus-1.1.1/django_paypal/
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.345182 django-paypal-plus-1.1.1/django_paypal/.ruff_cache/
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.1/django_paypal/.ruff_cache/.gitignore
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.345441 django-paypal-plus-1.1.1/django_paypal/.ruff_cache/0.1.15/
+-rw-r--r--   0 timtam     (502) staff       (20)      740 2024-04-24 05:35:37.000000 django-paypal-plus-1.1.1/django_paypal/.ruff_cache/0.1.15/10239535276270870560
+-rw-r--r--   0 timtam     (502) staff       (20)       43 2024-01-30 05:07:59.000000 django-paypal-plus-1.1.1/django_paypal/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0 timtam     (502) staff       (20)       22 2024-05-15 02:58:22.000000 django-paypal-plus-1.1.1/django_paypal/__init__.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.349405 django-paypal-plus-1.1.1/django_paypal/__pycache__/
+-rw-r--r--   0 timtam     (502) staff       (20)      193 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      205 2024-04-29 03:51:12.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      667 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    22441 2024-02-05 07:54:49.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/api_types.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    15871 2024-04-29 03:50:08.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/api_types.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      692 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/exceptions.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     8606 2024-04-29 03:51:12.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1614 2024-02-05 06:09:00.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1109 2024-04-29 03:51:13.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      348 2024-04-24 03:34:05.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/signals.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      362 2024-02-02 06:09:52.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      447 2024-01-31 06:16:42.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     2481 2024-04-29 03:51:13.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/webhooks.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)    15560 2024-02-05 07:54:18.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/wrappers.cpython-311.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     9336 2024-04-30 08:19:37.000000 django-paypal-plus-1.1.1/django_paypal/__pycache__/wrappers.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      315 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/django_paypal/admin.py
+-rw-r--r--   0 timtam     (502) staff       (20)     9971 2024-04-28 17:13:35.000000 django-paypal-plus-1.1.1/django_paypal/api_types.py
+-rw-r--r--   0 timtam     (502) staff       (20)      207 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/django_paypal/exceptions.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.350976 django-paypal-plus-1.1.1/django_paypal/migrations/
+-rw-r--r--   0 timtam     (502) staff       (20)     7840 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0001_initial.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1495 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0002_auto_20171002_1551.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1573 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0003_auto_20200124_1528.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1446 2024-01-30 03:42:26.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0004_paypalpayment_related_resource_state.py
+-rw-r--r--   0 timtam     (502) staff       (20)     4611 2024-04-28 17:13:35.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0005_auto_20240207_0630.py
+-rw-r--r--   0 timtam     (502) staff       (20)      755 2024-04-29 03:51:11.000000 django-paypal-plus-1.1.1/django_paypal/migrations/0006_auto_20240424_0727.py
+-rw-r--r--   0 timtam     (502) staff       (20)        0 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__init__.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.352176 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/
+-rw-r--r--   0 timtam     (502) staff       (20)     4088 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1162 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1319 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     1347 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     2713 2024-04-29 03:50:12.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      835 2024-04-29 03:51:14.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)      195 2024-01-31 07:22:43.000000 django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 timtam     (502) staff       (20)     9617 2024-04-29 03:51:11.000000 django-paypal-plus-1.1.1/django_paypal/models.py
+-rw-r--r--   0 timtam     (502) staff       (20)     1304 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/django_paypal/ruff.toml
+-rw-r--r--   0 timtam     (502) staff       (20)     1293 2024-04-29 03:51:11.000000 django-paypal-plus-1.1.1/django_paypal/settings.py
+-rw-r--r--   0 timtam     (502) staff       (20)      192 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/django_paypal/signals.py
+-rw-r--r--   0 timtam     (502) staff       (20)      174 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/django_paypal/urls.py
+-rw-r--r--   0 timtam     (502) staff       (20)      213 2024-01-30 03:41:51.000000 django-paypal-plus-1.1.1/django_paypal/utils.py
+-rw-r--r--   0 timtam     (502) staff       (20)     2423 2024-05-15 02:58:22.000000 django-paypal-plus-1.1.1/django_paypal/webhooks.py
+-rw-r--r--   0 timtam     (502) staff       (20)    11435 2024-04-30 08:19:35.000000 django-paypal-plus-1.1.1/django_paypal/wrappers.py
+drwxr-xr-x   0 timtam     (502) staff       (20)        0 2024-05-15 02:58:30.353181 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/
+-rw-r--r--   0 timtam     (502) staff       (20)      975 2024-05-15 02:58:30.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/PKG-INFO
+-rw-r--r--   0 timtam     (502) staff       (20)     2343 2024-05-15 02:58:30.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-05-15 02:58:30.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 timtam     (502) staff       (20)        1 2024-02-20 08:20:44.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/not-zip-safe
+-rw-r--r--   0 timtam     (502) staff       (20)       73 2024-05-15 02:58:30.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/requires.txt
+-rw-r--r--   0 timtam     (502) staff       (20)       39 2024-05-15 02:58:30.000000 django-paypal-plus-1.1.1/django_paypal_plus.egg-info/top_level.txt
+-rw-r--r--   0 timtam     (502) staff       (20)       38 2024-05-15 02:58:30.353701 django-paypal-plus-1.1.1/setup.cfg
+-rwxr-xr-x   0 timtam     (502) staff       (20)     2698 2024-04-23 04:40:19.000000 django-paypal-plus-1.1.1/setup.py
```

### Comparing `django-paypal-plus-1.1.0/LICENSE` & `django-paypal-plus-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/PKG-INFO` & `django-paypal-plus-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-paypal-plus
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django integration of PayPal's Orders v2 API
 Home-page: https://github.com/ParticulateSolutions/django-paypal-plus
 Author: Particulate Solutions GmbH
 Author-email: tech@particulate.me
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/.ruff_cache/0.1.15/10239535276270870560` & `django-paypal-plus-1.1.1/django_paypal/.ruff_cache/0.1.15/10239535276270870560`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/admin.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/admin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-311.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/api_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/api_types.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/api_types.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 23 04:40:19 2024 UTC, .py size: 9971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b33b 2766 f326 0000  U........;'f.&..
+00000000: 550d 0d0a 0000 0000 bf83 2e66 f326 0000  U..........f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e203 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6505 6404 1900 5a0b 6505  m.Z...e.d...Z.e.
 00000070: 6405 1900 5a0c 6505 6406 1900 5a0d 6501  d...Z.e.d...Z.e.
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/exceptions.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/exceptions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/models.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 26 04:47:09 2024 UTC, .py size: 9481 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,526 +1,538 @@
-00000000: 550d 0d0a 0000 0000 cd31 2b66 0925 0000  U........1+f.%..
+00000000: 550d 0d0a 0000 0000 2f19 2f66 9125 0000  U......././f.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 1a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 6d0f 5a0f 0100 7a10 6400 6408 6c10 6d11  m.Z...z.d.d.l.m.
-00000090: 5a11 0100 5700 6e20 0400 6512 6b0a 7288  Z...W.n ..e.k.r.
-000000a0: 0100 0100 0100 6400 6408 6c13 6d11 5a11  ......d.d.l.m.Z.
-000000b0: 0100 5900 6e02 5800 4700 6409 640a 8400  ..Y.n.X.G.d.d...
-000000c0: 640a 6509 6a14 8303 5a15 4700 640b 640c  d.e.j...Z.G.d.d.
-000000d0: 8400 640c 6509 6a14 8303 5a16 4700 640d  ..d.e.j...Z.G.d.
-000000e0: 640e 8400 640e 6509 6a14 8303 5a17 4700  d...d.e.j...Z.G.
-000000f0: 640f 6410 8400 6410 6509 6a14 8303 5a18  d.d...d.e.j...Z.
-00000100: 4700 6411 6412 8400 6412 6509 6a14 8303  G.d.d...d.e.j...
-00000110: 5a19 4700 6413 6414 8400 6414 6509 6a14  Z.G.d.d...d.e.j.
-00000120: 8303 5a1a 4700 6415 6416 8400 6416 6509  ..Z.G.d.d...d.e.
-00000130: 6a14 8303 5a1b 4700 6417 6418 8400 6418  j...Z.G.d.d...d.
-00000140: 6509 6a14 8303 5a1c 6419 5300 291a e900  e.j...Z.d.S.)...
-00000150: 0000 0029 01da 1075 6e69 636f 6465 5f6c  ...)...unicode_l
-00000160: 6974 6572 616c 7329 01da 0744 6563 696d  iterals)...Decim
-00000170: 616c 2901 da04 4c69 7374 2901 da08 6672  al)...List)...fr
-00000180: 6f6d 6469 6374 2901 da06 6d6f 6465 6c73  omdict)...models
-00000190: 2901 da0c 6765 7474 6578 745f 6c61 7a79  )...gettext_lazy
-000001a0: 2902 da19 5365 6c6c 6572 5265 6365 6976  )...SellerReceiv
-000001b0: 6162 6c65 4272 6561 6b64 6f77 6eda 0743  ableBreakdown..C
-000001c0: 6170 7475 7265 2901 da09 4a53 4f4e 4669  apture)...JSONFi
-000001d0: 656c 6463 0000 0000 0000 0000 0000 0000  eldc............
-000001e0: 0000 0000 0500 0000 4000 0000 735a 0000  ........@...sZ..
-000001f0: 0065 005a 0164 005a 0265 036a 0465 0564  .e.Z.d.Z.e.j.e.d
-00000200: 0183 0164 0264 0364 048d 035a 0665 036a  ...d.d.d...Z.e.j
-00000210: 0465 0564 0583 0164 0264 0364 068d 035a  .e.d...d.d.d...Z
-00000220: 0765 036a 0864 079c 0164 0864 0984 045a  .e.j.d...d.d...Z
-00000230: 0965 0a65 0b65 0c19 0064 079c 0164 0a64  .e.e.e...d...d.d
-00000240: 0b84 0483 015a 0d64 0c53 0029 0dda 0b50  .....Z.d.S.)...P
-00000250: 6179 7061 6c4f 7264 6572 7a08 4f72 6465  aypalOrderz.Orde
-00000260: 7220 4944 e9ff 0000 0054 a902 da0a 6d61  r ID.....T....ma
-00000270: 785f 6c65 6e67 7468 da06 756e 6971 7565  x_length..unique
-00000280: 5a06 5374 6174 7573 a902 720e 0000 00da  Z.Status..r.....
-00000290: 0562 6c61 6e6b 2901 da06 7265 7475 726e  .blank)...return
-000002a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000002b0: 0004 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-000002c0: 6a00 6a01 6401 7c00 6a02 9b00 6402 9d03  j.j.d.|.j...d...
-000002d0: 6403 8d01 5300 2904 4e7a 142f 7632 2f63  d...S.).Nz./v2/c
-000002e0: 6865 636b 6f75 742f 6f72 6465 7273 2f7a  heckout/orders/z
-000002f0: 082f 6361 7074 7572 6529 015a 0d75 726c  ./capture).Z.url
-00000300: 5f5f 636f 6e74 6169 6e73 2903 da0d 6170  __contains)...ap
-00000310: 695f 7265 7370 6f6e 7365 73da 0666 696c  i_responses..fil
-00000320: 7465 72da 086f 7264 6572 5f69 64a9 01da  ter..order_id...
-00000330: 0473 656c 66a9 0072 1800 0000 fa5b 2f55  .self..r.....[/U
-00000340: 7365 7273 2f74 696d 7461 6d2f 2e70 7965  sers/timtam/.pye
-00000350: 6e76 2f76 6572 7369 6f6e 732f 7366 2d33  nv/versions/sf-3
-00000360: 2e38 2e31 322f 6c69 622f 7079 7468 6f6e  .8.12/lib/python
-00000370: 332e 382f 7369 7465 2d70 6163 6b61 6765  3.8/site-package
-00000380: 732f 646a 616e 676f 5f70 6179 7061 6c2f  s/django_paypal/
-00000390: 6d6f 6465 6c73 2e70 79da 1967 6574 5f63  models.py..get_c
-000003a0: 6170 7475 7265 5f61 7069 5f72 6573 706f  apture_api_respo
-000003b0: 6e73 6573 1900 0000 7302 0000 0000 017a  nses....s......z
-000003c0: 2550 6179 7061 6c4f 7264 6572 2e67 6574  %PaypalOrder.get
-000003d0: 5f63 6170 7475 7265 5f61 7069 5f72 6573  _capture_api_res
-000003e0: 706f 6e73 6573 6301 0000 0000 0000 0000  ponsesc.........
-000003f0: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00000400: 5600 0000 7400 8300 7d01 7c00 a001 a100  V...t...}.|.....
-00000410: 4400 5d42 7d02 7c02 6a02 a003 6401 6700  D.]B}.|.j...d.g.
-00000420: a102 4400 5d2e 7d03 7c03 a003 6402 6900  ..D.].}.|...d.i.
-00000430: a102 a003 6403 6700 a102 4400 5d14 7d04  ....d.g...D.].}.
-00000440: 7c01 a004 7405 7406 7c04 8302 a101 0100  |...t.t.|.......
-00000450: 7138 7120 710e 7c01 5300 2904 4e5a 0e70  q8q q.|.S.).NZ.p
-00000460: 7572 6368 6173 655f 756e 6974 735a 0870  urchase_unitsZ.p
-00000470: 6179 6d65 6e74 73da 0863 6170 7475 7265  ayments..capture
-00000480: 7329 07da 046c 6973 7472 1a00 0000 da0d  s)...listr......
-00000490: 7265 7370 6f6e 7365 5f64 6174 61da 0367  response_data..g
-000004a0: 6574 da06 6170 7065 6e64 7205 0000 0072  et..appendr....r
-000004b0: 0900 0000 2905 7217 0000 0072 1b00 0000  ....).r....r....
-000004c0: da10 6361 7074 7572 655f 7265 7370 6f6e  ..capture_respon
-000004d0: 7365 5a0d 7075 7263 6861 7365 5f75 6e69  seZ.purchase_uni
-000004e0: 74da 0763 6170 7475 7265 7218 0000 0072  t..capturer....r
-000004f0: 1800 0000 7219 0000 0072 1b00 0000 1c00  ....r....r......
-00000500: 0000 730c 0000 0000 0206 010c 0112 0118  ..s.............
-00000510: 0116 017a 1450 6179 7061 6c4f 7264 6572  ...z.PaypalOrder
-00000520: 2e63 6170 7475 7265 734e 290e da08 5f5f  .capturesN)...__
-00000530: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000540: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000550: 7206 0000 00da 0943 6861 7246 6965 6c64  r......CharField
-00000560: da01 5f72 1500 0000 da06 7374 6174 7573  .._r......status
-00000570: da08 5175 6572 7953 6574 721a 0000 00da  ..QuerySetr.....
-00000580: 0870 726f 7065 7274 7972 0400 0000 7209  .propertyr....r.
-00000590: 0000 0072 1b00 0000 7218 0000 0072 1800  ...r....r....r..
-000005a0: 0000 7218 0000 0072 1900 0000 720b 0000  ..r....r....r...
-000005b0: 0015 0000 0073 0a00 0000 0801 1401 1402  .....s..........
-000005c0: 1003 0201 720b 0000 0063 0000 0000 0000  ....r....c......
-000005d0: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
-000005e0: 0000 734a 0000 0065 005a 0164 005a 0265  ..sJ...e.Z.d.Z.e
-000005f0: 036a 0465 0564 0165 036a 0664 028d 035a  .j.e.d.e.j.d...Z
-00000600: 0765 036a 0865 0964 0383 0164 0464 0564  .e.j.e.d...d.d.d
-00000610: 068d 035a 0a65 0b65 0964 0783 0183 015a  ...Z.e.e.d.....Z
-00000620: 0c65 036a 0d64 0564 088d 015a 0e64 0953  .e.j.d.d...Z.d.S
-00000630: 0029 0ada 1150 6179 7061 6c41 5049 506f  .)...PaypalAPIPo
-00000640: 7374 4461 7461 5a09 6170 695f 706f 7374  stDataZ.api_post
-00000650: 73a9 02da 0c72 656c 6174 6564 5f6e 616d  s....related_nam
-00000660: 65da 096f 6e5f 6465 6c65 7465 da03 5552  e..on_delete..UR
-00000670: 4c72 0c00 0000 5472 1000 0000 7a09 506f  Lr....Tr....z.Po
-00000680: 7374 2044 6174 61a9 01da 0c61 7574 6f5f  st Data....auto_
-00000690: 6e6f 775f 6164 644e 290f 7222 0000 0072  now_addN).r"...r
-000006a0: 2300 0000 7224 0000 0072 0600 0000 da0a  #...r$...r......
-000006b0: 466f 7265 6967 6e4b 6579 720b 0000 00da  ForeignKeyr.....
-000006c0: 0743 4153 4341 4445 da05 6f72 6465 7272  .CASCADE..orderr
-000006d0: 2500 0000 7226 0000 00da 0375 726c 720a  %...r&.....urlr.
-000006e0: 0000 00da 0970 6f73 745f 6461 7461 da0d  .....post_data..
-000006f0: 4461 7465 5469 6d65 4669 656c 64da 0a63  DateTimeField..c
-00000700: 7265 6174 6564 5f61 7472 1800 0000 7218  reated_atr....r.
-00000710: 0000 0072 1800 0000 7219 0000 0072 2a00  ...r....r....r*.
-00000720: 0000 2600 0000 7308 0000 0008 0112 0114  ..&...s.........
-00000730: 010c 0172 2a00 0000 6300 0000 0000 0000  ...r*...c.......
-00000740: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00000750: 0073 5e00 0000 6500 5a01 6400 5a02 6503  .s^...e.Z.d.Z.e.
-00000760: 6a04 6505 6401 6503 6a06 6402 8d03 5a07  j.e.d.e.j.d...Z.
-00000770: 6503 6a04 6508 6403 6404 6503 6a06 6405  e.j.e.d.d.e.j.d.
-00000780: 8d04 5a09 6503 6a0a 650b 6406 8301 6407  ..Z.e.j.e.d...d.
-00000790: 6404 6408 8d03 5a0c 650d 650b 6409 8301  d.d...Z.e.e.d...
-000007a0: 8301 5a0e 6503 6a0f 6404 640a 8d01 5a10  ..Z.e.j.d.d...Z.
-000007b0: 640b 5300 290c da11 5061 7970 616c 4150  d.S.)...PaypalAP
-000007c0: 4952 6573 706f 6e73 6572 1300 0000 722b  IResponser....r+
-000007d0: 0000 00da 0972 6573 706f 6e73 6573 5429  .....responsesT)
-000007e0: 0372 2c00 0000 da04 6e75 6c6c 722d 0000  .r,.....nullr-..
-000007f0: 0072 2e00 0000 720c 0000 0072 1000 0000  .r....r....r....
-00000800: 7a0d 5265 7370 6f6e 7365 2044 6174 6172  z.Response Datar
-00000810: 2f00 0000 4e29 1172 2200 0000 7223 0000  /...N).r"...r#..
-00000820: 0072 2400 0000 7206 0000 0072 3100 0000  .r$...r....r1...
-00000830: 720b 0000 0072 3200 0000 7233 0000 0072  r....r2...r3...r
-00000840: 2a00 0000 da04 706f 7374 7225 0000 0072  *.....postr%...r
-00000850: 2600 0000 7234 0000 0072 0a00 0000 721d  &...r4...r....r.
-00000860: 0000 0072 3600 0000 7237 0000 0072 1800  ...r6...r7...r..
-00000870: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000880: 0072 3800 0000 2d00 0000 730a 0000 0008  .r8...-...s.....
-00000890: 0112 0114 0114 010c 0172 3800 0000 6300  .........r8...c.
-000008a0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000008b0: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
-000008c0: 6400 5a02 6503 6a04 6505 6401 8301 6402  d.Z.e.j.e.d...d.
-000008d0: 6403 6404 8d03 5a06 6503 6a04 6405 6402  d.d...Z.e.j.d.d.
-000008e0: 6403 6404 8d03 5a07 6508 6505 6406 8301  d.d...Z.e.e.d...
-000008f0: 8301 5a09 6407 5300 2908 da0d 5061 7970  ..Z.d.S.)...Payp
-00000900: 616c 5765 6268 6f6f 6b7a 0a57 6562 686f  alWebhookz.Webho
-00000910: 6f6b 2049 4472 0c00 0000 5472 0d00 0000  ok IDr....Tr....
-00000920: 722e 0000 007a 1541 6374 6976 6520 5765  r....z.Active We
-00000930: 6268 6f6f 6b20 4576 656e 7473 4e29 0a72  bhook EventsN).r
-00000940: 2200 0000 7223 0000 0072 2400 0000 7206  "...r#...r$...r.
-00000950: 0000 0072 2500 0000 7226 0000 005a 0a77  ...r%...r&...Z.w
-00000960: 6562 686f 6f6b 5f69 6472 3400 0000 720a  ebhook_idr4...r.
-00000970: 0000 005a 0b65 7665 6e74 5f74 7970 6573  ...Z.event_types
-00000980: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000990: 1900 0000 723c 0000 0035 0000 0073 0600  ....r<...5...s..
-000009a0: 0000 0801 1401 1001 723c 0000 0063 0000  ........r<...c..
-000009b0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
-000009c0: 0000 4000 0000 733c 0000 0065 005a 0164  ..@...s<...e.Z.d
-000009d0: 005a 0265 0365 0464 0183 0183 015a 0565  .Z.e.e.d.....Z.e
-000009e0: 066a 0765 0864 0265 066a 0964 038d 035a  .j.e.d.e.j.d...Z
-000009f0: 0a65 066a 0765 0b64 0465 066a 0964 038d  .e.j.e.d.e.j.d..
-00000a00: 035a 0c64 0553 0029 06da 1250 6179 7061  .Z.d.S.)...Paypa
-00000a10: 6c57 6562 686f 6f6b 4576 656e 745a 0750  lWebhookEventZ.P
-00000a20: 6179 6c6f 6164 5a0e 7765 6268 6f6f 6b5f  ayloadZ.webhook_
-00000a30: 6576 656e 7473 722b 0000 00da 0665 7665  eventsr+.....eve
-00000a40: 6e74 734e 290d 7222 0000 0072 2300 0000  ntsN).r"...r#...
-00000a50: 7224 0000 0072 0a00 0000 7226 0000 00da  r$...r....r&....
-00000a60: 0770 6179 6c6f 6164 7206 0000 0072 3100  .payloadr....r1.
-00000a70: 0000 720b 0000 0072 3200 0000 7233 0000  ..r....r2...r3..
-00000a80: 0072 3c00 0000 5a07 7765 6268 6f6f 6b72  .r<...Z.webhookr
-00000a90: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00000aa0: 0000 0072 3d00 0000 3b00 0000 7306 0000  ...r=...;...s...
-00000ab0: 0008 010c 0112 0172 3d00 0000 6300 0000  .......r=...c...
-00000ac0: 0000 0000 0000 0000 0000 0000 0006 0000  ................
-00000ad0: 0040 0000 0073 a401 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000ae0: 5a02 6503 6a04 6505 6401 8301 6402 6403  Z.e.j.e.d...d.d.
-00000af0: 6404 8d03 5a06 6503 6a04 6505 6405 8301  d...Z.e.j.e.d...
-00000b00: 6402 6406 8d02 5a07 6503 6a04 6505 6405  d.d...Z.e.j.e.d.
-00000b10: 8301 6402 6403 6407 8d03 5a08 6503 6a04  ..d.d.d...Z.e.j.
-00000b20: 6505 6405 8301 6408 6403 6407 8d03 5a09  e.d...d.d.d...Z.
-00000b30: 6503 6a04 6505 6409 8301 6402 6403 6407  e.j.e.d...d.d.d.
-00000b40: 8d03 5a0a 6503 6a04 6505 640a 8301 6402  ..Z.e.j.e.d...d.
-00000b50: 6403 6407 8d03 5a0b 6503 6a04 6505 640a  d.d...Z.e.j.e.d.
-00000b60: 8301 6402 6403 6407 8d03 5a0c 6503 6a04  ..d.d.d...Z.e.j.
-00000b70: 6505 640b 8301 6402 6403 6407 8d03 5a0d  e.d...d.d.d...Z.
-00000b80: 6503 6a0e 6505 640c 8301 640d 640e 650f  e.j.e.d...d.d.e.
-00000b90: 640f 8301 6410 8d04 5a10 6503 6a04 6505  d...d...Z.e.j.e.
-00000ba0: 6411 8301 6402 6403 6403 6412 8d04 5a11  d...d.d.d.d...Z.
-00000bb0: 6503 6a04 6505 6413 8301 6402 6403 6403  e.j.e.d...d.d.d.
-00000bc0: 6412 8d04 5a12 6503 6a13 6505 6414 8301  d...Z.e.j.e.d...
-00000bd0: 6403 6403 6415 8d03 5a14 6503 6a13 6505  d.d.d...Z.e.j.e.
-00000be0: 6416 8301 6403 6403 6415 8d03 5a15 6503  d...d.d.d...Z.e.
-00000bf0: 6a04 6505 6417 8301 6402 6403 6407 8d03  j.e.d...d.d.d...
-00000c00: 5a16 6503 6a17 6505 6418 8301 6403 6419  Z.e.j.e.d...d.d.
-00000c10: 8d02 5a18 6503 6a17 6505 641a 8301 6403  ..Z.e.j.e.d...d.
-00000c20: 6419 8d02 5a19 6503 6a17 6505 641b 8301  d...Z.e.j.e.d...
-00000c30: 6403 6419 8d02 5a1a 6503 6a1b 6505 641c  d.d...Z.e.j.e.d.
-00000c40: 8301 6403 641d 8d02 5a1c 6503 6a1b 6505  ..d.d...Z.e.j.e.
-00000c50: 641e 8301 6403 641f 8d02 5a1d 6503 a01e  d...d.d...Z.e...
-00000c60: a100 5a1f 6420 6421 8400 5a20 4700 6422  ..Z.d d!..Z G.d"
-00000c70: 6423 8400 6423 8302 5a21 6424 5300 2925  d#..d#..Z!d$S.)%
-00000c80: da13 4c65 6761 6379 5061 7970 616c 5061  ..LegacyPaypalPa
-00000c90: 796d 656e 747a 0a70 6179 6d65 6e74 2069  ymentz.payment i
-00000ca0: 6472 0c00 0000 5472 0d00 0000 da06 696e  dr....Tr......in
-00000cb0: 7465 6e74 a901 720e 0000 0072 1000 0000  tent..r....r....
-00000cc0: e9a5 0000 00da 0573 7461 7465 7a0e 7061  .......statez.pa
-00000cd0: 796d 656e 7420 6d65 7468 6f64 7a08 7061  yment methodz.pa
-00000ce0: 7965 7220 6964 7a0f 7472 616e 7361 6374  yer idz.transact
-00000cf0: 696f 6e20 6665 65e9 0900 0000 e902 0000  ion fee.........
-00000d00: 0072 0100 0000 2903 da0a 6d61 785f 6469  .r....)...max_di
-00000d10: 6769 7473 da0e 6465 6369 6d61 6c5f 706c  gits..decimal_pl
-00000d20: 6163 6573 da07 6465 6661 756c 747a 1372  aces..defaultz.r
-00000d30: 656c 6174 6564 2072 6573 6f75 7263 6520  elated resource 
-00000d40: 6964 2903 720e 0000 0072 1100 0000 723a  id).r....r....r:
-00000d50: 0000 007a 1672 656c 6174 6564 2072 6573  ...z.related res
-00000d60: 6f75 7263 6520 7374 6174 657a 1569 6e69  ource statez.ini
-00000d70: 7469 616c 2070 6f73 7420 7265 7370 6f6e  tial post respon
-00000d80: 7365 2902 723a 0000 0072 1100 0000 7a14  se).r:...r....z.
-00000d90: 7570 6461 7465 6420 6765 7420 7265 7370  updated get resp
-00000da0: 6f6e 7365 7a0e 6661 696c 7572 6520 7265  onsez.failure re
-00000db0: 6173 6f6e da04 6c69 6e6b a901 7211 0000  ason..link..r...
-00000dc0: 007a 0c61 7070 726f 7665 206c 696e 6b7a  .z.approve linkz
-00000dd0: 0c65 7865 6375 7465 206c 696e 6bfa 0a63  .execute link..c
-00000de0: 7265 6174 6564 2061 7472 2f00 0000 fa0d  reated atr/.....
-00000df0: 6c61 7374 206d 6f64 6966 6965 64a9 01da  last modified...
-00000e00: 0861 7574 6f5f 6e6f 7763 0100 0000 0000  .auto_nowc......
-00000e10: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000e20: 0000 7306 0000 007c 006a 0053 00a9 014e  ..s....|.j.S...N
-00000e30: 2901 da0a 7061 796d 656e 745f 6964 7216  )...payment_idr.
-00000e40: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000e50: 0000 da07 5f5f 7374 725f 5f5e 0000 0073  ....__str__^...s
-00000e60: 0200 0000 0001 7a1b 4c65 6761 6379 5061  ......z.LegacyPa
-00000e70: 7970 616c 5061 796d 656e 742e 5f5f 7374  ypalPayment.__st
-00000e80: 725f 5f63 0000 0000 0000 0000 0000 0000  r__c............
-00000e90: 0000 0000 0200 0000 4000 0000 731c 0000  ........@...s...
-00000ea0: 0065 005a 0164 005a 0265 0364 0183 015a  .e.Z.d.Z.e.d...Z
-00000eb0: 0465 0364 0283 015a 0564 0353 0029 047a  .e.d...Z.d.S.).z
-00000ec0: 184c 6567 6163 7950 6179 7061 6c50 6179  .LegacyPaypalPay
-00000ed0: 6d65 6e74 2e4d 6574 617a 274c 6567 6163  ment.Metaz'Legac
-00000ee0: 7920 5061 7970 616c 2050 6179 6d65 6e74  y Paypal Payment
-00000ef0: 2028 7061 796d 656e 7473 2076 3120 4150   (payments v1 AP
-00000f00: 4929 7a28 4c65 6761 6379 2050 6179 7061  I)z(Legacy Paypa
-00000f10: 6c20 5061 796d 656e 7473 2028 7061 796d  l Payments (paym
-00000f20: 656e 7473 2076 3120 4150 4929 4ea9 0672  ents v1 API)N..r
-00000f30: 2200 0000 7223 0000 0072 2400 0000 7226  "...r#...r$...r&
-00000f40: 0000 00da 0c76 6572 626f 7365 5f6e 616d  .....verbose_nam
-00000f50: 65da 1376 6572 626f 7365 5f6e 616d 655f  e..verbose_name_
-00000f60: 706c 7572 616c 7218 0000 0072 1800 0000  pluralr....r....
-00000f70: 7218 0000 0072 1900 0000 da04 4d65 7461  r....r......Meta
-00000f80: 6100 0000 7304 0000 0008 0108 0172 5600  a...s........rV.
-00000f90: 0000 4e29 2272 2200 0000 7223 0000 0072  ..N)"r"...r#...r
-00000fa0: 2400 0000 7206 0000 0072 2500 0000 7226  $...r....r%...r&
-00000fb0: 0000 0072 5100 0000 7241 0000 005a 1565  ...rQ...rA...Z.e
-00000fc0: 7870 6572 6965 6e63 655f 7072 6f66 696c  xperience_profil
-00000fd0: 655f 6964 5a0d 6e6f 7465 5f74 6f5f 7061  e_idZ.note_to_pa
-00000fe0: 7965 7272 4400 0000 5a0e 7061 796d 656e  yerrD...Z.paymen
-00000ff0: 745f 6d65 7468 6f64 da06 6375 7374 6f6d  t_method..custom
-00001000: 5a08 7061 7965 725f 6964 da0c 4465 6369  Z.payer_id..Deci
-00001010: 6d61 6c46 6965 6c64 7203 0000 005a 0f74  malFieldr....Z.t
-00001020: 7261 6e73 6163 7469 6f6e 5f66 6565 5a13  ransaction_feeZ.
-00001030: 7265 6c61 7465 645f 7265 736f 7572 6365  related_resource
-00001040: 5f69 645a 1672 656c 6174 6564 5f72 6573  _idZ.related_res
-00001050: 6f75 7263 655f 7374 6174 65da 0954 6578  ource_state..Tex
-00001060: 7446 6965 6c64 5a17 696e 6974 6961 6c5f  tFieldZ.initial_
-00001070: 7265 7370 6f6e 7365 5f6f 626a 6563 745a  response_objectZ
-00001080: 1675 7064 6174 655f 7265 7370 6f6e 7365  .update_response
-00001090: 5f6f 626a 6563 745a 0e66 6169 6c75 7265  _objectZ.failure
-000010a0: 5f72 6561 736f 6eda 0855 524c 4669 656c  _reason..URLFiel
-000010b0: 6472 4a00 0000 da0c 6170 7072 6f76 655f  drJ.....approve_
-000010c0: 6c69 6e6b 5a0c 6578 6563 7574 655f 6c69  linkZ.execute_li
-000010d0: 6e6b 7236 0000 0072 3700 0000 da0d 6c61  nkr6...r7.....la
-000010e0: 7374 5f6d 6f64 6966 6965 64da 074d 616e  st_modified..Man
-000010f0: 6167 6572 da07 6f62 6a65 6374 7372 5200  ager..objectsrR.
-00001100: 0000 7256 0000 0072 1800 0000 7218 0000  ..rV...r....r...
-00001110: 0072 1800 0000 7219 0000 0072 4000 0000  .r....r....r@...
-00001120: 4400 0000 732c 0000 0008 0114 0112 0114  D...s,..........
-00001130: 0114 0114 0114 0114 0114 011a 0116 0116  ................
-00001140: 0114 0114 0214 0212 0112 0112 0212 0112  ................
-00001150: 0208 0208 0372 4000 0000 6300 0000 0000  .....r@...c.....
-00001160: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
-00001170: 0000 0073 b802 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001180: 6503 6a04 6505 6506 6401 8301 6402 6503  e.j.e.e.d...d.e.
-00001190: 6a07 6403 8d04 5a08 6503 6a09 6506 6404  j.d...Z.e.j.e.d.
-000011a0: 8301 6405 6406 6407 8d03 5a0a 6503 6a0b  ..d.d.d...Z.e.j.
-000011b0: 6506 6408 8301 6409 640a 8d02 5a0c 6503  e.d...d.d...Z.e.
-000011c0: 6a09 6506 640b 8301 6405 6406 6407 8d03  j.e.d...d.d.d...
-000011d0: 5a0d 6503 6a09 6506 640c 8301 6405 6406  Z.e.j.e.d...d.d.
-000011e0: 640d 640e 8d04 5a0e 6503 6a09 6506 640f  d.d...Z.e.j.e.d.
-000011f0: 8301 6405 6406 640d 640e 8d04 5a0f 6503  ..d.d.d.d...Z.e.
-00001200: 6a09 6506 6410 8301 6405 6406 640d 640e  j.e.d...d.d.d.d.
-00001210: 8d04 5a10 6503 6a09 6506 6411 8301 6405  ..Z.e.j.e.d...d.
-00001220: 6406 640d 640e 8d04 5a11 6503 6a09 6506  d.d.d...Z.e.j.e.
-00001230: 6412 8301 6405 6406 640d 640e 8d04 5a12  d...d.d.d.d...Z.
-00001240: 6503 6a09 6506 6413 8301 6405 6406 640d  e.j.e.d...d.d.d.
-00001250: 640e 8d04 5a13 6503 6a0b 6506 6414 8301  d...Z.e.j.e.d...
-00001260: 6415 640d 6416 8d03 5a14 6503 6a0b 6506  d.d.d...Z.e.j.e.
-00001270: 6417 8301 6415 6418 6419 8d03 5a15 6503  d...d.d.d...Z.e.
-00001280: 6a0b 6506 641a 8301 6415 641b 6419 8d03  j.e.d...d.d.d...
-00001290: 5a16 6503 6a0b 6506 641c 8301 6415 640d  Z.e.j.e.d...d.d.
-000012a0: 6416 8d03 5a17 6503 6a0b 6506 641d 8301  d...Z.e.j.e.d...
-000012b0: 6415 640d 6416 8d03 5a18 6503 6a0b 6506  d.d.d...Z.e.j.e.
-000012c0: 641e 8301 641f 640d 6416 8d03 5a19 6503  d...d.d.d...Z.e.
-000012d0: 6a0b 6506 6420 8301 641f 640a 8d02 5a1a  j.e.d ..d.d...Z.
-000012e0: 6503 6a0b 6506 6421 8301 641f 640a 8d02  e.j.e.d!..d.d...
-000012f0: 5a1b 6503 6a0b 6506 6422 8301 6423 640a  Z.e.j.e.d"..d#d.
-00001300: 8d02 5a1c 6503 6a1d 6506 6424 8301 640d  ..Z.e.j.e.d$..d.
-00001310: 6425 8d02 5a1e 6503 6a1d 6506 6426 8301  d%..Z.e.j.e.d&..
-00001320: 640d 6427 8d02 5a1f 6503 6a0b 6506 6428  d.d'..Z.e.j.e.d(
-00001330: 8301 6415 640d 6416 8d03 5a20 6503 6a0b  ..d.d.d...Z e.j.
-00001340: 6506 6429 8301 6415 640d 6416 8d03 5a21  e.d)..d.d.d...Z!
-00001350: 6503 6a0b 6506 642a 8301 642b 640a 8d02  e.j.e.d*..d+d...
-00001360: 5a22 6503 6a0b 6506 642c 8301 642b 640d  Z"e.j.e.d,..d+d.
-00001370: 6416 8d03 5a23 6503 6a0b 6506 642d 8301  d...Z#e.j.e.d-..
-00001380: 642e 640a 8d02 5a24 6503 6a0b 6506 642f  d.d...Z$e.j.e.d/
-00001390: 8301 6406 640a 8d02 5a25 6503 6a0b 6506  ..d.d...Z%e.j.e.
-000013a0: 6430 8301 6431 640d 6416 8d03 5a26 6503  d0..d1d.d...Z&e.
-000013b0: 6a0b 6506 6432 8301 642b 640d 6416 8d03  j.e.d2..d+d.d...
-000013c0: 5a27 6503 6a0b 6506 6433 8301 642e 640a  Z'e.j.e.d3..d.d.
-000013d0: 8d02 5a28 6503 6a0b 6506 6434 8301 642e  ..Z(e.j.e.d4..d.
-000013e0: 6435 6419 8d03 5a29 6503 6a0b 6506 6436  d5d...Z)e.j.e.d6
-000013f0: 8301 642e 6437 6419 8d03 5a2a 6503 6a0b  ..d.d7d...Z*e.j.
-00001400: 6506 6438 8301 641f 640a 8d02 5a2b 6503  e.d8..d.d...Z+e.
-00001410: a02c a100 5a2d 6439 643a 8400 5a2e 4700  .,..Z-d9d:..Z.G.
-00001420: 643b 643c 8400 643c 8302 5a2f 643d 5300  d;d<..d<..Z/d=S.
-00001430: 293e da17 4c65 6761 6379 5061 7970 616c  )>..LegacyPaypal
-00001440: 5472 616e 7361 6374 696f 6eda 0770 6179  Transaction..pay
-00001450: 6d65 6e74 da0c 7472 616e 7361 6374 696f  ment..transactio
-00001460: 6e73 a903 7254 0000 0072 2c00 0000 722d  ns..rT...r,...r-
-00001470: 0000 007a 0c74 6f74 616c 2061 6d6f 756e  ...z.total amoun
-00001480: 7472 4500 0000 7246 0000 0029 0272 4700  trE...rF...).rG.
-00001490: 0000 7248 0000 00da 0863 7572 7265 6e63  ..rH.....currenc
-000014a0: 79e9 0a00 0000 7242 0000 00da 0873 7562  y.....rB.....sub
-000014b0: 746f 7461 6cda 0374 6178 5429 0372 4700  total..taxT).rG.
-000014c0: 0000 7248 0000 0072 1100 0000 da08 7368  ..rH...r......sh
-000014d0: 6970 7069 6e67 7a0c 6861 6e64 6c69 6e67  ippingz.handling
-000014e0: 2066 6565 7a11 7368 6970 7069 6e67 2064   feez.shipping d
-000014f0: 6973 636f 756e 747a 0d69 6e73 7572 616e  iscountz.insuran
-00001500: 6365 2066 6565 7a0d 6769 6674 2077 7261  ce feez.gift wra
-00001510: 7020 6665 657a 0c72 6566 6572 656e 6365  p feez.reference
-00001520: 2069 6472 0c00 0000 7210 0000 007a 1673   idr....r....z.s
-00001530: 6574 746c 656d 656e 7420 6465 7374 696e  ettlement destin
-00001540: 6174 696f 6e5a 0f50 4152 544e 4552 5f42  ationZ.PARTNER_B
-00001550: 414c 414e 4345 2902 720e 0000 0072 4900  ALANCE).r....rI.
-00001560: 0000 7a16 616c 6c6f 7765 6420 7061 796d  ..z.allowed paym
-00001570: 656e 7420 6d65 7468 6f64 5a16 494e 5354  ent methodZ.INST
-00001580: 414e 545f 4655 4e44 494e 475f 534f 5552  ANT_FUNDING_SOUR
-00001590: 4345 da0b 6465 7363 7269 7074 696f 6e7a  CE..descriptionz
-000015a0: 0d6e 6f74 6520 746f 2070 6179 6565 7257  .note to payeerW
-000015b0: 0000 00e9 7f00 0000 7a0e 696e 766f 6963  ........z.invoic
-000015c0: 6520 6e75 6d62 6572 7a0e 7075 7263 6861  e numberz.purcha
-000015d0: 7365 206f 7264 6572 7a0f 736f 6674 2064  se orderz.soft d
-000015e0: 6573 6372 6970 746f 72e9 1600 0000 724c  escriptor.....rL
-000015f0: 0000 0072 2f00 0000 724d 0000 0072 4e00  ...r/...rM...rN.
-00001600: 0000 7a0f 7368 6970 7069 6e67 206d 6574  ..z.shipping met
-00001610: 686f 647a 1573 6869 7070 696e 6720 7068  hodz.shipping ph
-00001620: 6f6e 6520 6e75 6d62 6572 7a17 7368 6970  one numberz.ship
-00001630: 7069 6e67 2061 6464 7265 7373 206c 696e  ping address lin
-00001640: 6520 31e9 6400 0000 7a17 7368 6970 7069  e 1.d...z.shippi
-00001650: 6e67 2061 6464 7265 7373 206c 696e 6520  ng address line 
-00001660: 327a 1573 6869 7070 696e 6720 6164 6472  2z.shipping addr
-00001670: 6573 7320 6369 7479 e932 0000 007a 1873  ess city.2...z.s
-00001680: 6869 7070 696e 6720 6164 6472 6573 7320  hipping address 
-00001690: 636f 756e 7472 797a 1c73 6869 7070 696e  countryz.shippin
-000016a0: 6720 6164 6472 6573 7320 706f 7374 616c  g address postal
-000016b0: 2063 6f64 65e9 1400 0000 7a16 7368 6970   code.....z.ship
-000016c0: 7069 6e67 2061 6464 7265 7373 2073 7461  ping address sta
-000016d0: 7465 7a16 7368 6970 7069 6e67 2061 6464  tez.shipping add
-000016e0: 7265 7373 2070 686f 6e65 7a25 7368 6970  ress phonez%ship
-000016f0: 7069 6e67 2061 6464 7265 7373 206e 6f72  ping address nor
-00001700: 6d61 6c69 7a61 7469 6f6e 2073 7461 7475  malization statu
-00001710: 73da 0755 4e4b 4e4f 574e 7a15 7368 6970  s..UNKNOWNz.ship
-00001720: 7069 6e67 2061 6464 7265 7373 2074 7970  ping address typ
-00001730: 655a 0c48 4f4d 455f 4f52 5f57 4f52 4b7a  eZ.HOME_OR_WORKz
-00001740: 1f73 6869 7070 696e 6720 6164 6472 6573  .shipping addres
-00001750: 7320 7265 6369 7069 656e 7420 6e61 6d65  s recipient name
-00001760: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001770: 0005 0000 0043 0000 0073 1400 0000 6401  .....C...s....d.
-00001780: a000 7c00 6a01 7c00 6a02 7c00 6a03 a103  ..|.j.|.j.|.j...
-00001790: 5300 2902 4e7a 0a7b 7d20 2d20 7b7d 207b  S.).Nz.{} - {} {
-000017a0: 7d29 04da 0666 6f72 6d61 74da 0c72 6566  })...format..ref
-000017b0: 6572 656e 6365 5f69 64da 0c74 6f74 616c  erence_id..total
-000017c0: 5f61 6d6f 756e 7472 6300 0000 7216 0000  _amountrc...r...
-000017d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-000017e0: 7252 0000 0098 0000 0073 0200 0000 0001  rR.......s......
-000017f0: 7a1f 4c65 6761 6379 5061 7970 616c 5472  z.LegacyPaypalTr
-00001800: 616e 7361 6374 696f 6e2e 5f5f 7374 725f  ansaction.__str_
-00001810: 5f63 0000 0000 0000 0000 0000 0000 0000  _c..............
-00001820: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
-00001830: 005a 0164 005a 0265 0364 0183 015a 0465  .Z.d.Z.e.d...Z.e
-00001840: 0364 0283 015a 0564 0353 0029 047a 1c4c  .d...Z.d.S.).z.L
-00001850: 6567 6163 7950 6179 7061 6c54 7261 6e73  egacyPaypalTrans
-00001860: 6163 7469 6f6e 2e4d 6574 617a 2b4c 6567  action.Metaz+Leg
-00001870: 6163 7920 5061 7970 616c 2054 7261 6e73  acy Paypal Trans
-00001880: 6163 7469 6f6e 2028 7061 796d 656e 7473  action (payments
-00001890: 2076 3120 4150 4929 7a2c 4c65 6761 6379   v1 API)z,Legacy
-000018a0: 2050 6179 7061 6c20 5472 616e 7361 6374   Paypal Transact
-000018b0: 696f 6e73 2028 7061 796d 656e 7473 2076  ions (payments v
-000018c0: 3120 4150 4929 4e72 5300 0000 7218 0000  1 API)NrS...r...
-000018d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-000018e0: 7256 0000 009b 0000 0073 0400 0000 0801  rV.......s......
-000018f0: 0801 7256 0000 004e 2930 7222 0000 0072  ..rV...N)0r"...r
-00001900: 2300 0000 7224 0000 0072 0600 0000 7231  #...r$...r....r1
-00001910: 0000 0072 4000 0000 7226 0000 00da 0750  ...r@...r&.....P
-00001920: 524f 5445 4354 7260 0000 0072 5800 0000  ROTECTr`...rX...
-00001930: 7271 0000 0072 2500 0000 7263 0000 0072  rq...r%...rc...r
-00001940: 6500 0000 7266 0000 0072 6700 0000 5a0c  e...rf...rg...Z.
-00001950: 6861 6e64 6c69 6e67 5f66 6565 5a11 7368  handling_feeZ.sh
-00001960: 6970 7069 6e67 5f64 6973 636f 756e 745a  ipping_discountZ
-00001970: 0969 6e73 7572 616e 6365 5a09 6769 6674  .insuranceZ.gift
-00001980: 5f77 7261 7072 7000 0000 5a16 7365 7474  _wraprp...Z.sett
-00001990: 6c65 6d65 6e74 5f64 6573 7469 6e61 7469  lement_destinati
-000019a0: 6f6e 5a16 616c 6c6f 7765 645f 7061 796d  onZ.allowed_paym
-000019b0: 656e 745f 6d65 7468 6f64 7268 0000 005a  ent_methodrh...Z
-000019c0: 0d6e 6f74 655f 746f 5f70 6179 6565 7257  .note_to_payeerW
-000019d0: 0000 005a 0e69 6e76 6f69 6365 5f6e 756d  ...Z.invoice_num
-000019e0: 6265 725a 0e70 7572 6368 6173 655f 6f72  berZ.purchase_or
-000019f0: 6465 725a 0f73 6f66 745f 6465 7363 7269  derZ.soft_descri
-00001a00: 7074 6f72 7236 0000 0072 3700 0000 725c  ptorr6...r7...r\
-00001a10: 0000 005a 0f73 6869 7070 696e 675f 6d65  ...Z.shipping_me
-00001a20: 7468 6f64 5a15 7368 6970 7069 6e67 5f70  thodZ.shipping_p
-00001a30: 686f 6e65 5f6e 756d 6265 725a 1773 6869  hone_numberZ.shi
-00001a40: 7070 696e 675f 6164 6472 6573 735f 6c69  pping_address_li
-00001a50: 6e65 5f31 5a17 7368 6970 7069 6e67 5f61  ne_1Z.shipping_a
-00001a60: 6464 7265 7373 5f6c 696e 655f 325a 1573  ddress_line_2Z.s
-00001a70: 6869 7070 696e 675f 6164 6472 6573 735f  hipping_address_
-00001a80: 6369 7479 5a18 7368 6970 7069 6e67 5f61  cityZ.shipping_a
-00001a90: 6464 7265 7373 5f63 6f75 6e74 7279 5a1c  ddress_countryZ.
-00001aa0: 7368 6970 7069 6e67 5f61 6464 7265 7373  shipping_address
-00001ab0: 5f70 6f73 7461 6c5f 636f 6465 5a16 7368  _postal_codeZ.sh
-00001ac0: 6970 7069 6e67 5f61 6464 7265 7373 5f73  ipping_address_s
-00001ad0: 7461 7465 5a16 7368 6970 7069 6e67 5f61  tateZ.shipping_a
-00001ae0: 6464 7265 7373 5f70 686f 6e65 5a25 7368  ddress_phoneZ%sh
-00001af0: 6970 7069 6e67 5f61 6464 7265 7373 5f6e  ipping_address_n
-00001b00: 6f72 6d61 6c69 7a61 7469 6f6e 5f73 7461  ormalization_sta
-00001b10: 7475 735a 1573 6869 7070 696e 675f 6164  tusZ.shipping_ad
-00001b20: 6472 6573 735f 7479 7065 5a1f 7368 6970  dress_typeZ.ship
-00001b30: 7069 6e67 5f61 6464 7265 7373 5f72 6563  ping_address_rec
-00001b40: 6970 6965 6e74 5f6e 616d 6572 5d00 0000  ipient_namer]...
-00001b50: 725e 0000 0072 5200 0000 7256 0000 0072  r^...rR...rV...r
-00001b60: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00001b70: 0000 0072 5f00 0000 6600 0000 7368 0000  ...r_...f...sh..
-00001b80: 0008 0118 0214 0112 0114 0116 0116 0116  ................
-00001b90: 0116 0116 0116 0214 0114 0104 0106 0002  ................
-00001ba0: 0002 ff06 0314 0114 0114 0112 0112 0112  ................
-00001bb0: 0212 0112 0214 0114 0212 0114 0112 0112  ................
-00001bc0: 0104 0106 0002 0002 ff06 0314 0112 0104  ................
-00001bd0: 0106 0002 0002 ff06 0304 0106 0002 0002  ................
-00001be0: ff06 0312 0208 0208 0372 5f00 0000 6300  .........r_...c.
-00001bf0: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00001c00: 0000 0040 0000 0073 fa00 0000 6500 5a01  ...@...s....e.Z.
-00001c10: 6400 5a02 6503 6a04 6505 6506 6401 8301  d.Z.e.j.e.e.d...
-00001c20: 6402 6503 6a07 6403 8d04 5a08 6503 6a09  d.e.j.d...Z.e.j.
-00001c30: 6506 6404 8301 6405 6406 8d02 5a0a 6503  e.d...d.d...Z.e.
-00001c40: 6a09 6506 6407 8301 6405 6406 8d02 5a0b  j.e.d...d.d...Z.
-00001c50: 6503 6a09 6506 6408 8301 6405 6409 640a  e.j.e.d...d.d.d.
-00001c60: 8d03 5a0c 6503 6a09 6506 640b 8301 640c  ..Z.e.j.e.d...d.
-00001c70: 6406 8d02 5a0d 6503 6a09 6506 640d 8301  d...Z.e.j.e.d...
-00001c80: 640c 6406 8d02 5a0e 6503 6a09 6506 640e  d.d...Z.e.j.e.d.
-00001c90: 8301 640f 6406 8d02 5a0f 6503 6a09 6506  ..d.d...Z.e.j.e.
-00001ca0: 640e 8301 640c 6409 640a 8d03 5a10 6503  d...d.d.d...Z.e.
-00001cb0: 6a11 6506 6410 8301 6409 6411 8d02 5a12  j.e.d...d.d...Z.
-00001cc0: 6503 6a13 6506 6412 8301 6409 6413 8d02  e.j.e.d...d.d...
-00001cd0: 5a14 6503 6a13 6506 6414 8301 6409 6415  Z.e.j.e.d...d.d.
-00001ce0: 8d02 5a15 6503 a016 a100 5a17 6416 6417  ..Z.e.....Z.d.d.
-00001cf0: 8400 5a18 4700 6418 6419 8400 6419 8302  ..Z.G.d.d...d...
-00001d00: 5a19 641a 5300 291b da10 4c65 6761 6379  Z.d.S.)...Legacy
-00001d10: 5061 7970 616c 4974 656d da0b 7472 616e  PaypalItem..tran
-00001d20: 7361 6374 696f 6eda 0569 7465 6d73 7262  saction..itemsrb
-00001d30: 0000 007a 1273 746f 636b 206b 6565 7069  ...z.stock keepi
-00001d40: 6e67 2075 6e69 7472 6900 0000 7242 0000  ng unitri...rB..
-00001d50: 00da 046e 616d 6572 6800 0000 5472 1000  ...namerh...Tr..
-00001d60: 0000 da08 7175 616e 7469 7479 7264 0000  ....quantityrd..
-00001d70: 00da 0570 7269 6365 7263 0000 00e9 0300  ...pricerc......
-00001d80: 0000 7234 0000 0072 4b00 0000 724c 0000  ..r4...rK...rL..
-00001d90: 0072 2f00 0000 724d 0000 0072 4e00 0000  .r/...rM...rN...
-00001da0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001db0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00001dc0: 6a00 5300 7250 0000 0029 0172 7600 0000  j.S.rP...).rv...
-00001dd0: 7216 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00001de0: 1900 0000 7252 0000 00b1 0000 0073 0200  ....rR.......s..
-00001df0: 0000 0001 7a18 4c65 6761 6379 5061 7970  ....z.LegacyPayp
-00001e00: 616c 4974 656d 2e5f 5f73 7472 5f5f 6300  alItem.__str__c.
-00001e10: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00001e20: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
-00001e30: 6400 5a02 6503 6401 8301 5a04 6503 6401  d.Z.e.d...Z.e.d.
-00001e40: 8301 5a05 6402 5300 2903 7a15 4c65 6761  ..Z.d.S.).z.Lega
-00001e50: 6379 5061 7970 616c 4974 656d 2e4d 6574  cyPaypalItem.Met
-00001e60: 617a 244c 6567 6163 7920 5061 7970 616c  az$Legacy Paypal
-00001e70: 2049 7465 6d20 2870 6179 6d65 6e74 7320   Item (payments 
-00001e80: 7631 2041 5049 294e 7253 0000 0072 1800  v1 API)NrS...r..
-00001e90: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001ea0: 0072 5600 0000 b400 0000 7304 0000 0008  .rV.......s.....
-00001eb0: 0108 0172 5600 0000 4e29 1a72 2200 0000  ...rV...N).r"...
-00001ec0: 7223 0000 0072 2400 0000 7206 0000 0072  r#...r$...r....r
-00001ed0: 3100 0000 725f 0000 0072 2600 0000 7272  1...r_...r&...rr
-00001ee0: 0000 0072 7400 0000 7225 0000 005a 0373  ...rt...r%...Z.s
-00001ef0: 6b75 7276 0000 0072 6800 0000 7277 0000  kurv...rh...rw..
-00001f00: 0072 7800 0000 7263 0000 0072 6600 0000  .rx...rc...rf...
-00001f10: 725a 0000 0072 3400 0000 7236 0000 0072  rZ...r4...r6...r
-00001f20: 3700 0000 725c 0000 0072 5d00 0000 725e  7...r\...r]...r^
-00001f30: 0000 0072 5200 0000 7256 0000 0072 1800  ...rR...rV...r..
-00001f40: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001f50: 0072 7300 0000 a000 0000 731c 0000 0008  .rs.......s.....
-00001f60: 0118 0212 0112 0114 0112 0112 0112 0114  ................
-00001f70: 0112 0212 0112 0208 0208 0372 7300 0000  ...........rs...
-00001f80: 4e29 1dda 0a5f 5f66 7574 7572 655f 5f72  N)...__future__r
-00001f90: 0200 0000 da07 6465 6369 6d61 6c72 0300  ......decimalr..
-00001fa0: 0000 da06 7479 7069 6e67 7204 0000 005a  ....typingr....Z
-00001fb0: 1064 6174 6163 6c61 7373 5f77 697a 6172  .dataclass_wizar
-00001fc0: 6472 0500 0000 da09 646a 616e 676f 2e64  dr......django.d
-00001fd0: 6272 0600 0000 da18 646a 616e 676f 2e75  br......django.u
-00001fe0: 7469 6c73 2e74 7261 6e73 6c61 7469 6f6e  tils.translation
-00001ff0: 7207 0000 0072 2600 0000 5a17 646a 616e  r....r&...Z.djan
-00002000: 676f 5f70 6179 7061 6c2e 6170 695f 7479  go_paypal.api_ty
-00002010: 7065 7372 0800 0000 7209 0000 00da 1064  pesr....r......d
-00002020: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 7372  jango.db.modelsr
-00002030: 0a00 0000 da0b 496d 706f 7274 4572 726f  ......ImportErro
-00002040: 725a 1e64 6a61 6e67 6f2e 636f 6e74 7269  rZ.django.contri
-00002050: 622e 706f 7374 6772 6573 2e66 6965 6c64  b.postgres.field
-00002060: 73da 054d 6f64 656c 720b 0000 0072 2a00  s..Modelr....r*.
-00002070: 0000 7238 0000 0072 3c00 0000 723d 0000  ..r8...r<...r=..
-00002080: 0072 4000 0000 725f 0000 0072 7300 0000  .r@...r_...rs...
-00002090: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-000020a0: 1900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000020b0: 0000 7324 0000 000c 030c 010c 020c 010c  ..s$............
-000020c0: 010c 0210 0202 0210 010e 0212 0312 1112  ................
-000020d0: 0712 0812 0612 0912 2212 3a              ........".:
+00000080: 0100 7a10 6400 6408 6c0f 6d10 5a10 0100  ..z.d.d.l.m.Z...
+00000090: 5700 6e20 0400 6511 6b0a 7284 0100 0100  W.n ..e.k.r.....
+000000a0: 0100 6400 6408 6c12 6d10 5a10 0100 5900  ..d.d.l.m.Z...Y.
+000000b0: 6e02 5800 4700 6409 640a 8400 640a 6509  n.X.G.d.d...d.e.
+000000c0: 6a13 8303 5a14 4700 640b 640c 8400 640c  j...Z.G.d.d...d.
+000000d0: 6509 6a13 8303 5a15 4700 640d 640e 8400  e.j...Z.G.d.d...
+000000e0: 640e 6509 6a13 8303 5a16 4700 640f 6410  d.e.j...Z.G.d.d.
+000000f0: 8400 6410 6509 6a13 8303 5a17 4700 6411  ..d.e.j...Z.G.d.
+00000100: 6412 8400 6412 6509 6a13 8303 5a18 4700  d...d.e.j...Z.G.
+00000110: 6413 6414 8400 6414 6509 6a13 8303 5a19  d.d...d.e.j...Z.
+00000120: 4700 6415 6416 8400 6416 6509 6a13 8303  G.d.d...d.e.j...
+00000130: 5a1a 4700 6417 6418 8400 6418 6509 6a13  Z.G.d.d...d.e.j.
+00000140: 8303 5a1b 6419 5300 291a e900 0000 0029  ..Z.d.S.)......)
+00000150: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000160: 616c 7329 01da 0744 6563 696d 616c 2901  als)...Decimal).
+00000170: da04 4c69 7374 2901 da08 6672 6f6d 6469  ..List)...fromdi
+00000180: 6374 2901 da06 6d6f 6465 6c73 2901 da0c  ct)...models)...
+00000190: 6765 7474 6578 745f 6c61 7a79 2901 da07  gettext_lazy)...
+000001a0: 4361 7074 7572 6529 01da 094a 534f 4e46  Capture)...JSONF
+000001b0: 6965 6c64 6300 0000 0000 0000 0000 0000  ieldc...........
+000001c0: 0000 0000 0005 0000 0040 0000 0073 5a00  .........@...sZ.
+000001d0: 0000 6500 5a01 6400 5a02 6503 6a04 6505  ..e.Z.d.Z.e.j.e.
+000001e0: 6401 8301 6402 6403 6404 8d03 5a06 6503  d...d.d.d...Z.e.
+000001f0: 6a04 6505 6405 8301 6402 6403 6406 8d03  j.e.d...d.d.d...
+00000200: 5a07 6503 6a08 6407 9c01 6408 6409 8404  Z.e.j.d...d.d...
+00000210: 5a09 650a 650b 650c 1900 6407 9c01 640a  Z.e.e.e...d...d.
+00000220: 640b 8404 8301 5a0d 640c 5300 290d da0b  d.....Z.d.S.)...
+00000230: 5061 7970 616c 4f72 6465 727a 084f 7264  PaypalOrderz.Ord
+00000240: 6572 2049 44e9 ff00 0000 54a9 02da 0a6d  er ID.....T....m
+00000250: 6178 5f6c 656e 6774 68da 0675 6e69 7175  ax_length..uniqu
+00000260: 655a 0653 7461 7475 73a9 0272 0d00 0000  eZ.Status..r....
+00000270: da05 626c 616e 6b29 01da 0672 6574 7572  ..blank)...retur
+00000280: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00000290: 0000 0400 0000 4300 0000 7318 0000 007c  ......C...s....|
+000002a0: 006a 006a 0164 017c 006a 029b 0064 029d  .j.j.d.|.j...d..
+000002b0: 0364 038d 0153 0029 044e 7a14 2f76 322f  .d...S.).Nz./v2/
+000002c0: 6368 6563 6b6f 7574 2f6f 7264 6572 732f  checkout/orders/
+000002d0: 7a08 2f63 6170 7475 7265 2901 5a0d 7572  z./capture).Z.ur
+000002e0: 6c5f 5f63 6f6e 7461 696e 7329 03da 0d61  l__contains)...a
+000002f0: 7069 5f72 6573 706f 6e73 6573 da06 6669  pi_responses..fi
+00000300: 6c74 6572 da08 6f72 6465 725f 6964 a901  lter..order_id..
+00000310: da04 7365 6c66 a900 7217 0000 00fa 5b2f  ..self..r.....[/
+00000320: 5573 6572 732f 7469 6d74 616d 2f2e 7079  Users/timtam/.py
+00000330: 656e 762f 7665 7273 696f 6e73 2f73 662d  env/versions/sf-
+00000340: 332e 382e 3132 2f6c 6962 2f70 7974 686f  3.8.12/lib/pytho
+00000350: 6e33 2e38 2f73 6974 652d 7061 636b 6167  n3.8/site-packag
+00000360: 6573 2f64 6a61 6e67 6f5f 7061 7970 616c  es/django_paypal
+00000370: 2f6d 6f64 656c 732e 7079 da19 6765 745f  /models.py..get_
+00000380: 6361 7074 7572 655f 6170 695f 7265 7370  capture_api_resp
+00000390: 6f6e 7365 7319 0000 0073 0200 0000 0001  onses....s......
+000003a0: 7a25 5061 7970 616c 4f72 6465 722e 6765  z%PaypalOrder.ge
+000003b0: 745f 6361 7074 7572 655f 6170 695f 7265  t_capture_api_re
+000003c0: 7370 6f6e 7365 7363 0100 0000 0000 0000  sponsesc........
+000003d0: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
+000003e0: 7356 0000 0074 0083 007d 017c 00a0 01a1  sV...t...}.|....
+000003f0: 0044 005d 427d 027c 026a 02a0 0364 0167  .D.]B}.|.j...d.g
+00000400: 00a1 0244 005d 2e7d 037c 03a0 0364 0269  ...D.].}.|...d.i
+00000410: 00a1 02a0 0364 0367 00a1 0244 005d 147d  .....d.g...D.].}
+00000420: 047c 01a0 0474 0574 067c 0483 02a1 0101  .|...t.t.|......
+00000430: 0071 3871 2071 0e7c 0153 0029 044e 5a0e  .q8q q.|.S.).NZ.
+00000440: 7075 7263 6861 7365 5f75 6e69 7473 5a08  purchase_unitsZ.
+00000450: 7061 796d 656e 7473 da08 6361 7074 7572  payments..captur
+00000460: 6573 2907 da04 6c69 7374 7219 0000 00da  es)...listr.....
+00000470: 0d72 6573 706f 6e73 655f 6461 7461 da03  .response_data..
+00000480: 6765 74da 0661 7070 656e 6472 0500 0000  get..appendr....
+00000490: 7208 0000 0029 0572 1600 0000 721a 0000  r....).r....r...
+000004a0: 00da 1063 6170 7475 7265 5f72 6573 706f  ...capture_respo
+000004b0: 6e73 655a 0d70 7572 6368 6173 655f 756e  nseZ.purchase_un
+000004c0: 6974 da07 6361 7074 7572 6572 1700 0000  it..capturer....
+000004d0: 7217 0000 0072 1800 0000 721a 0000 001c  r....r....r.....
+000004e0: 0000 0073 0c00 0000 0002 0601 0c01 1201  ...s............
+000004f0: 1801 1601 7a14 5061 7970 616c 4f72 6465  ....z.PaypalOrde
+00000500: 722e 6361 7074 7572 6573 4e29 0eda 085f  r.capturesN)..._
+00000510: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000520: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000530: 5f72 0600 0000 da09 4368 6172 4669 656c  _r......CharFiel
+00000540: 64da 015f 7214 0000 00da 0673 7461 7475  d.._r......statu
+00000550: 73da 0851 7565 7279 5365 7472 1900 0000  s..QuerySetr....
+00000560: da08 7072 6f70 6572 7479 7204 0000 0072  ..propertyr....r
+00000570: 0800 0000 721a 0000 0072 1700 0000 7217  ....r....r....r.
+00000580: 0000 0072 1700 0000 7218 0000 0072 0a00  ...r....r....r..
+00000590: 0000 1500 0000 730a 0000 0008 0114 0114  ......s.........
+000005a0: 0210 0302 0172 0a00 0000 6300 0000 0000  .....r....c.....
+000005b0: 0000 0000 0000 0000 0000 0005 0000 0040  ...............@
+000005c0: 0000 0073 4a00 0000 6500 5a01 6400 5a02  ...sJ...e.Z.d.Z.
+000005d0: 6503 6a04 6505 6401 6503 6a06 6402 8d03  e.j.e.d.e.j.d...
+000005e0: 5a07 6503 6a08 6509 6403 8301 6404 6405  Z.e.j.e.d...d.d.
+000005f0: 6406 8d03 5a0a 650b 6509 6407 8301 8301  d...Z.e.e.d.....
+00000600: 5a0c 6503 6a0d 6405 6408 8d01 5a0e 6409  Z.e.j.d.d...Z.d.
+00000610: 5300 290a da11 5061 7970 616c 4150 4950  S.)...PaypalAPIP
+00000620: 6f73 7444 6174 615a 0961 7069 5f70 6f73  ostDataZ.api_pos
+00000630: 7473 a902 da0c 7265 6c61 7465 645f 6e61  ts....related_na
+00000640: 6d65 da09 6f6e 5f64 656c 6574 65da 0355  me..on_delete..U
+00000650: 524c 720b 0000 0054 720f 0000 007a 0950  RLr....Tr....z.P
+00000660: 6f73 7420 4461 7461 a901 da0c 6175 746f  ost Data....auto
+00000670: 5f6e 6f77 5f61 6464 4e29 0f72 2100 0000  _now_addN).r!...
+00000680: 7222 0000 0072 2300 0000 7206 0000 00da  r"...r#...r.....
+00000690: 0a46 6f72 6569 676e 4b65 7972 0a00 0000  .ForeignKeyr....
+000006a0: da07 4341 5343 4144 45da 056f 7264 6572  ..CASCADE..order
+000006b0: 7224 0000 0072 2500 0000 da03 7572 6c72  r$...r%.....urlr
+000006c0: 0900 0000 da09 706f 7374 5f64 6174 61da  ......post_data.
+000006d0: 0d44 6174 6554 696d 6546 6965 6c64 da0a  .DateTimeField..
+000006e0: 6372 6561 7465 645f 6174 7217 0000 0072  created_atr....r
+000006f0: 1700 0000 7217 0000 0072 1800 0000 7229  ....r....r....r)
+00000700: 0000 0026 0000 0073 0800 0000 0801 1201  ...&...s........
+00000710: 1401 0c01 7229 0000 0063 0000 0000 0000  ....r)...c......
+00000720: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00000730: 0000 735e 0000 0065 005a 0164 005a 0265  ..s^...e.Z.d.Z.e
+00000740: 036a 0465 0564 0165 036a 0664 028d 035a  .j.e.d.e.j.d...Z
+00000750: 0765 036a 0465 0864 0364 0465 036a 0664  .e.j.e.d.d.e.j.d
+00000760: 058d 045a 0965 036a 0a65 0b64 0683 0164  ...Z.e.j.e.d...d
+00000770: 0764 0464 088d 035a 0c65 0d65 0b64 0983  .d.d...Z.e.e.d..
+00000780: 0183 015a 0e65 036a 0f64 0464 0a8d 015a  ...Z.e.j.d.d...Z
+00000790: 1064 0b53 0029 0cda 1150 6179 7061 6c41  .d.S.)...PaypalA
+000007a0: 5049 5265 7370 6f6e 7365 7212 0000 0072  PIResponser....r
+000007b0: 2a00 0000 da09 7265 7370 6f6e 7365 7354  *.....responsesT
+000007c0: 2903 722b 0000 00da 046e 756c 6c72 2c00  ).r+.....nullr,.
+000007d0: 0000 722d 0000 0072 0b00 0000 720f 0000  ..r-...r....r...
+000007e0: 007a 0d52 6573 706f 6e73 6520 4461 7461  .z.Response Data
+000007f0: 722e 0000 004e 2911 7221 0000 0072 2200  r....N).r!...r".
+00000800: 0000 7223 0000 0072 0600 0000 7230 0000  ..r#...r....r0..
+00000810: 0072 0a00 0000 7231 0000 0072 3200 0000  .r....r1...r2...
+00000820: 7229 0000 00da 0470 6f73 7472 2400 0000  r).....postr$...
+00000830: 7225 0000 0072 3300 0000 7209 0000 0072  r%...r3...r....r
+00000840: 1c00 0000 7235 0000 0072 3600 0000 7217  ....r5...r6...r.
+00000850: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000860: 0000 7237 0000 002d 0000 0073 0a00 0000  ..r7...-...s....
+00000870: 0801 1201 1401 1401 0c01 7237 0000 0063  ..........r7...c
+00000880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000890: 0500 0000 4000 0000 735c 0000 0065 005a  ....@...s\...e.Z
+000008a0: 0164 005a 0265 036a 0465 0564 0183 0164  .d.Z.e.j.e.d...d
+000008b0: 0264 0364 048d 035a 0665 036a 0465 0564  .d.d...Z.e.j.e.d
+000008c0: 0583 0164 0264 0664 078d 035a 0765 036a  ...d.d.d...Z.e.j
+000008d0: 0464 0864 0264 098d 025a 0865 0965 0564  .d.d.d...Z.e.e.d
+000008e0: 0a83 0183 015a 0a47 0064 0b64 0c84 0064  .....Z.G.d.d...d
+000008f0: 0c83 025a 0b64 0d53 0029 0eda 0d50 6179  ...Z.d.S.)...Pay
+00000900: 7061 6c57 6562 686f 6f6b 7a0a 5765 6268  palWebhookz.Webh
+00000910: 6f6f 6b20 4944 720b 0000 0054 720c 0000  ook IDr....Tr...
+00000920: 007a 0941 7574 6820 4861 7368 da00 a902  .z.Auth Hash....
+00000930: 720d 0000 00da 0764 6566 6175 6c74 722d  r......defaultr-
+00000940: 0000 00a9 0172 0d00 0000 7a15 4163 7469  .....r....z.Acti
+00000950: 7665 2057 6562 686f 6f6b 2045 7665 6e74  ve Webhook Event
+00000960: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000970: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
+00000980: 005a 0164 005a 0264 015a 0364 0253 0029  .Z.d.Z.d.Z.d.S.)
+00000990: 037a 1250 6179 7061 6c57 6562 686f 6f6b  .z.PaypalWebhook
+000009a0: 2e4d 6574 6129 0272 3300 0000 da09 6175  .Meta).r3.....au
+000009b0: 7468 5f68 6173 684e 2904 7221 0000 0072  th_hashN).r!...r
+000009c0: 2200 0000 7223 0000 00da 0f75 6e69 7175  "...r#.....uniqu
+000009d0: 655f 746f 6765 7468 6572 7217 0000 0072  e_togetherr....r
+000009e0: 1700 0000 7217 0000 0072 1800 0000 da04  ....r....r......
+000009f0: 4d65 7461 3b00 0000 7302 0000 0008 0172  Meta;...s......r
+00000a00: 4200 0000 4e29 0c72 2100 0000 7222 0000  B...N).r!...r"..
+00000a10: 0072 2300 0000 7206 0000 0072 2400 0000  .r#...r....r$...
+00000a20: 7225 0000 005a 0a77 6562 686f 6f6b 5f69  r%...Z.webhook_i
+00000a30: 6472 4000 0000 7233 0000 0072 0900 0000  dr@...r3...r....
+00000a40: 5a0b 6576 656e 745f 7479 7065 7372 4200  Z.event_typesrB.
+00000a50: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000a60: 0072 1800 0000 723b 0000 0035 0000 0073  .r....r;...5...s
+00000a70: 0a00 0000 0801 1401 1401 0e01 0c02 723b  ..............r;
+00000a80: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000a90: 0000 0000 0500 0000 4000 0000 733c 0000  ........@...s<..
+00000aa0: 0065 005a 0164 005a 0265 0365 0464 0183  .e.Z.d.Z.e.e.d..
+00000ab0: 0183 015a 0565 066a 0765 0864 0265 066a  ...Z.e.j.e.d.e.j
+00000ac0: 0964 038d 035a 0a65 066a 0765 0b64 0465  .d...Z.e.j.e.d.e
+00000ad0: 066a 0964 038d 035a 0c64 0553 0029 06da  .j.d...Z.d.S.)..
+00000ae0: 1250 6179 7061 6c57 6562 686f 6f6b 4576  .PaypalWebhookEv
+00000af0: 656e 745a 0750 6179 6c6f 6164 5a0e 7765  entZ.PayloadZ.we
+00000b00: 6268 6f6f 6b5f 6576 656e 7473 722a 0000  bhook_eventsr*..
+00000b10: 00da 0665 7665 6e74 734e 290d 7221 0000  ...eventsN).r!..
+00000b20: 0072 2200 0000 7223 0000 0072 0900 0000  .r"...r#...r....
+00000b30: 7225 0000 00da 0770 6179 6c6f 6164 7206  r%.....payloadr.
+00000b40: 0000 0072 3000 0000 720a 0000 0072 3100  ...r0...r....r1.
+00000b50: 0000 7232 0000 0072 3b00 0000 5a07 7765  ..r2...r;...Z.we
+00000b60: 6268 6f6f 6b72 1700 0000 7217 0000 0072  bhookr....r....r
+00000b70: 1700 0000 7218 0000 0072 4300 0000 4200  ....r....rC...B.
+00000b80: 0000 7306 0000 0008 010c 0112 0172 4300  ..s..........rC.
+00000b90: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000ba0: 0000 0006 0000 0040 0000 0073 a401 0000  .......@...s....
+00000bb0: 6500 5a01 6400 5a02 6503 6a04 6505 6401  e.Z.d.Z.e.j.e.d.
+00000bc0: 8301 6402 6403 6404 8d03 5a06 6503 6a04  ..d.d.d...Z.e.j.
+00000bd0: 6505 6405 8301 6402 6406 8d02 5a07 6503  e.d...d.d...Z.e.
+00000be0: 6a04 6505 6405 8301 6402 6403 6407 8d03  j.e.d...d.d.d...
+00000bf0: 5a08 6503 6a04 6505 6405 8301 6408 6403  Z.e.j.e.d...d.d.
+00000c00: 6407 8d03 5a09 6503 6a04 6505 6409 8301  d...Z.e.j.e.d...
+00000c10: 6402 6403 6407 8d03 5a0a 6503 6a04 6505  d.d.d...Z.e.j.e.
+00000c20: 640a 8301 6402 6403 6407 8d03 5a0b 6503  d...d.d.d...Z.e.
+00000c30: 6a04 6505 640a 8301 6402 6403 6407 8d03  j.e.d...d.d.d...
+00000c40: 5a0c 6503 6a04 6505 640b 8301 6402 6403  Z.e.j.e.d...d.d.
+00000c50: 6407 8d03 5a0d 6503 6a0e 6505 640c 8301  d...Z.e.j.e.d...
+00000c60: 640d 640e 650f 640f 8301 6410 8d04 5a10  d.d.e.d...d...Z.
+00000c70: 6503 6a04 6505 6411 8301 6402 6403 6403  e.j.e.d...d.d.d.
+00000c80: 6412 8d04 5a11 6503 6a04 6505 6413 8301  d...Z.e.j.e.d...
+00000c90: 6402 6403 6403 6412 8d04 5a12 6503 6a13  d.d.d.d...Z.e.j.
+00000ca0: 6505 6414 8301 6403 6403 6415 8d03 5a14  e.d...d.d.d...Z.
+00000cb0: 6503 6a13 6505 6416 8301 6403 6403 6415  e.j.e.d...d.d.d.
+00000cc0: 8d03 5a15 6503 6a04 6505 6417 8301 6402  ..Z.e.j.e.d...d.
+00000cd0: 6403 6407 8d03 5a16 6503 6a17 6505 6418  d.d...Z.e.j.e.d.
+00000ce0: 8301 6403 6419 8d02 5a18 6503 6a17 6505  ..d.d...Z.e.j.e.
+00000cf0: 641a 8301 6403 6419 8d02 5a19 6503 6a17  d...d.d...Z.e.j.
+00000d00: 6505 641b 8301 6403 6419 8d02 5a1a 6503  e.d...d.d...Z.e.
+00000d10: 6a1b 6505 641c 8301 6403 641d 8d02 5a1c  j.e.d...d.d...Z.
+00000d20: 6503 6a1b 6505 641e 8301 6403 641f 8d02  e.j.e.d...d.d...
+00000d30: 5a1d 6503 a01e a100 5a1f 6420 6421 8400  Z.e.....Z.d d!..
+00000d40: 5a20 4700 6422 6423 8400 6423 8302 5a21  Z G.d"d#..d#..Z!
+00000d50: 6424 5300 2925 da13 4c65 6761 6379 5061  d$S.)%..LegacyPa
+00000d60: 7970 616c 5061 796d 656e 747a 0a70 6179  ypalPaymentz.pay
+00000d70: 6d65 6e74 2069 6472 0b00 0000 5472 0c00  ment idr....Tr..
+00000d80: 0000 da06 696e 7465 6e74 723f 0000 0072  ....intentr?...r
+00000d90: 0f00 0000 e9a5 0000 00da 0573 7461 7465  ...........state
+00000da0: 7a0e 7061 796d 656e 7420 6d65 7468 6f64  z.payment method
+00000db0: 7a08 7061 7965 7220 6964 7a0f 7472 616e  z.payer idz.tran
+00000dc0: 7361 6374 696f 6e20 6665 65e9 0900 0000  saction fee.....
+00000dd0: e902 0000 0072 0100 0000 2903 da0a 6d61  .....r....)...ma
+00000de0: 785f 6469 6769 7473 da0e 6465 6369 6d61  x_digits..decima
+00000df0: 6c5f 706c 6163 6573 723e 0000 007a 1372  l_placesr>...z.r
+00000e00: 656c 6174 6564 2072 6573 6f75 7263 6520  elated resource 
+00000e10: 6964 2903 720d 0000 0072 1000 0000 7239  id).r....r....r9
+00000e20: 0000 007a 1672 656c 6174 6564 2072 6573  ...z.related res
+00000e30: 6f75 7263 6520 7374 6174 657a 1569 6e69  ource statez.ini
+00000e40: 7469 616c 2070 6f73 7420 7265 7370 6f6e  tial post respon
+00000e50: 7365 2902 7239 0000 0072 1000 0000 7a14  se).r9...r....z.
+00000e60: 7570 6461 7465 6420 6765 7420 7265 7370  updated get resp
+00000e70: 6f6e 7365 7a0e 6661 696c 7572 6520 7265  onsez.failure re
+00000e80: 6173 6f6e da04 6c69 6e6b a901 7210 0000  ason..link..r...
+00000e90: 007a 0c61 7070 726f 7665 206c 696e 6b7a  .z.approve linkz
+00000ea0: 0c65 7865 6375 7465 206c 696e 6bfa 0a63  .execute link..c
+00000eb0: 7265 6174 6564 2061 7472 2e00 0000 fa0d  reated atr......
+00000ec0: 6c61 7374 206d 6f64 6966 6965 64a9 01da  last modified...
+00000ed0: 0861 7574 6f5f 6e6f 7763 0100 0000 0000  .auto_nowc......
+00000ee0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000ef0: 0000 7306 0000 007c 006a 0053 00a9 014e  ..s....|.j.S...N
+00000f00: 2901 da0a 7061 796d 656e 745f 6964 7215  )...payment_idr.
+00000f10: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000f20: 0000 da07 5f5f 7374 725f 5f65 0000 0073  ....__str__e...s
+00000f30: 0200 0000 0001 7a1b 4c65 6761 6379 5061  ......z.LegacyPa
+00000f40: 7970 616c 5061 796d 656e 742e 5f5f 7374  ypalPayment.__st
+00000f50: 725f 5f63 0000 0000 0000 0000 0000 0000  r__c............
+00000f60: 0000 0000 0200 0000 4000 0000 731c 0000  ........@...s...
+00000f70: 0065 005a 0164 005a 0265 0364 0183 015a  .e.Z.d.Z.e.d...Z
+00000f80: 0465 0364 0283 015a 0564 0353 0029 047a  .e.d...Z.d.S.).z
+00000f90: 184c 6567 6163 7950 6179 7061 6c50 6179  .LegacyPaypalPay
+00000fa0: 6d65 6e74 2e4d 6574 617a 274c 6567 6163  ment.Metaz'Legac
+00000fb0: 7920 5061 7970 616c 2050 6179 6d65 6e74  y Paypal Payment
+00000fc0: 2028 7061 796d 656e 7473 2076 3120 4150   (payments v1 AP
+00000fd0: 4929 7a28 4c65 6761 6379 2050 6179 7061  I)z(Legacy Paypa
+00000fe0: 6c20 5061 796d 656e 7473 2028 7061 796d  l Payments (paym
+00000ff0: 656e 7473 2076 3120 4150 4929 4ea9 0672  ents v1 API)N..r
+00001000: 2100 0000 7222 0000 0072 2300 0000 7225  !...r"...r#...r%
+00001010: 0000 00da 0c76 6572 626f 7365 5f6e 616d  .....verbose_nam
+00001020: 65da 1376 6572 626f 7365 5f6e 616d 655f  e..verbose_name_
+00001030: 706c 7572 616c 7217 0000 0072 1700 0000  pluralr....r....
+00001040: 7217 0000 0072 1800 0000 7242 0000 0068  r....r....rB...h
+00001050: 0000 0073 0400 0000 0801 0801 7242 0000  ...s........rB..
+00001060: 004e 2922 7221 0000 0072 2200 0000 7223  .N)"r!...r"...r#
+00001070: 0000 0072 0600 0000 7224 0000 0072 2500  ...r....r$...r%.
+00001080: 0000 7255 0000 0072 4700 0000 5a15 6578  ..rU...rG...Z.ex
+00001090: 7065 7269 656e 6365 5f70 726f 6669 6c65  perience_profile
+000010a0: 5f69 645a 0d6e 6f74 655f 746f 5f70 6179  _idZ.note_to_pay
+000010b0: 6572 7249 0000 005a 0e70 6179 6d65 6e74  errI...Z.payment
+000010c0: 5f6d 6574 686f 64da 0663 7573 746f 6d5a  _method..customZ
+000010d0: 0870 6179 6572 5f69 64da 0c44 6563 696d  .payer_id..Decim
+000010e0: 616c 4669 656c 6472 0300 0000 5a0f 7472  alFieldr....Z.tr
+000010f0: 616e 7361 6374 696f 6e5f 6665 655a 1372  ansaction_feeZ.r
+00001100: 656c 6174 6564 5f72 6573 6f75 7263 655f  elated_resource_
+00001110: 6964 5a16 7265 6c61 7465 645f 7265 736f  idZ.related_reso
+00001120: 7572 6365 5f73 7461 7465 da09 5465 7874  urce_state..Text
+00001130: 4669 656c 645a 1769 6e69 7469 616c 5f72  FieldZ.initial_r
+00001140: 6573 706f 6e73 655f 6f62 6a65 6374 5a16  esponse_objectZ.
+00001150: 7570 6461 7465 5f72 6573 706f 6e73 655f  update_response_
+00001160: 6f62 6a65 6374 5a0e 6661 696c 7572 655f  objectZ.failure_
+00001170: 7265 6173 6f6e da08 5552 4c46 6965 6c64  reason..URLField
+00001180: 724e 0000 00da 0c61 7070 726f 7665 5f6c  rN.....approve_l
+00001190: 696e 6b5a 0c65 7865 6375 7465 5f6c 696e  inkZ.execute_lin
+000011a0: 6b72 3500 0000 7236 0000 00da 0d6c 6173  kr5...r6.....las
+000011b0: 745f 6d6f 6469 6669 6564 da07 4d61 6e61  t_modified..Mana
+000011c0: 6765 72da 076f 626a 6563 7473 7256 0000  ger..objectsrV..
+000011d0: 0072 4200 0000 7217 0000 0072 1700 0000  .rB...r....r....
+000011e0: 7217 0000 0072 1800 0000 7246 0000 004b  r....r....rF...K
+000011f0: 0000 0073 2c00 0000 0801 1401 1201 1401  ...s,...........
+00001200: 1401 1401 1401 1401 1401 1a01 1601 1601  ................
+00001210: 1401 1402 1402 1201 1201 1202 1201 1202  ................
+00001220: 0802 0803 7246 0000 0063 0000 0000 0000  ....rF...c......
+00001230: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00001240: 0000 73b8 0200 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+00001250: 036a 0465 0565 0664 0183 0164 0265 036a  .j.e.e.d...d.e.j
+00001260: 0764 038d 045a 0865 036a 0965 0664 0483  .d...Z.e.j.e.d..
+00001270: 0164 0564 0664 078d 035a 0a65 036a 0b65  .d.d.d...Z.e.j.e
+00001280: 0664 0883 0164 0964 0a8d 025a 0c65 036a  .d...d.d...Z.e.j
+00001290: 0965 0664 0b83 0164 0564 0664 078d 035a  .e.d...d.d.d...Z
+000012a0: 0d65 036a 0965 0664 0c83 0164 0564 0664  .e.j.e.d...d.d.d
+000012b0: 0d64 0e8d 045a 0e65 036a 0965 0664 0f83  .d...Z.e.j.e.d..
+000012c0: 0164 0564 0664 0d64 0e8d 045a 0f65 036a  .d.d.d.d...Z.e.j
+000012d0: 0965 0664 1083 0164 0564 0664 0d64 0e8d  .e.d...d.d.d.d..
+000012e0: 045a 1065 036a 0965 0664 1183 0164 0564  .Z.e.j.e.d...d.d
+000012f0: 0664 0d64 0e8d 045a 1165 036a 0965 0664  .d.d...Z.e.j.e.d
+00001300: 1283 0164 0564 0664 0d64 0e8d 045a 1265  ...d.d.d.d...Z.e
+00001310: 036a 0965 0664 1383 0164 0564 0664 0d64  .j.e.d...d.d.d.d
+00001320: 0e8d 045a 1365 036a 0b65 0664 1483 0164  ...Z.e.j.e.d...d
+00001330: 1564 0d64 168d 035a 1465 036a 0b65 0664  .d.d...Z.e.j.e.d
+00001340: 1783 0164 1564 1864 198d 035a 1565 036a  ...d.d.d...Z.e.j
+00001350: 0b65 0664 1a83 0164 1564 1b64 198d 035a  .e.d...d.d.d...Z
+00001360: 1665 036a 0b65 0664 1c83 0164 1564 0d64  .e.j.e.d...d.d.d
+00001370: 168d 035a 1765 036a 0b65 0664 1d83 0164  ...Z.e.j.e.d...d
+00001380: 1564 0d64 168d 035a 1865 036a 0b65 0664  .d.d...Z.e.j.e.d
+00001390: 1e83 0164 1f64 0d64 168d 035a 1965 036a  ...d.d.d...Z.e.j
+000013a0: 0b65 0664 2083 0164 1f64 0a8d 025a 1a65  .e.d ..d.d...Z.e
+000013b0: 036a 0b65 0664 2183 0164 1f64 0a8d 025a  .j.e.d!..d.d...Z
+000013c0: 1b65 036a 0b65 0664 2283 0164 2364 0a8d  .e.j.e.d"..d#d..
+000013d0: 025a 1c65 036a 1d65 0664 2483 0164 0d64  .Z.e.j.e.d$..d.d
+000013e0: 258d 025a 1e65 036a 1d65 0664 2683 0164  %..Z.e.j.e.d&..d
+000013f0: 0d64 278d 025a 1f65 036a 0b65 0664 2883  .d'..Z.e.j.e.d(.
+00001400: 0164 1564 0d64 168d 035a 2065 036a 0b65  .d.d.d...Z e.j.e
+00001410: 0664 2983 0164 1564 0d64 168d 035a 2165  .d)..d.d.d...Z!e
+00001420: 036a 0b65 0664 2a83 0164 2b64 0a8d 025a  .j.e.d*..d+d...Z
+00001430: 2265 036a 0b65 0664 2c83 0164 2b64 0d64  "e.j.e.d,..d+d.d
+00001440: 168d 035a 2365 036a 0b65 0664 2d83 0164  ...Z#e.j.e.d-..d
+00001450: 2e64 0a8d 025a 2465 036a 0b65 0664 2f83  .d...Z$e.j.e.d/.
+00001460: 0164 0664 0a8d 025a 2565 036a 0b65 0664  .d.d...Z%e.j.e.d
+00001470: 3083 0164 3164 0d64 168d 035a 2665 036a  0..d1d.d...Z&e.j
+00001480: 0b65 0664 3283 0164 2b64 0d64 168d 035a  .e.d2..d+d.d...Z
+00001490: 2765 036a 0b65 0664 3383 0164 2e64 0a8d  'e.j.e.d3..d.d..
+000014a0: 025a 2865 036a 0b65 0664 3483 0164 2e64  .Z(e.j.e.d4..d.d
+000014b0: 3564 198d 035a 2965 036a 0b65 0664 3683  5d...Z)e.j.e.d6.
+000014c0: 0164 2e64 3764 198d 035a 2a65 036a 0b65  .d.d7d...Z*e.j.e
+000014d0: 0664 3883 0164 1f64 0a8d 025a 2b65 03a0  .d8..d.d...Z+e..
+000014e0: 2ca1 005a 2d64 3964 3a84 005a 2e47 0064  ,..Z-d9d:..Z.G.d
+000014f0: 3b64 3c84 0064 3c83 025a 2f64 3d53 0029  ;d<..d<..Z/d=S.)
+00001500: 3eda 174c 6567 6163 7950 6179 7061 6c54  >..LegacyPaypalT
+00001510: 7261 6e73 6163 7469 6f6e da07 7061 796d  ransaction..paym
+00001520: 656e 74da 0c74 7261 6e73 6163 7469 6f6e  ent..transaction
+00001530: 73a9 0372 5800 0000 722b 0000 0072 2c00  s..rX...r+...r,.
+00001540: 0000 7a0c 746f 7461 6c20 616d 6f75 6e74  ..z.total amount
+00001550: 724a 0000 0072 4b00 0000 2902 724c 0000  rJ...rK...).rL..
+00001560: 0072 4d00 0000 da08 6375 7272 656e 6379  .rM.....currency
+00001570: e90a 0000 0072 3f00 0000 da08 7375 6274  .....r?.....subt
+00001580: 6f74 616c da03 7461 7854 2903 724c 0000  otal..taxT).rL..
+00001590: 0072 4d00 0000 7210 0000 00da 0873 6869  .rM...r......shi
+000015a0: 7070 696e 677a 0c68 616e 646c 696e 6720  ppingz.handling 
+000015b0: 6665 657a 1173 6869 7070 696e 6720 6469  feez.shipping di
+000015c0: 7363 6f75 6e74 7a0d 696e 7375 7261 6e63  scountz.insuranc
+000015d0: 6520 6665 657a 0d67 6966 7420 7772 6170  e feez.gift wrap
+000015e0: 2066 6565 7a0c 7265 6665 7265 6e63 6520   feez.reference 
+000015f0: 6964 720b 0000 0072 0f00 0000 7a16 7365  idr....r....z.se
+00001600: 7474 6c65 6d65 6e74 2064 6573 7469 6e61  ttlement destina
+00001610: 7469 6f6e 5a0f 5041 5254 4e45 525f 4241  tionZ.PARTNER_BA
+00001620: 4c41 4e43 4572 3d00 0000 7a16 616c 6c6f  LANCEr=...z.allo
+00001630: 7765 6420 7061 796d 656e 7420 6d65 7468  wed payment meth
+00001640: 6f64 5a16 494e 5354 414e 545f 4655 4e44  odZ.INSTANT_FUND
+00001650: 494e 475f 534f 5552 4345 da0b 6465 7363  ING_SOURCE..desc
+00001660: 7269 7074 696f 6e7a 0d6e 6f74 6520 746f  riptionz.note to
+00001670: 2070 6179 6565 725a 0000 00e9 7f00 0000   payeerZ........
+00001680: 7a0e 696e 766f 6963 6520 6e75 6d62 6572  z.invoice number
+00001690: 7a0e 7075 7263 6861 7365 206f 7264 6572  z.purchase order
+000016a0: 7a0f 736f 6674 2064 6573 6372 6970 746f  z.soft descripto
+000016b0: 72e9 1600 0000 7250 0000 0072 2e00 0000  r.....rP...r....
+000016c0: 7251 0000 0072 5200 0000 7a0f 7368 6970  rQ...rR...z.ship
+000016d0: 7069 6e67 206d 6574 686f 647a 1573 6869  ping methodz.shi
+000016e0: 7070 696e 6720 7068 6f6e 6520 6e75 6d62  pping phone numb
+000016f0: 6572 7a17 7368 6970 7069 6e67 2061 6464  erz.shipping add
+00001700: 7265 7373 206c 696e 6520 31e9 6400 0000  ress line 1.d...
+00001710: 7a17 7368 6970 7069 6e67 2061 6464 7265  z.shipping addre
+00001720: 7373 206c 696e 6520 327a 1573 6869 7070  ss line 2z.shipp
+00001730: 696e 6720 6164 6472 6573 7320 6369 7479  ing address city
+00001740: e932 0000 007a 1873 6869 7070 696e 6720  .2...z.shipping 
+00001750: 6164 6472 6573 7320 636f 756e 7472 797a  address countryz
+00001760: 1c73 6869 7070 696e 6720 6164 6472 6573  .shipping addres
+00001770: 7320 706f 7374 616c 2063 6f64 65e9 1400  s postal code...
+00001780: 0000 7a16 7368 6970 7069 6e67 2061 6464  ..z.shipping add
+00001790: 7265 7373 2073 7461 7465 7a16 7368 6970  ress statez.ship
+000017a0: 7069 6e67 2061 6464 7265 7373 2070 686f  ping address pho
+000017b0: 6e65 7a25 7368 6970 7069 6e67 2061 6464  nez%shipping add
+000017c0: 7265 7373 206e 6f72 6d61 6c69 7a61 7469  ress normalizati
+000017d0: 6f6e 2073 7461 7475 73da 0755 4e4b 4e4f  on status..UNKNO
+000017e0: 574e 7a15 7368 6970 7069 6e67 2061 6464  WNz.shipping add
+000017f0: 7265 7373 2074 7970 655a 0c48 4f4d 455f  ress typeZ.HOME_
+00001800: 4f52 5f57 4f52 4b7a 1f73 6869 7070 696e  OR_WORKz.shippin
+00001810: 6720 6164 6472 6573 7320 7265 6369 7069  g address recipi
+00001820: 656e 7420 6e61 6d65 6301 0000 0000 0000  ent namec.......
+00001830: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00001840: 0073 1400 0000 6401 a000 7c00 6a01 7c00  .s....d...|.j.|.
+00001850: 6a02 7c00 6a03 a103 5300 2902 4e7a 0a7b  j.|.j...S.).Nz.{
+00001860: 7d20 2d20 7b7d 207b 7d29 04da 0666 6f72  } - {} {})...for
+00001870: 6d61 74da 0c72 6566 6572 656e 6365 5f69  mat..reference_i
+00001880: 64da 0c74 6f74 616c 5f61 6d6f 756e 7472  d..total_amountr
+00001890: 6600 0000 7215 0000 0072 1700 0000 7217  f...r....r....r.
+000018a0: 0000 0072 1800 0000 7256 0000 009f 0000  ...r....rV......
+000018b0: 0073 0200 0000 0001 7a1f 4c65 6761 6379  .s......z.Legacy
+000018c0: 5061 7970 616c 5472 616e 7361 6374 696f  PaypalTransactio
+000018d0: 6e2e 5f5f 7374 725f 5f63 0000 0000 0000  n.__str__c......
+000018e0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+000018f0: 0000 731c 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+00001900: 0364 0183 015a 0465 0364 0283 015a 0564  .d...Z.e.d...Z.d
+00001910: 0353 0029 047a 1c4c 6567 6163 7950 6179  .S.).z.LegacyPay
+00001920: 7061 6c54 7261 6e73 6163 7469 6f6e 2e4d  palTransaction.M
+00001930: 6574 617a 2b4c 6567 6163 7920 5061 7970  etaz+Legacy Payp
+00001940: 616c 2054 7261 6e73 6163 7469 6f6e 2028  al Transaction (
+00001950: 7061 796d 656e 7473 2076 3120 4150 4929  payments v1 API)
+00001960: 7a2c 4c65 6761 6379 2050 6179 7061 6c20  z,Legacy Paypal 
+00001970: 5472 616e 7361 6374 696f 6e73 2028 7061  Transactions (pa
+00001980: 796d 656e 7473 2076 3120 4150 4929 4e72  yments v1 API)Nr
+00001990: 5700 0000 7217 0000 0072 1700 0000 7217  W...r....r....r.
+000019a0: 0000 0072 1800 0000 7242 0000 00a2 0000  ...r....rB......
+000019b0: 0073 0400 0000 0801 0801 7242 0000 004e  .s........rB...N
+000019c0: 2930 7221 0000 0072 2200 0000 7223 0000  )0r!...r"...r#..
+000019d0: 0072 0600 0000 7230 0000 0072 4600 0000  .r....r0...rF...
+000019e0: 7225 0000 00da 0750 524f 5445 4354 7263  r%.....PROTECTrc
+000019f0: 0000 0072 5b00 0000 7274 0000 0072 2400  ...r[...rt...r$.
+00001a00: 0000 7266 0000 0072 6800 0000 7269 0000  ..rf...rh...ri..
+00001a10: 0072 6a00 0000 5a0c 6861 6e64 6c69 6e67  .rj...Z.handling
+00001a20: 5f66 6565 5a11 7368 6970 7069 6e67 5f64  _feeZ.shipping_d
+00001a30: 6973 636f 756e 745a 0969 6e73 7572 616e  iscountZ.insuran
+00001a40: 6365 5a09 6769 6674 5f77 7261 7072 7300  ceZ.gift_wraprs.
+00001a50: 0000 5a16 7365 7474 6c65 6d65 6e74 5f64  ..Z.settlement_d
+00001a60: 6573 7469 6e61 7469 6f6e 5a16 616c 6c6f  estinationZ.allo
+00001a70: 7765 645f 7061 796d 656e 745f 6d65 7468  wed_payment_meth
+00001a80: 6f64 726b 0000 005a 0d6e 6f74 655f 746f  odrk...Z.note_to
+00001a90: 5f70 6179 6565 725a 0000 005a 0e69 6e76  _payeerZ...Z.inv
+00001aa0: 6f69 6365 5f6e 756d 6265 725a 0e70 7572  oice_numberZ.pur
+00001ab0: 6368 6173 655f 6f72 6465 725a 0f73 6f66  chase_orderZ.sof
+00001ac0: 745f 6465 7363 7269 7074 6f72 7235 0000  t_descriptorr5..
+00001ad0: 0072 3600 0000 725f 0000 005a 0f73 6869  .r6...r_...Z.shi
+00001ae0: 7070 696e 675f 6d65 7468 6f64 5a15 7368  pping_methodZ.sh
+00001af0: 6970 7069 6e67 5f70 686f 6e65 5f6e 756d  ipping_phone_num
+00001b00: 6265 725a 1773 6869 7070 696e 675f 6164  berZ.shipping_ad
+00001b10: 6472 6573 735f 6c69 6e65 5f31 5a17 7368  dress_line_1Z.sh
+00001b20: 6970 7069 6e67 5f61 6464 7265 7373 5f6c  ipping_address_l
+00001b30: 696e 655f 325a 1573 6869 7070 696e 675f  ine_2Z.shipping_
+00001b40: 6164 6472 6573 735f 6369 7479 5a18 7368  address_cityZ.sh
+00001b50: 6970 7069 6e67 5f61 6464 7265 7373 5f63  ipping_address_c
+00001b60: 6f75 6e74 7279 5a1c 7368 6970 7069 6e67  ountryZ.shipping
+00001b70: 5f61 6464 7265 7373 5f70 6f73 7461 6c5f  _address_postal_
+00001b80: 636f 6465 5a16 7368 6970 7069 6e67 5f61  codeZ.shipping_a
+00001b90: 6464 7265 7373 5f73 7461 7465 5a16 7368  ddress_stateZ.sh
+00001ba0: 6970 7069 6e67 5f61 6464 7265 7373 5f70  ipping_address_p
+00001bb0: 686f 6e65 5a25 7368 6970 7069 6e67 5f61  honeZ%shipping_a
+00001bc0: 6464 7265 7373 5f6e 6f72 6d61 6c69 7a61  ddress_normaliza
+00001bd0: 7469 6f6e 5f73 7461 7475 735a 1573 6869  tion_statusZ.shi
+00001be0: 7070 696e 675f 6164 6472 6573 735f 7479  pping_address_ty
+00001bf0: 7065 5a1f 7368 6970 7069 6e67 5f61 6464  peZ.shipping_add
+00001c00: 7265 7373 5f72 6563 6970 6965 6e74 5f6e  ress_recipient_n
+00001c10: 616d 6572 6000 0000 7261 0000 0072 5600  amer`...ra...rV.
+00001c20: 0000 7242 0000 0072 1700 0000 7217 0000  ..rB...r....r...
+00001c30: 0072 1700 0000 7218 0000 0072 6200 0000  .r....r....rb...
+00001c40: 6d00 0000 7368 0000 0008 0118 0214 0112  m...sh..........
+00001c50: 0114 0116 0116 0116 0116 0116 0116 0214  ................
+00001c60: 0114 0104 0106 0002 0002 ff06 0314 0114  ................
+00001c70: 0114 0112 0112 0112 0212 0112 0214 0114  ................
+00001c80: 0212 0114 0112 0112 0104 0106 0002 0002  ................
+00001c90: ff06 0314 0112 0104 0106 0002 0002 ff06  ................
+00001ca0: 0304 0106 0002 0002 ff06 0312 0208 0208  ................
+00001cb0: 0372 6200 0000 6300 0000 0000 0000 0000  .rb...c.........
+00001cc0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+00001cd0: fa00 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00001ce0: 6505 6506 6401 8301 6402 6503 6a07 6403  e.e.d...d.e.j.d.
+00001cf0: 8d04 5a08 6503 6a09 6506 6404 8301 6405  ..Z.e.j.e.d...d.
+00001d00: 6406 8d02 5a0a 6503 6a09 6506 6407 8301  d...Z.e.j.e.d...
+00001d10: 6405 6406 8d02 5a0b 6503 6a09 6506 6408  d.d...Z.e.j.e.d.
+00001d20: 8301 6405 6409 640a 8d03 5a0c 6503 6a09  ..d.d.d...Z.e.j.
+00001d30: 6506 640b 8301 640c 6406 8d02 5a0d 6503  e.d...d.d...Z.e.
+00001d40: 6a09 6506 640d 8301 640c 6406 8d02 5a0e  j.e.d...d.d...Z.
+00001d50: 6503 6a09 6506 640e 8301 640f 6406 8d02  e.j.e.d...d.d...
+00001d60: 5a0f 6503 6a09 6506 640e 8301 640c 6409  Z.e.j.e.d...d.d.
+00001d70: 640a 8d03 5a10 6503 6a11 6506 6410 8301  d...Z.e.j.e.d...
+00001d80: 6409 6411 8d02 5a12 6503 6a13 6506 6412  d.d...Z.e.j.e.d.
+00001d90: 8301 6409 6413 8d02 5a14 6503 6a13 6506  ..d.d...Z.e.j.e.
+00001da0: 6414 8301 6409 6415 8d02 5a15 6503 a016  d...d.d...Z.e...
+00001db0: a100 5a17 6416 6417 8400 5a18 4700 6418  ..Z.d.d...Z.G.d.
+00001dc0: 6419 8400 6419 8302 5a19 641a 5300 291b  d...d...Z.d.S.).
+00001dd0: da10 4c65 6761 6379 5061 7970 616c 4974  ..LegacyPaypalIt
+00001de0: 656d da0b 7472 616e 7361 6374 696f 6eda  em..transaction.
+00001df0: 0569 7465 6d73 7265 0000 007a 1273 746f  .itemsre...z.sto
+00001e00: 636b 206b 6565 7069 6e67 2075 6e69 7472  ck keeping unitr
+00001e10: 6c00 0000 723f 0000 00da 046e 616d 6572  l...r?.....namer
+00001e20: 6b00 0000 5472 0f00 0000 da08 7175 616e  k...Tr......quan
+00001e30: 7469 7479 7267 0000 00da 0570 7269 6365  tityrg.....price
+00001e40: 7266 0000 00e9 0300 0000 7233 0000 0072  rf........r3...r
+00001e50: 4f00 0000 7250 0000 0072 2e00 0000 7251  O...rP...r....rQ
+00001e60: 0000 0072 5200 0000 6301 0000 0000 0000  ...rR...c.......
+00001e70: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00001e80: 0073 0600 0000 7c00 6a00 5300 7254 0000  .s....|.j.S.rT..
+00001e90: 0029 0172 7900 0000 7215 0000 0072 1700  .).ry...r....r..
+00001ea0: 0000 7217 0000 0072 1800 0000 7256 0000  ..r....r....rV..
+00001eb0: 00b8 0000 0073 0200 0000 0001 7a18 4c65  .....s......z.Le
+00001ec0: 6761 6379 5061 7970 616c 4974 656d 2e5f  gacyPaypalItem._
+00001ed0: 5f73 7472 5f5f 6300 0000 0000 0000 0000  _str__c.........
+00001ee0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00001ef0: 1c00 0000 6500 5a01 6400 5a02 6503 6401  ....e.Z.d.Z.e.d.
+00001f00: 8301 5a04 6503 6401 8301 5a05 6402 5300  ..Z.e.d...Z.d.S.
+00001f10: 2903 7a15 4c65 6761 6379 5061 7970 616c  ).z.LegacyPaypal
+00001f20: 4974 656d 2e4d 6574 617a 244c 6567 6163  Item.Metaz$Legac
+00001f30: 7920 5061 7970 616c 2049 7465 6d20 2870  y Paypal Item (p
+00001f40: 6179 6d65 6e74 7320 7631 2041 5049 294e  ayments v1 API)N
+00001f50: 7257 0000 0072 1700 0000 7217 0000 0072  rW...r....r....r
+00001f60: 1700 0000 7218 0000 0072 4200 0000 bb00  ....r....rB.....
+00001f70: 0000 7304 0000 0008 0108 0172 4200 0000  ..s........rB...
+00001f80: 4e29 1a72 2100 0000 7222 0000 0072 2300  N).r!...r"...r#.
+00001f90: 0000 7206 0000 0072 3000 0000 7262 0000  ..r....r0...rb..
+00001fa0: 0072 2500 0000 7275 0000 0072 7700 0000  .r%...ru...rw...
+00001fb0: 7224 0000 005a 0373 6b75 7279 0000 0072  r$...Z.skury...r
+00001fc0: 6b00 0000 727a 0000 0072 7b00 0000 7266  k...rz...r{...rf
+00001fd0: 0000 0072 6900 0000 725d 0000 0072 3300  ...ri...r]...r3.
+00001fe0: 0000 7235 0000 0072 3600 0000 725f 0000  ..r5...r6...r_..
+00001ff0: 0072 6000 0000 7261 0000 0072 5600 0000  .r`...ra...rV...
+00002000: 7242 0000 0072 1700 0000 7217 0000 0072  rB...r....r....r
+00002010: 1700 0000 7218 0000 0072 7600 0000 a700  ....r....rv.....
+00002020: 0000 731c 0000 0008 0118 0212 0112 0114  ..s.............
+00002030: 0112 0112 0112 0114 0112 0212 0112 0208  ................
+00002040: 0208 0372 7600 0000 4e29 1cda 0a5f 5f66  ...rv...N)...__f
+00002050: 7574 7572 655f 5f72 0200 0000 da07 6465  uture__r......de
+00002060: 6369 6d61 6c72 0300 0000 da06 7479 7069  cimalr......typi
+00002070: 6e67 7204 0000 005a 1064 6174 6163 6c61  ngr....Z.datacla
+00002080: 7373 5f77 697a 6172 6472 0500 0000 da09  ss_wizardr......
+00002090: 646a 616e 676f 2e64 6272 0600 0000 da18  django.dbr......
+000020a0: 646a 616e 676f 2e75 7469 6c73 2e74 7261  django.utils.tra
+000020b0: 6e73 6c61 7469 6f6e 7207 0000 0072 2500  nslationr....r%.
+000020c0: 0000 5a17 646a 616e 676f 5f70 6179 7061  ..Z.django_paypa
+000020d0: 6c2e 6170 695f 7479 7065 7372 0800 0000  l.api_typesr....
+000020e0: da10 646a 616e 676f 2e64 622e 6d6f 6465  ..django.db.mode
+000020f0: 6c73 7209 0000 00da 0b49 6d70 6f72 7445  lsr......ImportE
+00002100: 7272 6f72 5a1e 646a 616e 676f 2e63 6f6e  rrorZ.django.con
+00002110: 7472 6962 2e70 6f73 7467 7265 732e 6669  trib.postgres.fi
+00002120: 656c 6473 da05 4d6f 6465 6c72 0a00 0000  elds..Modelr....
+00002130: 7229 0000 0072 3700 0000 723b 0000 0072  r)...r7...r;...r
+00002140: 4300 0000 7246 0000 0072 6200 0000 7276  C...rF...rb...rv
+00002150: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00002160: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00002170: 3e01 0000 0073 2400 0000 0c03 0c01 0c02  >....s$.........
+00002180: 0c01 0c01 0c02 0c02 0202 1001 0e02 1203  ................
+00002190: 1211 1207 1208 120d 1209 1222 123a       ...........".:
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-311.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/settings.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/settings.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 26 04:47:09 2024 UTC, .py size: 1281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 cd31 2b66 0105 0000  U........1+f....
+00000000: 550d 0d0a 0000 0000 2f19 2f66 0d05 0000  U......././f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6503 5a04 6505 6501 6403  m.Z...e.Z.e.e.d.
 00000050: 6404 8303 5a06 6505 6501 6405 6404 8303  d...Z.e.e.d.d...
 00000060: 5a07 6505 6501 6406 6407 8303 5a08 6505  Z.e.e.d.d...Z.e.
 00000070: 6501 6408 6409 8303 5a09 6505 6501 640a  e.d.d...Z.e.e.d.
@@ -27,43 +27,44 @@
 000001a0: 782e 7061 7970 616c 2e63 6f6d da0e 5041  x.paypal.com..PA
 000001b0: 5950 414c 5f53 414e 4442 4f58 54da 0f50  YPAL_SANDBOXT..P
 000001c0: 4159 5041 4c5f 4155 5448 5f55 524c 7a10  AYPAL_AUTH_URLz.
 000001d0: 2f76 312f 6f61 7574 6832 2f74 6f6b 656e  /v1/oauth2/token
 000001e0: da19 5041 5950 414c 5f41 5554 485f 4341  ..PAYPAL_AUTH_CA
 000001f0: 4348 455f 5449 4d45 4f55 5469 5802 0000  CHE_TIMEOUTiX...
 00000200: da15 5041 5950 414c 5f41 5554 485f 4341  ..PAYPAL_AUTH_CA
-00000210: 4348 455f 4b45 597a 1264 6a61 6e67 6f2d  CHE_KEYz.django-
-00000220: 7061 7970 616c 2d61 7574 68da 1a50 4159  paypal-auth..PAY
-00000230: 5041 4c5f 4f52 4445 5253 5f41 5049 5f45  PAL_ORDERS_API_E
-00000240: 4e44 504f 494e 547a 132f 7632 2f63 6865  NDPOINTz./v2/che
-00000250: 636b 6f75 742f 6f72 6465 7273 da17 5041  ckout/orders..PA
-00000260: 5950 414c 5f57 4542 484f 4f4b 5f4c 4953  YPAL_WEBHOOK_LIS
-00000270: 5445 4e45 524e da12 5041 5950 414c 5f53  TENERN..PAYPAL_S
-00000280: 5543 4345 5353 5f55 524c fa01 2fda 1a50  UCCESS_URL../..P
-00000290: 4159 4449 5245 4b54 5f43 414e 4345 4c4c  AYDIREKT_CANCELL
-000002a0: 4154 494f 4e5f 5552 4cda 1a50 4159 4449  ATION_URL..PAYDI
-000002b0: 5245 4b54 5f4e 4f54 4946 4943 4154 494f  REKT_NOTIFICATIO
-000002c0: 4e5f 5552 4c7a 0f2f 7061 7970 616c 2f6e  N_URLz./paypal/n
-000002d0: 6f74 6966 792f da06 5041 5950 414c 2914  otify/..PAYPAL).
-000002e0: da0b 646a 616e 676f 2e63 6f6e 6672 0200  ..django.confr..
-000002f0: 0000 5a16 646a 616e 676f 5f70 6179 7061  ..Z.django_paypa
-00000300: 6c2e 5f5f 696e 6974 5f5f 7203 0000 00da  l.__init__r.....
-00000310: 1544 4a41 4e47 4f5f 5041 5950 414c 5f56  .DJANGO_PAYPAL_V
-00000320: 4552 5349 4f4e da07 6765 7461 7474 7272  ERSION..getattrr
-00000330: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000340: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000350: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000360: 0072 0e00 0000 da17 5041 5950 414c 5f43  .r......PAYPAL_C
-00000370: 414e 4345 4c4c 4154 494f 4e5f 5552 4c5a  ANCELLATION_URLZ
-00000380: 1750 4159 5041 4c5f 4e4f 5449 4649 4341  .PAYPAL_NOTIFICA
-00000390: 5449 4f4e 5f55 524c da0f 5041 5950 414c  TION_URL..PAYPAL
-000003a0: 5f52 4f4f 545f 5552 4ca9 0072 1800 0000  _ROOT_URL..r....
-000003b0: 7218 0000 00fa 5d2f 5573 6572 732f 7469  r.....]/Users/ti
-000003c0: 6d74 616d 2f2e 7079 656e 762f 7665 7273  mtam/.pyenv/vers
-000003d0: 696f 6e73 2f73 662d 332e 382e 3132 2f6c  ions/sf-3.8.12/l
-000003e0: 6962 2f70 7974 686f 6e33 2e38 2f73 6974  ib/python3.8/sit
-000003f0: 652d 7061 636b 6167 6573 2f64 6a61 6e67  e-packages/djang
-00000400: 6f5f 7061 7970 616c 2f73 6574 7469 6e67  o_paypal/setting
-00000410: 732e 7079 da08 3c6d 6f64 756c 653e 0100  s.py..<module>..
-00000420: 0000 7322 0000 000c 020c 0204 020c 010c  ..s"............
-00000430: 020c 010c 010c 020c 010c 010c 010c 010c  ................
-00000440: 030c 010c 010c 020c 01                   .........
+00000210: 4348 455f 4b45 597a 1e64 6a61 6e67 6f2d  CHE_KEYz.django-
+00000220: 7061 7970 616c 2d61 7574 682d 7b61 7574  paypal-auth-{aut
+00000230: 685f 6861 7368 7dda 1a50 4159 5041 4c5f  h_hash}..PAYPAL_
+00000240: 4f52 4445 5253 5f41 5049 5f45 4e44 504f  ORDERS_API_ENDPO
+00000250: 494e 547a 132f 7632 2f63 6865 636b 6f75  INTz./v2/checkou
+00000260: 742f 6f72 6465 7273 da17 5041 5950 414c  t/orders..PAYPAL
+00000270: 5f57 4542 484f 4f4b 5f4c 4953 5445 4e45  _WEBHOOK_LISTENE
+00000280: 524e da12 5041 5950 414c 5f53 5543 4345  RN..PAYPAL_SUCCE
+00000290: 5353 5f55 524c fa01 2fda 1a50 4159 4449  SS_URL../..PAYDI
+000002a0: 5245 4b54 5f43 414e 4345 4c4c 4154 494f  REKT_CANCELLATIO
+000002b0: 4e5f 5552 4cda 1a50 4159 4449 5245 4b54  N_URL..PAYDIREKT
+000002c0: 5f4e 4f54 4946 4943 4154 494f 4e5f 5552  _NOTIFICATION_UR
+000002d0: 4c7a 0f2f 7061 7970 616c 2f6e 6f74 6966  Lz./paypal/notif
+000002e0: 792f da06 5041 5950 414c 2914 da0b 646a  y/..PAYPAL)...dj
+000002f0: 616e 676f 2e63 6f6e 6672 0200 0000 5a16  ango.confr....Z.
+00000300: 646a 616e 676f 5f70 6179 7061 6c2e 5f5f  django_paypal.__
+00000310: 696e 6974 5f5f 7203 0000 00da 1544 4a41  init__r......DJA
+00000320: 4e47 4f5f 5041 5950 414c 5f56 4552 5349  NGO_PAYPAL_VERSI
+00000330: 4f4e da07 6765 7461 7474 7272 0400 0000  ON..getattrr....
+00000340: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00000350: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+00000360: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000370: 0000 da17 5041 5950 414c 5f43 414e 4345  ....PAYPAL_CANCE
+00000380: 4c4c 4154 494f 4e5f 5552 4c5a 1750 4159  LLATION_URLZ.PAY
+00000390: 5041 4c5f 4e4f 5449 4649 4341 5449 4f4e  PAL_NOTIFICATION
+000003a0: 5f55 524c da0f 5041 5950 414c 5f52 4f4f  _URL..PAYPAL_ROO
+000003b0: 545f 5552 4ca9 0072 1800 0000 7218 0000  T_URL..r....r...
+000003c0: 00fa 5d2f 5573 6572 732f 7469 6d74 616d  ..]/Users/timtam
+000003d0: 2f2e 7079 656e 762f 7665 7273 696f 6e73  /.pyenv/versions
+000003e0: 2f73 662d 332e 382e 3132 2f6c 6962 2f70  /sf-3.8.12/lib/p
+000003f0: 7974 686f 6e33 2e38 2f73 6974 652d 7061  ython3.8/site-pa
+00000400: 636b 6167 6573 2f64 6a61 6e67 6f5f 7061  ckages/django_pa
+00000410: 7970 616c 2f73 6574 7469 6e67 732e 7079  ypal/settings.py
+00000420: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
+00000430: 0000 000c 020c 0204 020c 010c 020c 010c  ................
+00000440: 010c 020c 010c 010c 010c 010c 030c 010c  ................
+00000450: 010c 020c 01                             .....
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/webhooks.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/webhooks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 26 05:07:12 2024 UTC, .py size: 2602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8036 2b66 2a0a 0000  U........6+f*...
+00000000: 550d 0d0a 0000 0000 2f19 2f66 4f09 0000  U......././fO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -49,114 +49,108 @@
 00000300: 2f6c 6962 2f70 7974 686f 6e33 2e38 2f73  /lib/python3.8/s
 00000310: 6974 652d 7061 636b 6167 6573 2f64 6a61  ite-packages/dja
 00000320: 6e67 6f5f 7061 7970 616c 2f77 6562 686f  ngo_paypal/webho
 00000330: 6f6b 732e 7079 7212 0000 0011 0000 0073  oks.pyr........s
 00000340: 0200 0000 0801 7212 0000 0029 03da 0772  ......r....)...r
 00000350: 6571 7565 7374 da0e 7061 7970 616c 5f77  equest..paypal_w
 00000360: 7261 7070 6572 da07 7061 796c 6f61 6463  rapper..payloadc
-00000370: 0300 0000 0000 0000 0000 0000 0800 0000  ................
-00000380: 0900 0000 4300 0000 73b6 0000 0074 0064  ....C...s....t.d
-00000390: 017c 0283 0201 0074 0064 027c 0264 0319  .|.....t.d.|.d..
-000003a0: 0064 0419 0083 0201 0064 0564 066c 016d  .d.......d.d.l.m
-000003b0: 017d 0301 007c 037c 006a 0283 0101 0074  .}...|.|.j.....t
-000003c0: 036a 0473 b27c 0264 0319 0064 0419 007d  .j.s.|.d...d...}
-000003d0: 0474 056a 066a 077c 0464 078d 017d 057c  .t.j.j.|.d...}.|
-000003e0: 01a0 087c 007c 056a 09a1 0201 007a 1a74  ...|.|.j.....z.t
-000003f0: 0a6a 066a 077c 0264 0319 0064 0419 0064  .j.j.|.d...d...d
-00000400: 088d 017d 0657 006e 1c04 0074 0b74 0c66  ...}.W.n...t.t.f
-00000410: 026b 0a72 9601 0001 0001 0064 007d 0659  .k.r.......d.}.Y
-00000420: 006e 0258 007c 027c 057c 0664 099c 037d  .n.X.|.|.|.d...}
-00000430: 0774 0d6a 066a 0e66 007c 078e 0101 0064  .t.j.j.f.|.....d
-00000440: 0053 0029 0a4e 721d 0000 00da 0a77 6562  .S.).Nr......web
-00000450: 686f 6f6b 5f69 64da 0872 6573 6f75 7263  hook_id..resourc
-00000460: 65da 0269 6472 0100 0000 2901 da06 7070  e..idr....)...pp
-00000470: 7269 6e74 2901 721e 0000 0029 01da 086f  rint).r....)...o
-00000480: 7264 6572 5f69 6429 0372 1d00 0000 da07  rder_id).r......
-00000490: 7765 6268 6f6f 6bda 056f 7264 6572 290f  webhook..order).
-000004a0: da05 7072 696e 7472 2100 0000 da04 4d45  ..printr!.....ME
-000004b0: 5441 7204 0000 00da 0544 4542 5547 720c  TAr......DEBUGr.
-000004c0: 0000 00da 076f 626a 6563 7473 da03 6765  .....objects..ge
-000004d0: 74da 1476 6572 6966 795f 7765 6268 6f6f  t..verify_webhoo
-000004e0: 6b5f 6576 656e 7472 1e00 0000 720e 0000  k_eventr....r...
-000004f0: 00da 084b 6579 4572 726f 72da 0954 7970  ...KeyError..Typ
-00000500: 6545 7272 6f72 720d 0000 00da 0663 7265  eErrorr......cre
-00000510: 6174 6529 0872 1b00 0000 721c 0000 0072  ate).r....r....r
-00000520: 1d00 0000 7221 0000 0072 1e00 0000 da0e  ....r!...r......
-00000530: 7061 7970 616c 5f77 6562 686f 6f6b da0c  paypal_webhook..
-00000540: 7061 7970 616c 5f6f 7264 6572 5a0a 6576  paypal_orderZ.ev
-00000550: 656e 745f 6461 7461 7219 0000 0072 1900  ent_datar....r..
-00000560: 0000 721a 0000 00da 1d76 6572 6966 795f  ..r......verify_
-00000570: 616e 645f 7361 7665 5f77 6562 686f 6f6b  and_save_webhook
-00000580: 5f65 7665 6e74 1500 0000 7322 0000 0000  _event....s"....
-00000590: 010a 0112 010c 010a 0106 010c 010e 010e  ................
-000005a0: 0102 011a 0112 010a 0202 0102 0102 fd06  ................
-000005b0: 0572 3000 0000 da08 6469 7370 6174 6368  .r0.....dispatch
-000005c0: 2901 da04 6e61 6d65 6300 0000 0000 0000  )...namec.......
-000005d0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-000005e0: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-000005f0: 6402 8400 5a03 6403 5300 2904 da11 5061  d...Z.d.S.)...Pa
-00000600: 7970 616c 5765 6268 6f6f 6b56 6965 7763  ypalWebhookViewc
-00000610: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00000620: 0500 0000 4f00 0000 73b0 0000 0074 00a0  ....O...s....t..
-00000630: 017c 016a 02a0 0364 01a1 01a1 017d 047c  .|.j...d.....}.|
-00000640: 04a0 0464 02a1 017d 057c 0574 056a 066b  ...d...}.|.t.j.k
-00000650: 0772 3074 0764 0364 048d 0153 0074 0874  .r0t.d.d...S.t.t
-00000660: 0974 0a6a 0b74 0a6a 0c64 058d 0264 068d  .t.j.t.j.d...d..
-00000670: 017d 0674 0d7c 017c 067c 0464 078d 0301  .}.t.|.|.|.d....
-00000680: 007c 0564 086b 0272 8874 0e6a 0f7c 006a  .|.d.k.r.t.j.|.j
-00000690: 107c 04a0 0464 09a1 0164 0a8d 0201 007c  .|...d...d.....|
-000006a0: 06a0 117c 04a0 0464 09a1 01a0 0464 0ba1  ...|...d.....d..
-000006b0: 01a1 0101 007c 0564 0c6b 0272 a674 126a  .....|.d.k.r.t.j
-000006c0: 0f7c 006a 107c 04a0 0464 09a1 0164 0a8d  .|.j.|...d...d..
-000006d0: 0201 0074 0764 0d64 048d 0153 0029 0e4e  ...t.d.d...S.).N
-000006e0: 7a05 7574 662d 38da 0a65 7665 6e74 5f74  z.utf-8..event_t
-000006f0: 7970 6569 9001 0000 2901 da06 7374 6174  ypei....)...stat
-00000700: 7573 2902 da09 636c 6965 6e74 5f69 64da  us)...client_id.
-00000710: 0d63 6c69 656e 745f 7365 6372 6574 2901  .client_secret).
-00000720: da04 6175 7468 2901 721d 0000 0072 1400  ..auth).r....r..
-00000730: 0000 721f 0000 0029 02da 0673 656e 6465  ..r....)...sende
-00000740: 7272 1f00 0000 7220 0000 0072 1300 0000  rr....r ...r....
-00000750: e9c8 0000 0029 13da 046a 736f 6eda 056c  .....)...json..l
-00000760: 6f61 6473 da04 626f 6479 da06 6465 636f  oads..body..deco
-00000770: 6465 7229 0000 0072 1200 0000 7218 0000  der)...r....r...
-00000780: 0072 0500 0000 7211 0000 0072 0b00 0000  .r....r....r....
-00000790: da16 646a 616e 676f 5f70 6179 7061 6c5f  ..django_paypal_
-000007a0: 7365 7474 696e 6773 da14 5041 5950 414c  settings..PAYPAL
-000007b0: 5f41 5049 5f43 4c49 454e 545f 4944 da11  _API_CLIENT_ID..
-000007c0: 5041 5950 414c 5f41 5049 5f53 4543 5245  PAYPAL_API_SECRE
-000007d0: 5472 3000 0000 720f 0000 00da 0473 656e  Tr0...r......sen
-000007e0: 64da 095f 5f63 6c61 7373 5f5f da0d 6361  d..__class__..ca
-000007f0: 7074 7572 655f 6f72 6465 7272 1000 0000  pture_orderr....
-00000800: 2907 da04 7365 6c66 721b 0000 00da 0461  )...selfr......a
-00000810: 7267 73da 066b 7761 7267 73da 0970 6f73  rgs..kwargs..pos
-00000820: 745f 6469 6374 7234 0000 0072 1c00 0000  t_dictr4...r....
-00000830: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000840: 0470 6f73 742c 0000 0073 2200 0000 0001  .post,...s".....
-00000850: 1201 0a01 0a01 0a02 0201 0201 0400 04ff  ................
-00000860: 04ff 0606 0e02 0801 1601 1601 0801 1602  ................
-00000870: 7a16 5061 7970 616c 5765 6268 6f6f 6b56  z.PaypalWebhookV
-00000880: 6965 772e 706f 7374 4e29 0472 1500 0000  iew.postN).r....
-00000890: 7216 0000 0072 1700 0000 7249 0000 0072  r....r....rI...r
-000008a0: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-000008b0: 0000 0072 3300 0000 2a00 0000 7302 0000  ...r3...*...s...
-000008c0: 0008 0272 3300 0000 2920 723b 0000 00da  ...r3...) r;....
-000008d0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-000008e0: 00da 0b64 6a61 6e67 6f2e 636f 6e66 7204  ...django.confr.
-000008f0: 0000 00da 0b64 6a61 6e67 6f2e 6874 7470  .....django.http
-00000900: 7205 0000 0072 0600 0000 da17 646a 616e  r....r......djan
-00000910: 676f 2e75 7469 6c73 2e64 6563 6f72 6174  go.utils.decorat
-00000920: 6f72 7372 0700 0000 da1c 646a 616e 676f  orsr......django
-00000930: 2e76 6965 7773 2e64 6563 6f72 6174 6f72  .views.decorator
-00000940: 732e 6373 7266 7208 0000 00da 1464 6a61  s.csrfr......dja
-00000950: 6e67 6f2e 7669 6577 732e 6765 6e65 7269  ngo.views.generi
-00000960: 6372 0900 0000 da09 6170 695f 7479 7065  cr......api_type
-00000970: 7372 0b00 0000 da06 6d6f 6465 6c73 720c  sr......modelsr.
-00000980: 0000 0072 0d00 0000 720e 0000 00da 0773  ...r....r......s
-00000990: 6967 6e61 6c73 720f 0000 0072 1000 0000  ignalsr....r....
-000009a0: da08 7772 6170 7065 7273 7211 0000 00da  ..wrappersr.....
-000009b0: 0d64 6a61 6e67 6f5f 7061 7970 616c 723f  .django_paypalr?
-000009c0: 0000 0072 1200 0000 da03 7374 7272 3000  ...r......strr0.
-000009d0: 0000 7233 0000 0072 1900 0000 7219 0000  ..r3...r....r...
-000009e0: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
-000009f0: 6475 6c65 3e01 0000 0073 1e00 0000 0801  dule>....s......
-00000a00: 1002 0c01 1001 0c01 0c01 0c02 0c01 1401  ................
-00000a10: 1001 0c01 0c03 0e04 1a15 0a01            ............
+00000370: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+00000380: 0900 0000 4300 0000 737c 0000 0074 006a  ....C...s|...t.j
+00000390: 0173 7874 026a 036a 047c 00a0 05a1 0064  .sxt.j.j.|.....d
+000003a0: 018d 017d 037c 01a0 067c 007c 036a 07a1  ...}.|...|.|.j..
+000003b0: 0201 007a 1a74 086a 036a 047c 0264 0219  ...z.t.j.j.|.d..
+000003c0: 0064 0319 0064 048d 017d 0457 006e 1c04  .d...d...}.W.n..
+000003d0: 0074 0974 0a66 026b 0a72 5c01 0001 0001  .t.t.f.k.r\.....
+000003e0: 0064 007d 0459 006e 0258 007c 027c 037c  .d.}.Y.n.X.|.|.|
+000003f0: 0464 059c 037d 0574 0b6a 036a 0c66 007c  .d...}.t.j.j.f.|
+00000400: 058e 0101 0064 0053 0029 064e 2901 da03  .....d.S.).N)...
+00000410: 7572 6cda 0872 6573 6f75 7263 65da 0269  url..resource..i
+00000420: 6429 01da 086f 7264 6572 5f69 6429 0372  d)...order_id).r
+00000430: 1d00 0000 da07 7765 6268 6f6f 6bda 056f  ......webhook..o
+00000440: 7264 6572 290d 7204 0000 00da 0544 4542  rder).r......DEB
+00000450: 5547 720c 0000 00da 076f 626a 6563 7473  UGr......objects
+00000460: da03 6765 74da 1262 7569 6c64 5f61 6273  ..get..build_abs
+00000470: 6f6c 7574 655f 7572 69da 1476 6572 6966  olute_uri..verif
+00000480: 795f 7765 6268 6f6f 6b5f 6576 656e 74da  y_webhook_event.
+00000490: 0a77 6562 686f 6f6b 5f69 6472 0e00 0000  .webhook_idr....
+000004a0: da08 4b65 7945 7272 6f72 da09 5479 7065  ..KeyError..Type
+000004b0: 4572 726f 7272 0d00 0000 da06 6372 6561  Errorr......crea
+000004c0: 7465 2906 721b 0000 0072 1c00 0000 721d  te).r....r....r.
+000004d0: 0000 00da 0e70 6179 7061 6c5f 7765 6268  .....paypal_webh
+000004e0: 6f6f 6bda 0c70 6179 7061 6c5f 6f72 6465  ook..paypal_orde
+000004f0: 725a 0a65 7665 6e74 5f64 6174 6172 1900  rZ.event_datar..
+00000500: 0000 7219 0000 0072 1a00 0000 da1d 7665  ..r....r......ve
+00000510: 7269 6679 5f61 6e64 5f73 6176 655f 7765  rify_and_save_we
+00000520: 6268 6f6f 6b5f 6576 656e 7415 0000 0073  bhook_event....s
+00000530: 1200 0000 0001 0601 1201 0e01 0201 1a01  ................
+00000540: 1201 0a01 0c01 722f 0000 00da 0864 6973  ......r/.....dis
+00000550: 7061 7463 6829 01da 046e 616d 6563 0000  patch)...namec..
+00000560: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000570: 0000 4000 0000 7314 0000 0065 005a 0164  ..@...s....e.Z.d
+00000580: 005a 0264 0164 0284 005a 0364 0353 0029  .Z.d.d...Z.d.S.)
+00000590: 04da 1150 6179 7061 6c57 6562 686f 6f6b  ...PaypalWebhook
+000005a0: 5669 6577 6302 0000 0000 0000 0000 0000  Viewc...........
+000005b0: 0007 0000 0005 0000 004f 0000 0073 b000  .........O...s..
+000005c0: 0000 7400 a001 7c01 6a02 a003 6401 a101  ..t...|.j...d...
+000005d0: a101 7d04 7c04 a004 6402 a101 7d05 7c05  ..}.|...d...}.|.
+000005e0: 7405 6a06 6b07 7230 7407 6403 6404 8d01  t.j.k.r0t.d.d...
+000005f0: 5300 7408 7409 740a 6a0b 740a 6a0c 6405  S.t.t.t.j.t.j.d.
+00000600: 8d02 6406 8d01 7d06 740d 7c01 7c06 7c04  ..d...}.t.|.|.|.
+00000610: 6407 8d03 0100 7c05 6408 6b02 7288 740e  d.....|.d.k.r.t.
+00000620: 6a0f 7c00 6a10 7c04 a004 6409 a101 640a  j.|.j.|...d...d.
+00000630: 8d02 0100 7c06 a011 7c04 a004 6409 a101  ....|...|...d...
+00000640: a004 640b a101 a101 0100 7c05 640c 6b02  ..d.......|.d.k.
+00000650: 72a6 7412 6a0f 7c00 6a10 7c04 a004 6409  r.t.j.|.j.|...d.
+00000660: a101 640a 8d02 0100 7407 640d 6404 8d01  ..d.....t.d.d...
+00000670: 5300 290e 4e7a 0575 7466 2d38 da0a 6576  S.).Nz.utf-8..ev
+00000680: 656e 745f 7479 7065 6990 0100 0029 01da  ent_typei....)..
+00000690: 0673 7461 7475 7329 02da 0963 6c69 656e  .status)...clien
+000006a0: 745f 6964 da0d 636c 6965 6e74 5f73 6563  t_id..client_sec
+000006b0: 7265 7429 01da 0461 7574 6829 0172 1d00  ret)...auth).r..
+000006c0: 0000 7214 0000 0072 1f00 0000 2902 da06  ..r....r....)...
+000006d0: 7365 6e64 6572 721f 0000 0072 2000 0000  senderr....r ...
+000006e0: 7213 0000 00e9 c800 0000 2913 da04 6a73  r.........)...js
+000006f0: 6f6e da05 6c6f 6164 73da 0462 6f64 79da  on..loads..body.
+00000700: 0664 6563 6f64 6572 2600 0000 7212 0000  .decoder&...r...
+00000710: 0072 1800 0000 7205 0000 0072 1100 0000  .r....r....r....
+00000720: 720b 0000 00da 1664 6a61 6e67 6f5f 7061  r......django_pa
+00000730: 7970 616c 5f73 6574 7469 6e67 73da 1450  ypal_settings..P
+00000740: 4159 5041 4c5f 4150 495f 434c 4945 4e54  AYPAL_API_CLIENT
+00000750: 5f49 44da 1150 4159 5041 4c5f 4150 495f  _ID..PAYPAL_API_
+00000760: 5345 4352 4554 722f 0000 0072 0f00 0000  SECRETr/...r....
+00000770: da04 7365 6e64 da09 5f5f 636c 6173 735f  ..send..__class_
+00000780: 5fda 0d63 6170 7475 7265 5f6f 7264 6572  _..capture_order
+00000790: 7210 0000 0029 07da 0473 656c 6672 1b00  r....)...selfr..
+000007a0: 0000 da04 6172 6773 da06 6b77 6172 6773  ....args..kwargs
+000007b0: da09 706f 7374 5f64 6963 7472 3300 0000  ..post_dictr3...
+000007c0: 721c 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+000007d0: 1a00 0000 da04 706f 7374 2300 0000 7322  ......post#...s"
+000007e0: 0000 0000 0112 010a 010a 010a 0202 0102  ................
+000007f0: 0104 0004 ff04 ff06 060e 0208 0116 0116  ................
+00000800: 0108 0116 027a 1650 6179 7061 6c57 6562  .....z.PaypalWeb
+00000810: 686f 6f6b 5669 6577 2e70 6f73 744e 2904  hookView.postN).
+00000820: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000830: 4800 0000 7219 0000 0072 1900 0000 7219  H...r....r....r.
+00000840: 0000 0072 1a00 0000 7232 0000 0021 0000  ...r....r2...!..
+00000850: 0073 0200 0000 0802 7232 0000 0029 2072  .s......r2...) r
+00000860: 3a00 0000 da06 7479 7069 6e67 7202 0000  :.....typingr...
+00000870: 0072 0300 0000 da0b 646a 616e 676f 2e63  .r......django.c
+00000880: 6f6e 6672 0400 0000 da0b 646a 616e 676f  onfr......django
+00000890: 2e68 7474 7072 0500 0000 7206 0000 00da  .httpr....r.....
+000008a0: 1764 6a61 6e67 6f2e 7574 696c 732e 6465  .django.utils.de
+000008b0: 636f 7261 746f 7273 7207 0000 00da 1c64  coratorsr......d
+000008c0: 6a61 6e67 6f2e 7669 6577 732e 6465 636f  jango.views.deco
+000008d0: 7261 746f 7273 2e63 7372 6672 0800 0000  rators.csrfr....
+000008e0: da14 646a 616e 676f 2e76 6965 7773 2e67  ..django.views.g
+000008f0: 656e 6572 6963 7209 0000 00da 0961 7069  enericr......api
+00000900: 5f74 7970 6573 720b 0000 00da 066d 6f64  _typesr......mod
+00000910: 656c 7372 0c00 0000 720d 0000 0072 0e00  elsr....r....r..
+00000920: 0000 da07 7369 676e 616c 7372 0f00 0000  ....signalsr....
+00000930: 7210 0000 00da 0877 7261 7070 6572 7372  r......wrappersr
+00000940: 1100 0000 da0d 646a 616e 676f 5f70 6179  ......django_pay
+00000950: 7061 6c72 3e00 0000 7212 0000 00da 0373  palr>...r......s
+00000960: 7472 722f 0000 0072 3200 0000 7219 0000  trr/...r2...r...
+00000970: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000980: da08 3c6d 6f64 756c 653e 0100 0000 731e  ..<module>....s.
+00000990: 0000 0008 0110 020c 0110 010c 010c 010c  ................
+000009a0: 020c 0114 0110 010c 010c 030e 041a 0c0a  ................
+000009b0: 01                                       .
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-311.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/__pycache__/wrappers.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/__pycache__/wrappers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 26 04:47:09 2024 UTC, .py size: 10412 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,529 +1,584 @@
-00000000: 550d 0d0a 0000 0000 cd31 2b66 ac28 0000  U........1+f.(..
+00000000: 550d 0d0a 0000 0000 97a9 3066 ab2c 0000  U.........0f.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
-00000060: 0100 6400 6404 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6402 6c0b 5a0b 6400 6405 6c0c 6d0d 5a0d  d.l.Z.d.d.l.m.Z.
-00000080: 0100 6400 6406 6c0e 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6407 6c10 6d11 5a12 0100 6400 6408 6c13  d.l.m.Z...d.d.l.
-000000a0: 6d14 5a14 6d15 5a15 6d16 5a16 0100 6400  m.Z.m.Z.m.Z...d.
-000000b0: 6409 6c17 6d18 5a18 6d19 5a19 6d1a 5a1a  d.l.m.Z.m.Z.m.Z.
-000000c0: 6d1b 5a1b 0100 6400 640a 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000d0: 6d1e 5a1e 6d1f 5a1f 6d20 5a20 6d21 5a21  m.Z.m.Z.m Z m!Z!
-000000e0: 6d22 5a22 6d23 5a23 6d24 5a24 6d25 5a25  m"Z"m#Z#m$Z$m%Z%
-000000f0: 0100 6400 640b 6c26 6d27 5a27 0100 6400  ..d.d.l&m'Z'..d.
-00000100: 640c 6c28 6d29 5a29 6d2a 5a2a 0100 4700  d.l(m)Z)m*Z*..G.
-00000110: 640d 640e 8400 640e 652b 8303 5a2c 6402  d.d...d.e+..Z,d.
-00000120: 5300 290f e900 0000 0029 01da 1075 6e69  S.)......)...uni
-00000130: 636f 6465 5f6c 6974 6572 616c 734e 2904  code_literalsN).
-00000140: da07 4c69 7465 7261 6cda 044c 6973 74da  ..Literal..List.
-00000150: 0341 6e79 da04 4469 6374 2901 da05 6361  .Any..Dict)...ca
-00000160: 6368 6529 01da 0b48 7474 7052 6571 7565  che)...HttpReque
-00000170: 7374 2901 da0d 4854 5450 4261 7369 6341  st)...HTTPBasicA
-00000180: 7574 6829 01da 0873 6574 7469 6e67 7329  uth)...settings)
-00000190: 03da 1150 6179 7061 6c41 7574 6846 6169  ...PaypalAuthFai
-000001a0: 6c75 7265 da0e 5061 7970 616c 4150 4945  lure..PaypalAPIE
-000001b0: 7272 6f72 da1e 5061 7970 616c 5765 6268  rror..PaypalWebh
-000001c0: 6f6f 6b56 6572 6966 6963 6174 696f 6e45  ookVerificationE
-000001d0: 7272 6f72 2904 da0b 5061 7970 616c 4f72  rror)...PaypalOr
-000001e0: 6465 72da 1150 6179 7061 6c41 5049 506f  der..PaypalAPIPo
-000001f0: 7374 4461 7461 da11 5061 7970 616c 4150  stData..PaypalAP
-00000200: 4952 6573 706f 6e73 65da 0d50 6179 7061  IResponse..Paypa
-00000210: 6c57 6562 686f 6f6b 2909 da0d 4f41 7574  lWebhook)...OAut
-00000220: 6852 6573 706f 6e73 65da 0d50 6179 6d65  hResponse..Payme
-00000230: 6e74 536f 7572 6365 da12 4170 706c 6963  ntSource..Applic
-00000240: 6174 696f 6e43 6f6e 7465 7874 da11 4578  ationContext..Ex
-00000250: 7065 7269 656e 6365 436f 6e74 6578 74da  perienceContext.
-00000260: 0c50 7572 6368 6173 6555 6e69 74da 1241  .PurchaseUnit..A
-00000270: 5049 4175 7468 4372 6564 656e 7469 616c  PIAuthCredential
-00000280: 73da 174f 7264 6572 4372 6561 7465 6441  s..OrderCreatedA
-00000290: 5049 5265 7370 6f6e 7365 da17 4f72 6465  PIResponse..Orde
-000002a0: 7243 6170 7475 7265 4150 4952 6573 706f  rCaptureAPIRespo
-000002b0: 6e73 65da 164f 7264 6572 4465 7461 696c  nse..OrderDetail
-000002c0: 4150 4952 6573 706f 6e73 6529 01da 1562  APIResponse)...b
-000002d0: 7569 6c64 5f70 6179 7061 6c5f 6675 6c6c  uild_paypal_full
-000002e0: 5f75 7269 2902 da0e 6f72 6465 725f 6361  _uri)...order_ca
-000002f0: 7074 7572 6564 da0d 6f72 6465 725f 6372  ptured..order_cr
-00000300: 6561 7465 6463 0000 0000 0000 0000 0000  eatedc..........
-00000310: 0000 0000 0000 0700 0000 0000 0000 7320  ..............s 
-00000320: 0100 0065 005a 0164 005a 0255 0064 01a0  ...e.Z.d.Z.U.d..
-00000330: 0365 046a 05a1 015a 0665 046a 075a 0865  .e.j...Z.e.j.Z.e
-00000340: 046a 095a 0a65 046a 0b5a 0c65 046a 0d5a  .j.Z.e.j.Z.e.j.Z
-00000350: 0e65 046a 0f5a 1065 046a 115a 1264 025a  .e.j.Z.e.j.Z.d.Z
-00000360: 1365 1465 1564 033c 0064 2265 1464 049c  .e.e.d.<.d"e.d..
-00000370: 0187 0066 0164 0564 0684 0d5a 1664 0265  ...f.d.d...Z.d.e
-00000380: 046a 1765 046a 1866 0365 1964 0719 0065  .j.e.j.f.e.d...e
-00000390: 1a65 1b19 0065 1c65 1d65 1e64 089c 0564  .e...e.e.e.d...d
-000003a0: 0964 0a84 055a 1f65 2065 2164 0b9c 0264  .d...Z.e e!d...d
-000003b0: 0c64 0d84 045a 2265 2065 2364 0b9c 0264  .d...Z"e e#d...d
-000003c0: 0e64 0f84 045a 2464 2365 2065 1964 1019  .d...Z$d#e e.d..
-000003d0: 0065 2565 2065 2666 0219 0064 119c 0364  .e%e e&f...d...d
-000003e0: 1264 1384 055a 2765 2065 2864 149c 0264  .d...Z'e e(d...d
-000003f0: 1564 1684 045a 2965 2065 1a65 2519 0065  .d...Z)e e.e%..e
-00000400: 2864 179c 0364 1864 1984 045a 2a65 2b65  (d...d.d...Z*e+e
-00000410: 2065 2c64 1a9c 0364 1b64 1c84 045a 2d65   e,d...d.d...Z-e
-00000420: 2064 1d9c 0164 1e64 1f84 045a 2e65 2f64   d...d.d...Z.e/d
-00000430: 1d9c 0164 2064 2184 045a 3087 0004 005a  ...d d!..Z0....Z
-00000440: 3153 0029 24da 0d50 6179 7061 6c57 7261  1S.)$..PaypalWra
-00000450: 7070 6572 7a11 646a 616e 676f 5f70 6179  pperz.django_pay
-00000460: 7061 6c5f 767b 7d4e da04 6175 7468 2901  pal_v{}N..auth).
-00000470: 721f 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000480: 0000 0300 0000 0300 0000 0300 0000 732a  ..............s*
-00000490: 0000 0074 0074 017c 0083 02a0 02a1 0001  ...t.t.|........
-000004a0: 007c 017c 005f 037c 0273 1e74 046a 0572  .|.|._.|.s.t.j.r
-000004b0: 267c 006a 067c 005f 0764 0053 00a9 014e  &|.j.|._.d.S...N
-000004c0: 2908 da05 7375 7065 7272 1e00 0000 da08  )...superr......
-000004d0: 5f5f 696e 6974 5f5f 721f 0000 00da 1664  __init__r......d
-000004e0: 6a61 6e67 6f5f 7061 7970 616c 5f73 6574  jango_paypal_set
-000004f0: 7469 6e67 73da 0e50 4159 5041 4c5f 5341  tings..PAYPAL_SA
-00000500: 4e44 424f 58da 0b73 616e 6462 6f78 5f75  NDBOX..sandbox_u
-00000510: 726c da07 6170 695f 7572 6c29 03da 0473  rl..api_url)...s
-00000520: 656c 6672 1f00 0000 da07 7361 6e64 626f  elfr......sandbo
-00000530: 78a9 01da 095f 5f63 6c61 7373 5f5f a900  x....__class__..
-00000540: fa5d 2f55 7365 7273 2f74 696d 7461 6d2f  .]/Users/timtam/
-00000550: 2e70 7965 6e76 2f76 6572 7369 6f6e 732f  .pyenv/versions/
-00000560: 7366 2d33 2e38 2e31 322f 6c69 622f 7079  sf-3.8.12/lib/py
-00000570: 7468 6f6e 332e 382f 7369 7465 2d70 6163  thon3.8/site-pac
-00000580: 6b61 6765 732f 646a 616e 676f 5f70 6179  kages/django_pay
-00000590: 7061 6c2f 7772 6170 7065 7273 2e70 7972  pal/wrappers.pyr
-000005a0: 2200 0000 2f00 0000 7308 0000 0000 010e  ".../...s.......
-000005b0: 0106 010a 017a 1650 6179 7061 6c57 7261  .....z.PaypalWra
-000005c0: 7070 6572 2e5f 5f69 6e69 745f 5f29 02da  pper.__init__)..
-000005d0: 0743 4150 5455 5245 5a09 4155 5448 4f52  .CAPTUREZ.AUTHOR
-000005e0: 495a 4529 05da 0669 6e74 656e 74da 0e70  IZE)...intent..p
-000005f0: 7572 6368 6173 655f 756e 6974 73da 0e70  urchase_units..p
-00000600: 6179 6d65 6e74 5f73 6f75 7263 65da 1361  ayment_source..a
-00000610: 7070 6c69 6361 7469 6f6e 5f63 6f6e 7465  pplication_conte
-00000620: 7874 da06 7265 7475 726e 6307 0000 0000  xt..returnc.....
-00000630: 0000 0000 0000 000d 0000 0006 0000 0043  ...............C
-00000640: 0000 0073 1a01 0000 7c03 6a00 7260 7c05  ...s....|.j.r`|.
-00000650: 730e 7c06 7260 7c03 6a00 6a01 7330 7402  s.|.r`|.j.j.s0t.
-00000660: 7403 7c05 8301 7403 7c06 8301 6401 8d02  t.|...t.|...d...
-00000670: 7c03 6a00 5f01 6e30 7c03 6a00 6a01 6a04  |.j._.n0|.j.j.j.
-00000680: 7348 7403 7c05 8301 7c03 6a00 6a01 5f04  sHt.|...|.j.j._.
-00000690: 7c03 6a00 6a01 6a05 7360 7403 7c06 8301  |.j.j.j.s`t.|...
-000006a0: 7c03 6a00 6a01 5f05 7c01 6402 6403 8400  |.j.j._.|.d.d...
-000006b0: 7c02 4400 8301 6404 9c02 7d07 7c03 728a  |.D...d...}.|.r.
-000006c0: 7c07 a006 6405 7c03 a007 a100 6901 a101  |...d.|.....i...
-000006d0: 0100 7c04 72a0 7c07 a006 6406 7c04 a007  ..|.r.|...d.|...
-000006e0: a100 6901 a101 0100 6407 a008 7c00 6a09  ..i.....d...|.j.
-000006f0: 7c00 6a0a a102 7d08 7c00 6a0b 7c08 7c07  |.j...}.|.j.|.|.
-00000700: 6408 6409 8d03 7d09 740c a00d 7c09 a101  d.d...}.t...|...
-00000710: 7d0a 740e 6a0f 6a10 7c0a 6a11 7c0a 6a12  }.t.j.j.|.j.|.j.
-00000720: 640a 8d02 7d0b 7413 6a0f 6a10 7c0b 7c08  d...}.t.j.j.|.|.
-00000730: 7c07 640b 8d03 7d0c 7414 6a0f 6a10 7c0b  |.d...}.t.j.j.|.
-00000740: 7c08 7c09 7c0c 640c 8d04 0100 7415 6a16  |.|.|.d.....t.j.
-00000750: 7c00 6a17 7c0b 7c09 640d 8d03 0100 7c0a  |.j.|.|.d.....|.
-00000760: 5300 290e 4e29 02da 0a72 6574 7572 6e5f  S.).N)...return_
-00000770: 7572 6cda 0a63 616e 6365 6c5f 7572 6c63  url..cancel_urlc
-00000780: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000790: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-000007a0: 005d 0c7d 017c 01a0 00a1 0091 0271 0453  .].}.|.......q.S
-000007b0: 0072 2b00 0000 2901 da07 746f 5f64 6963  .r+...)...to_dic
-000007c0: 7429 02da 022e 30da 0d70 7572 6368 6173  t)....0..purchas
-000007d0: 655f 756e 6974 722b 0000 0072 2b00 0000  e_unitr+...r+...
-000007e0: 722c 0000 00da 0a3c 6c69 7374 636f 6d70  r,.....<listcomp
-000007f0: 3e4a 0000 0073 0400 0000 0600 0200 7a2e  >J...s........z.
-00000800: 5061 7970 616c 5772 6170 7065 722e 6372  PaypalWrapper.cr
-00000810: 6561 7465 5f6f 7264 6572 2e3c 6c6f 6361  eate_order.<loca
-00000820: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2902  ls>.<listcomp>).
-00000830: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00000840: 3100 0000 fa06 7b30 7d7b 317d da04 504f  1.....{0}{1}..PO
-00000850: 5354 2903 da03 7572 6cda 0464 6174 61da  ST)...url..data.
-00000860: 066d 6574 686f 6429 02da 086f 7264 6572  .method)...order
-00000870: 5f69 64da 0673 7461 7475 73a9 03da 056f  _id..status....o
-00000880: 7264 6572 723b 0000 00da 0970 6f73 745f  rderr;.....post_
-00000890: 6461 7461 a904 7241 0000 0072 3b00 0000  data..rA...r;...
-000008a0: da0d 7265 7370 6f6e 7365 5f64 6174 61da  ..response_data.
-000008b0: 0470 6f73 74a9 03da 0673 656e 6465 7272  .post....senderr
-000008c0: 4100 0000 da08 7265 7370 6f6e 7365 2918  A.....response).
-000008d0: da06 7061 7970 616c da12 6578 7065 7269  ..paypal..experi
-000008e0: 656e 6365 5f63 6f6e 7465 7874 7215 0000  ence_contextr...
-000008f0: 0072 1b00 0000 7233 0000 0072 3400 0000  .r....r3...r4...
-00000900: da06 7570 6461 7465 7235 0000 00da 0666  ..updater5.....f
-00000910: 6f72 6d61 7472 2600 0000 da13 6f72 6465  ormatr&.....orde
-00000920: 7273 5f61 7069 5f65 6e64 706f 696e 74da  rs_api_endpoint.
-00000930: 0863 616c 6c5f 6170 6972 1800 0000 da09  .call_apir......
-00000940: 6672 6f6d 5f64 6963 7472 0e00 0000 da07  from_dictr......
-00000950: 6f62 6a65 6374 73da 0663 7265 6174 65da  objects..create.
-00000960: 0269 6472 3f00 0000 720f 0000 0072 1000  .idr?...r....r..
-00000970: 0000 721d 0000 00da 0473 656e 6472 2a00  ..r......sendr*.
-00000980: 0000 290d 7227 0000 0072 2e00 0000 722f  ..).r'...r....r/
-00000990: 0000 0072 3000 0000 7231 0000 00da 0b73  ...r0...r1.....s
-000009a0: 7563 6365 7373 5f75 726c da10 6361 6e63  uccess_url..canc
-000009b0: 656c 6c61 7469 6f6e 5f75 726c 5a0a 6f72  ellation_urlZ.or
-000009c0: 6465 725f 6461 7461 723b 0000 005a 136f  der_datar;...Z.o
-000009d0: 7264 6572 5f72 6573 706f 6e73 655f 6469  rder_response_di
-000009e0: 6374 5a0e 6f72 6465 725f 7265 7370 6f6e  ctZ.order_respon
-000009f0: 7365 5a09 6e65 775f 6f72 6465 72da 0870  seZ.new_order..p
-00000a00: 6f73 745f 6f62 6a72 2b00 0000 722b 0000  ost_objr+...r+..
-00000a10: 0072 2c00 0000 da0c 6372 6561 7465 5f6f  .r,.....create_o
-00000a20: 7264 6572 3500 0000 732e 0000 0000 090e  rder5...s.......
-00000a30: 0108 0102 0106 0106 fe0c 050a 010e 010a  ................
-00000a40: 010e 0214 0104 0112 0104 0112 0210 0110  ................
-00000a50: 010a 0114 0112 0114 0112 017a 1a50 6179  ...........z.Pay
-00000a60: 7061 6c57 7261 7070 6572 2e63 7265 6174  palWrapper.creat
-00000a70: 655f 6f72 6465 7229 0272 3e00 0000 7232  e_order).r>...r2
-00000a80: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000a90: 0700 0000 0600 0000 4300 0000 7392 0000  ........C...s...
-00000aa0: 0074 006a 016a 027c 0164 018d 017d 027c  .t.j.j.|.d...}.|
-00000ab0: 006a 039b 007c 006a 049b 0064 027c 026a  .j...|.j...d.|.j
-00000ac0: 059b 0064 039d 057d 037c 006a 067c 0364  ...d...}.|.j.|.d
-00000ad0: 0464 058d 027d 0474 07a0 087c 04a1 017d  .d...}.t...|...}
-00000ae0: 057c 056a 097c 025f 097c 026a 0a64 0667  .|.j.|._.|.j.d.g
-00000af0: 0164 078d 0101 0074 0b6a 016a 0c7c 027c  .d.....t.j.j.|.|
-00000b00: 0369 0064 088d 037d 0674 0d6a 016a 0c7c  .i.d...}.t.j.j.|
-00000b10: 027c 037c 047c 0664 098d 0401 0074 0e6a  .|.|.|.d.....t.j
-00000b20: 0f7c 006a 107c 027c 0464 0a8d 0301 007c  .|.j.|.|.d.....|
-00000b30: 0553 0029 0b4e a901 723e 0000 00fa 012f  .S.).N..r>...../
-00000b40: 7a08 2f63 6170 7475 7265 723a 0000 00a9  z./capturer:....
-00000b50: 0272 3b00 0000 723d 0000 0072 3f00 0000  .r;...r=...r?...
-00000b60: 2901 da0d 7570 6461 7465 5f66 6965 6c64  )...update_field
-00000b70: 7372 4000 0000 7243 0000 0072 4600 0000  sr@...rC...rF...
-00000b80: 2911 720e 0000 0072 5000 0000 da03 6765  ).r....rP.....ge
-00000b90: 7472 2600 0000 724d 0000 0072 3e00 0000  tr&...rM...r>...
-00000ba0: 724e 0000 0072 1900 0000 724f 0000 0072  rN...r....rO...r
-00000bb0: 3f00 0000 da04 7361 7665 720f 0000 0072  ?.....saver....r
-00000bc0: 5100 0000 7210 0000 0072 1c00 0000 7253  Q...r....r....rS
-00000bd0: 0000 0072 2a00 0000 2907 7227 0000 0072  ...r*...).r'...r
-00000be0: 3e00 0000 7241 0000 0072 3b00 0000 5a16  >...rA...r;...Z.
-00000bf0: 6f72 6465 725f 6361 7074 7572 655f 7265  order_capture_re
-00000c00: 7370 6f6e 7365 5a0d 6f72 6465 725f 6361  sponseZ.order_ca
-00000c10: 7074 7572 6572 5600 0000 722b 0000 0072  pturerV...r+...r
-00000c20: 2b00 0000 722c 0000 00da 0d63 6170 7475  +...r,.....captu
-00000c30: 7265 5f6f 7264 6572 5900 0000 7314 0000  re_orderY...s...
-00000c40: 0000 010e 011a 010e 010a 0108 010e 0112  ................
-00000c50: 0114 0112 017a 1b50 6179 7061 6c57 7261  .....z.PaypalWra
-00000c60: 7070 6572 2e63 6170 7475 7265 5f6f 7264  pper.capture_ord
-00000c70: 6572 6302 0000 0000 0000 0000 0000 0005  erc.............
-00000c80: 0000 0004 0000 0043 0000 0073 3e00 0000  .......C...s>...
-00000c90: 7400 6a01 6a02 7c01 6401 8d01 7d02 7c00  t.j.j.|.d...}.|.
-00000ca0: 6a03 9b00 7c00 6a04 9b00 6402 7c02 6a05  j...|.j...d.|.j.
-00000cb0: 9b00 9d04 7d03 7c00 6a06 7c03 6403 6404  ....}.|.j.|.d.d.
-00000cc0: 8d02 7d04 7407 a008 7c04 a101 5300 2905  ..}.t...|...S.).
-00000cd0: 4e72 5800 0000 7259 0000 00da 0347 4554  NrX...rY.....GET
-00000ce0: 725a 0000 0029 0972 0e00 0000 7250 0000  rZ...).r....rP..
-00000cf0: 0072 5c00 0000 7226 0000 0072 4d00 0000  .r\...r&...rM...
-00000d00: 723e 0000 0072 4e00 0000 721a 0000 0072  r>...rN...r....r
-00000d10: 4f00 0000 2905 7227 0000 0072 3e00 0000  O...).r'...r>...
-00000d20: 7241 0000 0072 3b00 0000 5a16 6f72 6465  rA...r;...Z.orde
-00000d30: 725f 6465 7461 696c 735f 7265 7370 6f6e  r_details_respon
-00000d40: 7365 722b 0000 0072 2b00 0000 722c 0000  ser+...r+...r,..
-00000d50: 00da 1167 6574 5f6f 7264 6572 5f64 6574  ...get_order_det
-00000d60: 6169 6c73 6500 0000 7308 0000 0000 010e  ailse...s.......
-00000d70: 0118 010e 017a 1f50 6179 7061 6c57 7261  .....z.PaypalWra
-00000d80: 7070 6572 2e67 6574 5f6f 7264 6572 5f64  pper.get_order_d
-00000d90: 6574 6169 6c73 2903 725f 0000 0072 3a00  etails).r_...r:.
-00000da0: 0000 da05 5041 5443 4829 0372 3b00 0000  ....PATCH).r;...
-00000db0: 723d 0000 0072 3200 0000 6304 0000 0000  r=...r2...c.....
-00000dc0: 0000 0000 0000 0008 0000 000a 0000 0043  ...............C
-00000dd0: 0000 0073 ba00 0000 6401 7c00 a000 a100  ...s....d.|.....
-00000de0: 9b00 9d02 6402 6403 9c02 7d04 7a6a 7c02  ....d.d...}.zj|.
-00000df0: 6404 6b02 722e 7401 6a02 7c01 7c04 6405  d.k.r.t.j.|.|.d.
-00000e00: 8d02 7d05 6e3c 7c02 6406 6b02 7248 7401  ..}.n<|.d.k.rHt.
-00000e10: 6a03 7c01 7c04 7c03 6407 8d03 7d05 6e22  j.|.|.|.d...}.n"
-00000e20: 7c02 6408 6b02 7262 7401 6a04 7c01 7c04  |.d.k.rbt.j.|.|.
-00000e30: 7c03 6407 8d03 7d05 6e08 7405 6409 8301  |.d...}.n.t.d...
-00000e40: 8201 7c05 a006 a100 0100 7c05 a007 a100  ..|.......|.....
-00000e50: 7d06 7c06 5700 5300 0400 7401 6a08 6b0a  }.|.W.S...t.j.k.
-00000e60: 72b4 0100 7d07 0100 7a16 7409 740a 7c07  r...}...z.t.t.|.
-00000e70: 8301 7c07 6a0b 640a 8d02 8201 5700 3500  ..|.j.d.....W.5.
-00000e80: 6400 7d07 7e07 5800 5900 6e02 5800 6400  d.}.~.X.Y.n.X.d.
-00000e90: 5300 290b 4e7a 0742 6561 7265 7220 fa10  S.).Nz.Bearer ..
-00000ea0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00000eb0: 2902 da0d 4175 7468 6f72 697a 6174 696f  )...Authorizatio
-00000ec0: 6efa 0c43 6f6e 7465 6e74 2d54 7970 6572  n..Content-Typer
-00000ed0: 5f00 0000 2901 da07 6865 6164 6572 7372  _...)...headersr
-00000ee0: 3a00 0000 2902 7265 0000 00da 046a 736f  :...).re.....jso
-00000ef0: 6e72 6100 0000 7a0e 496e 7661 6c69 6420  nra...z.Invalid 
-00000f00: 6d65 7468 6f64 a901 7248 0000 0029 0cda  method..rH...)..
-00000f10: 115f 6765 745f 6163 6365 7373 5f74 6f6b  ._get_access_tok
-00000f20: 656e da08 7265 7175 6573 7473 725c 0000  en..requestsr\..
-00000f30: 0072 4500 0000 da05 7061 7463 68da 0a56  .rE.....patch..V
-00000f40: 616c 7565 4572 726f 72da 1072 6169 7365  alueError..raise
-00000f50: 5f66 6f72 5f73 7461 7475 7372 6600 0000  _for_statusrf...
-00000f60: da09 4854 5450 4572 726f 7272 0c00 0000  ..HTTPErrorr....
-00000f70: da03 7374 7272 4800 0000 2908 7227 0000  ..strrH...).r'..
-00000f80: 0072 3b00 0000 723d 0000 0072 3c00 0000  .r;...r=...r<...
-00000f90: 7265 0000 0072 4800 0000 da0d 7265 7370  re...rH.....resp
-00000fa0: 6f6e 7365 5f6a 736f 6eda 0165 722b 0000  onse_json..er+..
-00000fb0: 0072 2b00 0000 722c 0000 0072 4e00 0000  .r+...r,...rN...
-00000fc0: 6b00 0000 731c 0000 0000 0114 0202 0108  k...s...........
-00000fd0: 0110 0108 0112 0108 0112 0208 0108 0108  ................
-00000fe0: 0106 0112 017a 1650 6179 7061 6c57 7261  .....z.PaypalWra
-00000ff0: 7070 6572 2e63 616c 6c5f 6170 6929 02da  pper.call_api)..
-00001000: 1077 6562 686f 6f6b 5f6c 6973 7465 6e65  .webhook_listene
-00001010: 7272 3200 0000 6302 0000 0000 0000 0000  rr2...c.........
-00001020: 0000 000a 0000 000a 0000 0043 0000 0073  ...........C...s
-00001030: 2001 0000 7400 6a01 6a02 7c01 6401 8d01   ...t.j.j.|.d...
-00001040: a003 a100 7222 7404 6402 7c01 9b00 6403  ....r"t.d.|...d.
-00001050: 9d03 8301 8201 6404 6405 6c05 6d06 7d02  ......d.d.l.m.}.
-00001060: 0100 7c01 6406 6407 8400 7c02 6a07 4400  ..|.d.d...|.j.D.
-00001070: 8301 6408 9c02 7d03 6409 a008 7c00 6a09  ..d...}.d...|.j.
-00001080: 640a a102 7d04 7a30 7c00 6a0a 7c04 640b  d...}.z0|.j.|.d.
-00001090: 7c03 640c 8d03 7d05 7400 6a01 6a0b 7c05  |.d...}.t.j.j.|.
-000010a0: 640d 1900 7c05 640e 1900 7c05 640f 1900  d...|.d...|.d...
-000010b0: 6410 8d03 5700 5300 0400 740c 6b0a 9001  d...W.S...t.k...
-000010c0: 721a 0100 7d06 0100 7a78 7c06 6a0d a00e  r...}...zx|.j...
-000010d0: a100 7d07 7c07 a00f 6411 a101 6412 6b02  ..}.|...d...d.k.
-000010e0: 9001 7206 7c00 6a0a 7c04 6413 6414 8d02  ..r.|.j.|.d.d...
-000010f0: 7d08 7c08 a00f 6415 6700 a102 4400 5d3a  }.|...d.g...D.]:
-00001100: 7d09 7c09 640e 1900 7c01 6b02 72ca 7400  }.|.d...|.k.r.t.
-00001110: 6a01 6a0b 7c09 640d 1900 7c09 640e 1900  j.j.|.d...|.d...
-00001120: 7c09 640f 1900 6410 8d03 0200 0100 0600  |.d...d.........
-00001130: 5700 5900 a20c 5300 71ca 7c06 8201 5700  W.Y...S.q.|...W.
-00001140: 3500 6400 7d06 7e06 5800 5900 6e02 5800  5.d.}.~.X.Y.n.X.
-00001150: 6400 5300 2916 4e29 0172 3b00 0000 7a12  d.S.).N).r;...z.
-00001160: 5765 6268 6f6f 6b20 6c69 7374 656e 6572  Webhook listener
-00001170: 2028 7a10 2920 616c 7265 6164 7920 6578   (z.) already ex
-00001180: 6973 7473 7201 0000 0029 01da 0d57 6562  istsr....)...Web
-00001190: 686f 6f6b 4576 656e 7473 6301 0000 0000  hookEventsc.....
-000011a0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-000011b0: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-000011c0: 6400 7c01 6901 9102 7104 5300 2901 da04  d.|.i...q.S.)...
-000011d0: 6e61 6d65 722b 0000 0029 0272 3600 0000  namer+...).r6...
-000011e0: da05 6576 656e 7472 2b00 0000 722b 0000  ..eventr+...r+..
-000011f0: 0072 2c00 0000 7238 0000 0082 0000 0073  .r,...r8.......s
-00001200: 0400 0000 0600 0200 7a30 5061 7970 616c  ........z0Paypal
-00001210: 5772 6170 7065 722e 7365 7475 705f 7765  Wrapper.setup_we
-00001220: 6268 6f6f 6b73 2e3c 6c6f 6361 6c73 3e2e  bhooks.<locals>.
-00001230: 3c6c 6973 7463 6f6d 703e 2902 723b 0000  <listcomp>).r;..
-00001240: 00da 0b65 7665 6e74 5f74 7970 6573 7239  ...event_typesr9
-00001250: 0000 007a 1a2f 7631 2f6e 6f74 6966 6963  ...z./v1/notific
-00001260: 6174 696f 6e73 2f77 6562 686f 6f6b 7372  ations/webhooksr
-00001270: 3a00 0000 a903 723b 0000 0072 3d00 0000  :.....r;...r=...
-00001280: 723c 0000 0072 5200 0000 723b 0000 0072  r<...rR...r;...r
-00001290: 7500 0000 2903 da0a 7765 6268 6f6f 6b5f  u...)...webhook_
-000012a0: 6964 723b 0000 0072 7500 0000 7273 0000  idr;...ru...rs..
-000012b0: 005a 1a57 4542 484f 4f4b 5f55 524c 5f41  .Z.WEBHOOK_URL_A
-000012c0: 4c52 4541 4459 5f45 5849 5354 5372 5f00  LREADY_EXISTSr_.
-000012d0: 0000 725a 0000 00da 0877 6562 686f 6f6b  ..rZ.....webhook
-000012e0: 7329 1072 1100 0000 7250 0000 00da 0666  s).r....rP.....f
-000012f0: 696c 7465 72da 0665 7869 7374 7372 6b00  ilter..existsrk.
-00001300: 0000 5a16 646a 616e 676f 5f70 6179 7061  ..Z.django_paypa
-00001310: 6c2e 7765 6268 6f6f 6b73 7272 0000 005a  l.webhooksrr...Z
-00001320: 064f 5244 4552 5372 4c00 0000 7226 0000  .ORDERSrL...r&..
-00001330: 0072 4e00 0000 7251 0000 0072 0c00 0000  .rN...rQ...r....
-00001340: 7248 0000 0072 6600 0000 725c 0000 0029  rH...rf...r\...)
-00001350: 0a72 2700 0000 7271 0000 0072 7200 0000  .r'...rq...rr...
-00001360: 723c 0000 005a 0b77 6562 686f 6f6b 5f61  r<...Z.webhook_a
-00001370: 7069 da0d 7265 7370 6f6e 7365 5f64 6963  pi..response_dic
-00001380: 7472 7000 0000 726f 0000 005a 0c77 6562  trp...ro...Z.web
-00001390: 686f 6f6b 5f6c 6973 74da 0777 6562 686f  hook_list..webho
-000013a0: 6f6b 722b 0000 0072 2b00 0000 722c 0000  okr+...r+...r,..
-000013b0: 00da 0e73 6574 7570 5f77 6562 686f 6f6b  ...setup_webhook
-000013c0: 737d 0000 0073 2800 0000 0001 1201 1001  s}...s(.........
-000013d0: 0c02 1601 0e01 0201 1001 0601 0600 0600  ................
-000013e0: 06ff 0803 1201 0a01 1001 0e01 1001 0c01  ................
-000013f0: 2c01 7a1c 5061 7970 616c 5772 6170 7065  ,.z.PaypalWrappe
-00001400: 722e 7365 7475 705f 7765 6268 6f6f 6b73  r.setup_webhooks
-00001410: 2903 7277 0000 00da 0a70 6174 6368 5f64  ).rw.....patch_d
-00001420: 6174 6172 3200 0000 6303 0000 0000 0000  atar2...c.......
-00001430: 0000 0000 0007 0000 000a 0000 0043 0000  .............C..
-00001440: 0073 9200 0000 7a12 7400 6a01 6a02 7c01  .s....z.t.j.j.|.
-00001450: 6401 8d01 7d03 5700 6e3a 0400 7400 6a03  d...}.W.n:..t.j.
-00001460: 6b0a 724c 0100 7d04 0100 7a1a 7404 a005  k.rL..}...z.t...
-00001470: 6402 7c01 9b00 6403 9d03 a101 0100 7c04  d.|...d.......|.
-00001480: 8201 5700 3500 6400 7d04 7e04 5800 5900  ..W.5.d.}.~.X.Y.
-00001490: 6e02 5800 6404 a006 7c00 6a07 6405 7c01  n.X.d...|.j.d.|.
-000014a0: 9b00 9d02 a102 7d05 7c00 6a08 7c05 6406  ......}.|.j.|.d.
-000014b0: 7c02 6407 8d03 7d06 7c06 6408 1900 7c03  |.d...}.|.d...|.
-000014c0: 5f09 7c06 6409 1900 7c03 5f0a 7c03 a00b  _.|.d...|._.|...
-000014d0: a100 0100 7c03 5300 290a 4e29 0172 7700  ....|.S.).N).rw.
-000014e0: 0000 7a10 5765 6268 6f6f 6b20 7769 7468  ..z.Webhook with
-000014f0: 2069 6420 7a4c 2064 6f65 7320 6e6f 7420   id zL does not 
-00001500: 6578 6973 7420 696e 2074 6865 2064 6174  exist in the dat
-00001510: 6162 6173 652e 2053 6574 2075 7020 7765  abase. Set up we
-00001520: 6268 6f6f 6b73 2062 7920 6361 6c6c 696e  bhooks by callin
-00001530: 6720 2273 6574 7570 5f77 6562 686f 6f6b  g "setup_webhook
-00001540: 7322 7239 0000 007a 1b2f 7631 2f6e 6f74  s"r9...z./v1/not
-00001550: 6966 6963 6174 696f 6e73 2f77 6562 686f  ifications/webho
-00001560: 6f6b 732f 7261 0000 0072 7600 0000 723b  oks/ra...rv...r;
-00001570: 0000 0072 7500 0000 290c 7211 0000 0072  ...ru...).r....r
-00001580: 5000 0000 725c 0000 00da 0c44 6f65 734e  P...r\.....DoesN
-00001590: 6f74 4578 6973 74da 0877 6172 6e69 6e67  otExist..warning
-000015a0: 73da 0477 6172 6e72 4c00 0000 7226 0000  s..warnrL...r&..
-000015b0: 0072 4e00 0000 723b 0000 0072 7500 0000  .rN...r;...ru...
-000015c0: 725d 0000 0029 0772 2700 0000 7277 0000  r]...).r'...rw..
-000015d0: 0072 7e00 0000 5a0e 7061 7970 616c 5f77  .r~...Z.paypal_w
-000015e0: 6562 686f 6f6b 7270 0000 0072 3b00 0000  ebhookrp...r;...
-000015f0: 5a15 7765 6268 6f6f 6b5f 7265 7370 6f6e  Z.webhook_respon
-00001600: 7365 5f64 6963 7472 2b00 0000 722b 0000  se_dictr+...r+..
-00001610: 0072 2c00 0000 da0d 7061 7463 685f 7765  .r,.....patch_we
-00001620: 6268 6f6f 6b92 0000 0073 1600 0000 0001  bhook....s......
-00001630: 0201 1201 1201 1201 1601 1401 1001 0a01  ................
-00001640: 0a01 0801 7a1b 5061 7970 616c 5772 6170  ....z.PaypalWrap
-00001650: 7065 722e 7061 7463 685f 7765 6268 6f6f  per.patch_webhoo
-00001660: 6b29 03da 0772 6571 7565 7374 7277 0000  k)...requestrw..
-00001670: 0072 3200 0000 6303 0000 0000 0000 0000  .r2...c.........
-00001680: 0000 000d 0000 0008 0000 0043 0000 0073  ...........C...s
-00001690: 9a00 0000 7c01 6a00 7d03 7c03 a001 6401  ....|.j.}.|...d.
-000016a0: a101 7d04 7c03 a001 6402 a101 7d05 7c03  ..}.|...d...}.|.
-000016b0: a001 6403 a101 7d06 7c03 a001 6404 a101  ..d...}.|...d...
-000016c0: 7d07 7c03 a001 6405 a101 7d08 7402 a003  }.|...d...}.t...
-000016d0: 7c01 6a04 a005 6406 a101 a101 7d09 7c04  |.j...d.....}.|.
-000016e0: 7c05 7c06 7c07 7c08 7c02 7c09 6407 9c07  |.|.|.|.|.|.d...
-000016f0: 7d0a 7c00 6a06 9b00 6408 9d02 7d0b 7c00  }.|.j...d...}.|.
-00001700: 6a07 7c0b 6409 7c0a 640a 8d03 7d0c 7c0c  j.|.d.|.d...}.|.
-00001710: a001 640b a101 640c 6b02 728c 640d 5300  ..d...d.k.r.d.S.
-00001720: 7408 640e 7c0c 8302 8201 6400 5300 290f  t.d.|.....d.S.).
-00001730: 4e7a 1050 6179 7061 6c2d 4175 7468 2d41  Nz.Paypal-Auth-A
-00001740: 6c67 6f7a 0f50 6179 7061 6c2d 4365 7274  lgoz.Paypal-Cert
-00001750: 2d55 726c 7a16 5061 7970 616c 2d54 7261  -Urlz.Paypal-Tra
-00001760: 6e73 6d69 7373 696f 6e2d 4964 7a18 5061  nsmission-Idz.Pa
-00001770: 7970 616c 2d54 7261 6e73 6d69 7373 696f  ypal-Transmissio
-00001780: 6e2d 5469 6d65 7a17 5061 7970 616c 2d54  n-Timez.Paypal-T
-00001790: 7261 6e73 6d69 7373 696f 6e2d 5369 677a  ransmission-Sigz
-000017a0: 0575 7466 2d38 2907 da09 6175 7468 5f61  .utf-8)...auth_a
-000017b0: 6c67 6fda 0863 6572 745f 7572 6cda 0f74  lgo..cert_url..t
-000017c0: 7261 6e73 6d69 7373 696f 6e5f 6964 da11  ransmission_id..
-000017d0: 7472 616e 736d 6973 7369 6f6e 5f74 696d  transmission_tim
-000017e0: 65da 1074 7261 6e73 6d69 7373 696f 6e5f  e..transmission_
-000017f0: 7369 6772 7700 0000 5a0d 7765 6268 6f6f  sigrw...Z.webhoo
-00001800: 6b5f 6576 656e 747a 2a2f 7631 2f6e 6f74  k_eventz*/v1/not
-00001810: 6966 6963 6174 696f 6e73 2f76 6572 6966  ifications/verif
-00001820: 792d 7765 6268 6f6f 6b2d 7369 676e 6174  y-webhook-signat
-00001830: 7572 6572 3a00 0000 7276 0000 005a 1376  urer:...rv...Z.v
-00001840: 6572 6966 6963 6174 696f 6e5f 7374 6174  erification_stat
-00001850: 7573 da07 5355 4343 4553 5354 7a1b 5765  us..SUCCESSTz.We
-00001860: 6268 6f6f 6b20 7665 7269 6669 6361 7469  bhook verificati
-00001870: 6f6e 2066 6169 6c65 6429 0972 6500 0000  on failed).re...
-00001880: 725c 0000 0072 6600 0000 da05 6c6f 6164  r\...rf.....load
-00001890: 73da 0462 6f64 79da 0664 6563 6f64 6572  s..body..decoder
-000018a0: 2600 0000 724e 0000 0072 0d00 0000 290d  &...rN...r....).
-000018b0: 7227 0000 0072 8300 0000 7277 0000 0072  r'...r....rw...r
-000018c0: 6500 0000 7284 0000 0072 8500 0000 7286  e...r....r....r.
-000018d0: 0000 0072 8700 0000 7288 0000 00da 0c72  ...r....r......r
-000018e0: 6571 7565 7374 5f64 6174 615a 1476 6572  equest_dataZ.ver
-000018f0: 6966 6963 6174 696f 6e5f 7061 796c 6f61  ification_payloa
-00001900: 6472 3b00 0000 da03 7265 7372 2b00 0000  dr;.....resr+...
-00001910: 722b 0000 0072 2c00 0000 da14 7665 7269  r+...r,.....veri
-00001920: 6679 5f77 6562 686f 6f6b 5f65 7665 6e74  fy_webhook_event
-00001930: 9f00 0000 7328 0000 0000 0106 010a 010a  ....s(..........
-00001940: 010a 010a 010a 0112 0202 0102 0102 0102  ................
-00001950: 0102 0102 0102 f906 090c 0110 010e 0104  ................
-00001960: 017a 2250 6179 7061 6c57 7261 7070 6572  .z"PaypalWrapper
-00001970: 2e76 6572 6966 795f 7765 6268 6f6f 6b5f  .verify_webhook_
-00001980: 6576 656e 7429 0172 3200 0000 6301 0000  event).r2...c...
-00001990: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-000019a0: 0043 0000 0073 4c00 0000 7c00 6a00 7314  .C...sL...|.j.s.
-000019b0: 7c00 a001 a100 7d01 7c01 6a02 5300 7403  |.....}.|.j.S.t.
-000019c0: a004 7c00 6a05 a101 7d02 7c02 7344 7c00  ..|.j...}.|.sD|.
-000019d0: a001 a100 7d01 7c01 6a02 7d02 7403 a006  ....}.|.j.}.t...
-000019e0: 7c00 6a05 7c02 7c00 6a00 a103 0100 7c02  |.j.|.|.j.....|.
-000019f0: 5300 6400 5300 7220 0000 0029 07da 1261  S.d.S.r ...)...a
-00001a00: 7574 685f 6361 6368 655f 7469 6d65 6f75  uth_cache_timeou
-00001a10: 74da 115f 6175 7468 6f72 697a 655f 636c  t.._authorize_cl
-00001a20: 6965 6e74 da0c 6163 6365 7373 5f74 6f6b  ient..access_tok
-00001a30: 656e 7207 0000 0072 5c00 0000 da0e 6175  enr....r\.....au
-00001a40: 7468 5f63 6163 6865 5f6b 6579 da03 7365  th_cache_key..se
-00001a50: 7429 0372 2700 0000 da0d 6175 7468 5f72  t).r'.....auth_r
-00001a60: 6573 706f 6e73 6572 9200 0000 722b 0000  esponser....r+..
-00001a70: 0072 2b00 0000 722c 0000 0072 6800 0000  .r+...r,...rh...
-00001a80: b600 0000 7312 0000 0000 0106 0108 0106  ....s...........
-00001a90: 020c 0104 0108 0106 0112 017a 1f50 6179  ...........z.Pay
-00001aa0: 7061 6c57 7261 7070 6572 2e5f 6765 745f  palWrapper._get_
-00001ab0: 6163 6365 7373 5f74 6f6b 656e 6301 0000  access_tokenc...
-00001ac0: 0000 0000 0000 0000 0008 0000 000a 0000  ................
-00001ad0: 0043 0000 0073 ca00 0000 7c00 6a00 9b00  .C...s....|.j...
-00001ae0: 7c00 6a01 9b00 9d02 7d01 7402 7c00 6a03  |.j.....}.t.|.j.
-00001af0: 6a04 7c00 6a03 6a05 8302 7d02 6401 6402  j.|.j.j...}.d.d.
-00001b00: 6403 9c02 7d03 6404 6405 6901 7d04 7a2e  d...}.d.d.i.}.z.
-00001b10: 7406 6a07 7c01 7c03 7c04 7c02 6406 8d04  t.j.|.|.|.|.d...
-00001b20: 7d05 7c05 a008 a100 0100 7c05 a009 a100  }.|.......|.....
-00001b30: 7d06 740a 6600 7c06 8e01 5700 5300 0400  }.t.f.|...W.S...
-00001b40: 7406 6a0b 6b0a 72c4 0100 7d07 0100 7a42  t.j.k.r...}...zB
-00001b50: 740c 7c07 6a0d a009 a100 7c01 8302 0100  t.|.j.....|.....
-00001b60: 740c 6407 7c00 6a03 6a04 8302 0100 740c  t.d.|.j.j.....t.
-00001b70: 6408 7c00 6a03 6a05 8302 0100 740e 740f  d.|.j.j.....t.t.
-00001b80: 7c07 8301 7c07 6a0d 6409 8d02 8201 5700  |...|.j.d.....W.
-00001b90: 3500 6400 7d07 7e07 5800 5900 6e02 5800  5.d.}.~.X.Y.n.X.
-00001ba0: 6400 5300 290a 4e72 6200 0000 7a21 6170  d.S.).Nrb...z!ap
-00001bb0: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
-00001bc0: 666f 726d 2d75 726c 656e 636f 6465 6429  form-urlencoded)
-00001bd0: 02da 0641 6363 6570 7472 6400 0000 5a0a  ...Acceptrd...Z.
-00001be0: 6772 616e 745f 7479 7065 5a12 636c 6965  grant_typeZ.clie
-00001bf0: 6e74 5f63 7265 6465 6e74 6961 6c73 2903  nt_credentials).
-00001c00: 7265 0000 0072 3c00 0000 721f 0000 007a  re...r<...r....z
-00001c10: 0943 6c69 656e 7420 6964 7a0d 436c 6965  .Client idz.Clie
-00001c20: 6e74 2073 6563 7265 7472 6700 0000 2910  nt secretrg...).
-00001c30: 7226 0000 00da 0861 7574 685f 7572 6c72  r&.....auth_urlr
-00001c40: 0900 0000 721f 0000 00da 0963 6c69 656e  ....r......clien
-00001c50: 745f 6964 da0d 636c 6965 6e74 5f73 6563  t_id..client_sec
-00001c60: 7265 7472 6900 0000 7245 0000 0072 6c00  retri...rE...rl.
-00001c70: 0000 7266 0000 0072 1200 0000 726d 0000  ..rf...r....rm..
-00001c80: 00da 0570 7269 6e74 7248 0000 0072 0b00  ...printrH...r..
-00001c90: 0000 726e 0000 0029 0872 2700 0000 723b  ..rn...).r'...r;
-00001ca0: 0000 005a 0861 7069 5f61 7574 6872 6500  ...Z.api_authre.
-00001cb0: 0000 723c 0000 0072 4800 0000 726f 0000  ..r<...rH...ro..
-00001cc0: 0072 7000 0000 722b 0000 0072 2b00 0000  .rp...r+...r+...
-00001cd0: 722c 0000 0072 9100 0000 c200 0000 731c  r,...r........s.
-00001ce0: 0000 0000 0210 0212 010a 0108 0202 0112  ................
-00001cf0: 0108 0108 010c 0112 0110 010e 010e 017a  ...............z
-00001d00: 1f50 6179 7061 6c57 7261 7070 6572 2e5f  .PaypalWrapper._
-00001d10: 6175 7468 6f72 697a 655f 636c 6965 6e74  authorize_client
-00001d20: 2901 4e29 014e 2932 da08 5f5f 6e61 6d65  ).N).N)2..__name
-00001d30: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001d40: 5f5f 7175 616c 6e61 6d65 5f5f 724c 0000  __qualname__rL..
-00001d50: 0072 2300 0000 5a15 444a 414e 474f 5f50  .r#...Z.DJANGO_P
-00001d60: 4159 5041 4c5f 5645 5253 494f 4eda 1169  AYPAL_VERSION..i
-00001d70: 6e74 6572 6661 6365 5f76 6572 7369 6f6e  nterface_version
-00001d80: 5a0e 5041 5950 414c 5f41 5049 5f55 524c  Z.PAYPAL_API_URL
-00001d90: 7226 0000 005a 1650 4159 5041 4c5f 5341  r&...Z.PAYPAL_SA
-00001da0: 4e44 424f 585f 4150 495f 5552 4c72 2500  NDBOX_API_URLr%.
-00001db0: 0000 5a1a 5041 5950 414c 5f4f 5244 4552  ..Z.PAYPAL_ORDER
-00001dc0: 535f 4150 495f 454e 4450 4f49 4e54 724d  S_API_ENDPOINTrM
-00001dd0: 0000 005a 0f50 4159 5041 4c5f 4155 5448  ...Z.PAYPAL_AUTH
-00001de0: 5f55 524c 7297 0000 005a 1950 4159 5041  _URLr....Z.PAYPA
-00001df0: 4c5f 4155 5448 5f43 4143 4845 5f54 494d  L_AUTH_CACHE_TIM
-00001e00: 454f 5554 7290 0000 005a 1550 4159 5041  EOUTr....Z.PAYPA
-00001e10: 4c5f 4155 5448 5f43 4143 4845 5f4b 4559  L_AUTH_CACHE_KEY
-00001e20: 7293 0000 0072 1f00 0000 7217 0000 00da  r....r....r.....
-00001e30: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00001e40: 7222 0000 005a 1250 4159 5041 4c5f 5355  r"...Z.PAYPAL_SU
-00001e50: 4343 4553 535f 5552 4c5a 1750 4159 5041  CCESS_URLZ.PAYPA
-00001e60: 4c5f 4341 4e43 454c 4c41 5449 4f4e 5f55  L_CANCELLATION_U
-00001e70: 524c 7203 0000 0072 0400 0000 7216 0000  RLr....r....r...
-00001e80: 0072 1300 0000 7214 0000 0072 1800 0000  .r....r....r....
-00001e90: 7257 0000 0072 6e00 0000 7219 0000 0072  rW...rn...r....r
-00001ea0: 5e00 0000 721a 0000 0072 6000 0000 7206  ^...r....r`...r.
-00001eb0: 0000 0072 0500 0000 724e 0000 0072 1100  ...r....rN...r..
-00001ec0: 0000 727d 0000 0072 8200 0000 7208 0000  ..r}...r....r...
-00001ed0: 00da 0462 6f6f 6c72 8f00 0000 7268 0000  ...boolr....rh..
-00001ee0: 0072 1200 0000 7291 0000 00da 0d5f 5f63  .r....r......__c
-00001ef0: 6c61 7373 6365 6c6c 5f5f 722b 0000 0072  lasscell__r+...r
-00001f00: 2b00 0000 7229 0000 0072 2c00 0000 721e  +...r)...r,...r.
-00001f10: 0000 0023 0000 0073 3600 0000 0a01 0c02  ...#...s6.......
-00001f20: 0601 0601 0601 0601 0601 0602 0c02 140b  ................
-00001f30: 0201 0401 04f9 0202 0601 0601 0201 0203  ................
-00001f40: 02f8 0c24 100c 1006 2012 1015 160d 1217  ...$.... .......
-00001f50: 0e0c 721e 0000 0029 2dda 0a5f 5f66 7574  ..r....)-..__fut
-00001f60: 7572 655f 5f72 0200 0000 7266 0000 0072  ure__r....rf...r
-00001f70: 8000 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-00001f80: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-00001f90: da11 646a 616e 676f 2e63 6f72 652e 6361  ..django.core.ca
-00001fa0: 6368 6572 0700 0000 7269 0000 00da 0b64  cher....ri.....d
-00001fb0: 6a61 6e67 6f2e 6874 7470 7208 0000 005a  jango.httpr....Z
-00001fc0: 0d72 6571 7565 7374 732e 6175 7468 7209  .requests.authr.
-00001fd0: 0000 00da 0d64 6a61 6e67 6f5f 7061 7970  .....django_payp
-00001fe0: 616c 720a 0000 0072 2300 0000 5a18 646a  alr....r#...Z.dj
-00001ff0: 616e 676f 5f70 6179 7061 6c2e 6578 6365  ango_paypal.exce
-00002000: 7074 696f 6e73 720b 0000 0072 0c00 0000  ptionsr....r....
-00002010: 720d 0000 00da 1464 6a61 6e67 6f5f 7061  r......django_pa
-00002020: 7970 616c 2e6d 6f64 656c 7372 0e00 0000  ypal.modelsr....
-00002030: 720f 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00002040: 1764 6a61 6e67 6f5f 7061 7970 616c 2e61  .django_paypal.a
-00002050: 7069 5f74 7970 6573 7212 0000 0072 1300  pi_typesr....r..
-00002060: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00002070: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00002080: 721a 0000 005a 1364 6a61 6e67 6f5f 7061  r....Z.django_pa
-00002090: 7970 616c 2e75 7469 6c73 721b 0000 005a  ypal.utilsr....Z
-000020a0: 1564 6a61 6e67 6f5f 7061 7970 616c 2e73  .django_paypal.s
-000020b0: 6967 6e61 6c73 721c 0000 0072 1d00 0000  ignalsr....r....
-000020c0: da06 6f62 6a65 6374 721e 0000 0072 2b00  ..objectr....r+.
-000020d0: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
-000020e0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000020f0: 1c00 0000 0c02 0801 0801 1802 0c01 0801  ................
-00002100: 0c01 0c02 0c01 1401 1806 2c0b 0c01 1003  ..........,.....
+00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 5a04 6400 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
+00000060: 6d08 5a08 6d09 5a09 0100 6400 6404 6c0a  m.Z.m.Z...d.d.l.
+00000070: 6d0b 5a0b 0100 6400 6402 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
+00000080: 6405 6c0d 6d0e 5a0e 0100 6400 6406 6c0f  d.l.m.Z...d.d.l.
+00000090: 6d10 5a10 0100 6400 6407 6c11 6d12 5a13  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 6408 6c14 6d15 5a15 6d16 5a16  ..d.d.l.m.Z.m.Z.
+000000b0: 6d17 5a17 0100 6400 6409 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
+000000c0: 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c 0100 6400  m.Z.m.Z.m.Z...d.
+000000d0: 640a 6c1d 6d1e 5a1e 6d1f 5a1f 6d20 5a20  d.l.m.Z.m.Z.m Z 
+000000e0: 6d21 5a21 6d22 5a22 6d23 5a23 6d24 5a24  m!Z!m"Z"m#Z#m$Z$
+000000f0: 6d25 5a25 6d26 5a26 0100 6400 640b 6c27  m%Z%m&Z&..d.d.l'
+00000100: 6d28 5a28 0100 6400 640c 6c29 6d2a 5a2a  m(Z(..d.d.l)m*Z*
+00000110: 6d2b 5a2b 0100 4700 640d 640e 8400 640e  m+Z+..G.d.d...d.
+00000120: 652c 8303 5a2d 6402 5300 290f e900 0000  e,..Z-d.S.).....
+00000130: 0029 01da 1075 6e69 636f 6465 5f6c 6974  .)...unicode_lit
+00000140: 6572 616c 734e 2904 da07 4c69 7465 7261  eralsN)...Litera
+00000150: 6cda 044c 6973 74da 0341 6e79 da04 4469  l..List..Any..Di
+00000160: 6374 2901 da05 6361 6368 6529 01da 0b48  ct)...cache)...H
+00000170: 7474 7052 6571 7565 7374 2901 da0d 4854  ttpRequest)...HT
+00000180: 5450 4261 7369 6341 7574 6829 01da 0873  TPBasicAuth)...s
+00000190: 6574 7469 6e67 7329 03da 1150 6179 7061  ettings)...Paypa
+000001a0: 6c41 7574 6846 6169 6c75 7265 da0e 5061  lAuthFailure..Pa
+000001b0: 7970 616c 4150 4945 7272 6f72 da1e 5061  ypalAPIError..Pa
+000001c0: 7970 616c 5765 6268 6f6f 6b56 6572 6966  ypalWebhookVerif
+000001d0: 6963 6174 696f 6e45 7272 6f72 2904 da0b  icationError)...
+000001e0: 5061 7970 616c 4f72 6465 72da 1150 6179  PaypalOrder..Pay
+000001f0: 7061 6c41 5049 506f 7374 4461 7461 da11  palAPIPostData..
+00000200: 5061 7970 616c 4150 4952 6573 706f 6e73  PaypalAPIRespons
+00000210: 65da 0d50 6179 7061 6c57 6562 686f 6f6b  e..PaypalWebhook
+00000220: 2909 da0d 4f41 7574 6852 6573 706f 6e73  )...OAuthRespons
+00000230: 65da 0d50 6179 6d65 6e74 536f 7572 6365  e..PaymentSource
+00000240: da12 4170 706c 6963 6174 696f 6e43 6f6e  ..ApplicationCon
+00000250: 7465 7874 da11 4578 7065 7269 656e 6365  text..Experience
+00000260: 436f 6e74 6578 74da 0c50 7572 6368 6173  Context..Purchas
+00000270: 6555 6e69 74da 1241 5049 4175 7468 4372  eUnit..APIAuthCr
+00000280: 6564 656e 7469 616c 73da 174f 7264 6572  edentials..Order
+00000290: 4372 6561 7465 6441 5049 5265 7370 6f6e  CreatedAPIRespon
+000002a0: 7365 da17 4f72 6465 7243 6170 7475 7265  se..OrderCapture
+000002b0: 4150 4952 6573 706f 6e73 65da 164f 7264  APIResponse..Ord
+000002c0: 6572 4465 7461 696c 4150 4952 6573 706f  erDetailAPIRespo
+000002d0: 6e73 6529 01da 1562 7569 6c64 5f70 6179  nse)...build_pay
+000002e0: 7061 6c5f 6675 6c6c 5f75 7269 2902 da0e  pal_full_uri)...
+000002f0: 6f72 6465 725f 6361 7074 7572 6564 da0d  order_captured..
+00000300: 6f72 6465 725f 6372 6561 7465 6463 0000  order_createdc..
+00000310: 0000 0000 0000 0000 0000 0000 0000 0700  ................
+00000320: 0000 0000 0000 7350 0100 0065 005a 0164  ......sP...e.Z.d
+00000330: 005a 0255 0064 01a0 0365 046a 05a1 015a  .Z.U.d...e.j...Z
+00000340: 0665 046a 075a 0865 046a 095a 0a65 046a  .e.j.Z.e.j.Z.e.j
+00000350: 0b5a 0c65 046a 0d5a 0e65 046a 0f5a 1065  .Z.e.j.Z.e.j.Z.e
+00000360: 046a 115a 1264 025a 1365 1465 1564 033c  .j.Z.d.Z.e.e.d.<
+00000370: 0064 2865 1464 049c 0187 0066 0164 0564  .d(e.d.....f.d.d
+00000380: 0684 0d5a 1664 0265 046a 1765 046a 1866  ...Z.d.e.j.e.j.f
+00000390: 0365 1964 0719 0065 1a65 1b19 0065 1c65  .e.d...e.e...e.e
+000003a0: 1d65 1e64 089c 0564 0964 0a84 055a 1f65  .e.d...d.d...Z.e
+000003b0: 2065 2164 0b9c 0264 0c64 0d84 045a 2265   e!d...d.d...Z"e
+000003c0: 2065 2364 0b9c 0264 0e64 0f84 045a 2464   e#d...d.d...Z$d
+000003d0: 2965 2065 1964 1019 0065 2565 2065 2666  )e e.d...e%e e&f
+000003e0: 0219 0064 119c 0364 1264 1384 055a 2765  ...d...d.d...Z'e
+000003f0: 2065 2864 149c 0264 1564 1684 045a 2965   e(d...d.d...Z)e
+00000400: 2065 1a65 2519 0065 2864 179c 0364 1864   e.e%..e(d...d.d
+00000410: 1984 045a 2a65 2065 2b64 149c 0264 1a64  ...Z*e e+d...d.d
+00000420: 1b84 045a 2c65 2d65 2065 2b64 1c9c 0364  ...Z,e-e e+d...d
+00000430: 1d64 1e84 045a 2e65 2b64 1f9c 0164 2064  .d...Z.e+d...d d
+00000440: 2184 045a 2f65 2064 1f9c 0164 2264 2384  !..Z/e d...d"d#.
+00000450: 045a 3065 3164 1f9c 0164 2464 2584 045a  .Z0e1d...d$d%..Z
+00000460: 3265 3365 2064 1f9c 0164 2664 2784 0483  2e3e d...d&d'...
+00000470: 015a 3487 0004 005a 3553 0029 2ada 0d50  .Z4....Z5S.)*..P
+00000480: 6179 7061 6c57 7261 7070 6572 7a11 646a  aypalWrapperz.dj
+00000490: 616e 676f 5f70 6179 7061 6c5f 767b 7d4e  ango_paypal_v{}N
+000004a0: da04 6175 7468 2901 721f 0000 0063 0300  ..auth).r....c..
+000004b0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000004c0: 0000 0300 0000 732a 0000 0074 0074 017c  ......s*...t.t.|
+000004d0: 0083 02a0 02a1 0001 007c 017c 005f 037c  .........|.|._.|
+000004e0: 0273 1e74 046a 0572 267c 006a 067c 005f  .s.t.j.r&|.j.|._
+000004f0: 0764 0053 00a9 014e 2908 da05 7375 7065  .d.S...N)...supe
+00000500: 7272 1e00 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
+00000510: 721f 0000 00da 1664 6a61 6e67 6f5f 7061  r......django_pa
+00000520: 7970 616c 5f73 6574 7469 6e67 73da 0e50  ypal_settings..P
+00000530: 4159 5041 4c5f 5341 4e44 424f 58da 0b73  AYPAL_SANDBOX..s
+00000540: 616e 6462 6f78 5f75 726c da07 6170 695f  andbox_url..api_
+00000550: 7572 6c29 03da 0473 656c 6672 1f00 0000  url)...selfr....
+00000560: da07 7361 6e64 626f 78a9 01da 095f 5f63  ..sandbox....__c
+00000570: 6c61 7373 5f5f a900 fa5d 2f55 7365 7273  lass__...]/Users
+00000580: 2f74 696d 7461 6d2f 2e70 7965 6e76 2f76  /timtam/.pyenv/v
+00000590: 6572 7369 6f6e 732f 7366 2d33 2e38 2e31  ersions/sf-3.8.1
+000005a0: 322f 6c69 622f 7079 7468 6f6e 332e 382f  2/lib/python3.8/
+000005b0: 7369 7465 2d70 6163 6b61 6765 732f 646a  site-packages/dj
+000005c0: 616e 676f 5f70 6179 7061 6c2f 7772 6170  ango_paypal/wrap
+000005d0: 7065 7273 2e70 7972 2200 0000 3000 0000  pers.pyr"...0...
+000005e0: 7308 0000 0000 010e 0106 010a 017a 1650  s............z.P
+000005f0: 6179 7061 6c57 7261 7070 6572 2e5f 5f69  aypalWrapper.__i
+00000600: 6e69 745f 5f29 02da 0743 4150 5455 5245  nit__)...CAPTURE
+00000610: 5a09 4155 5448 4f52 495a 4529 05da 0669  Z.AUTHORIZE)...i
+00000620: 6e74 656e 74da 0e70 7572 6368 6173 655f  ntent..purchase_
+00000630: 756e 6974 73da 0e70 6179 6d65 6e74 5f73  units..payment_s
+00000640: 6f75 7263 65da 1361 7070 6c69 6361 7469  ource..applicati
+00000650: 6f6e 5f63 6f6e 7465 7874 da06 7265 7475  on_context..retu
+00000660: 726e 6307 0000 0000 0000 0000 0000 000d  rnc.............
+00000670: 0000 0006 0000 0043 0000 0073 1a01 0000  .......C...s....
+00000680: 7c03 6a00 7260 7c05 730e 7c06 7260 7c03  |.j.r`|.s.|.r`|.
+00000690: 6a00 6a01 7330 7402 7403 7c05 8301 7403  j.j.s0t.t.|...t.
+000006a0: 7c06 8301 6401 8d02 7c03 6a00 5f01 6e30  |...d...|.j._.n0
+000006b0: 7c03 6a00 6a01 6a04 7348 7403 7c05 8301  |.j.j.j.sHt.|...
+000006c0: 7c03 6a00 6a01 5f04 7c03 6a00 6a01 6a05  |.j.j._.|.j.j.j.
+000006d0: 7360 7403 7c06 8301 7c03 6a00 6a01 5f05  s`t.|...|.j.j._.
+000006e0: 7c01 6402 6403 8400 7c02 4400 8301 6404  |.d.d...|.D...d.
+000006f0: 9c02 7d07 7c03 728a 7c07 a006 6405 7c03  ..}.|.r.|...d.|.
+00000700: a007 a100 6901 a101 0100 7c04 72a0 7c07  ....i.....|.r.|.
+00000710: a006 6406 7c04 a007 a100 6901 a101 0100  ..d.|.....i.....
+00000720: 6407 a008 7c00 6a09 7c00 6a0a a102 7d08  d...|.j.|.j...}.
+00000730: 7c00 6a0b 7c08 7c07 6408 6409 8d03 7d09  |.j.|.|.d.d...}.
+00000740: 740c a00d 7c09 a101 7d0a 740e 6a0f 6a10  t...|...}.t.j.j.
+00000750: 7c0a 6a11 7c0a 6a12 640a 8d02 7d0b 7413  |.j.|.j.d...}.t.
+00000760: 6a0f 6a10 7c0b 7c08 7c07 640b 8d03 7d0c  j.j.|.|.|.d...}.
+00000770: 7414 6a0f 6a10 7c0b 7c08 7c09 7c0c 640c  t.j.j.|.|.|.|.d.
+00000780: 8d04 0100 7415 6a16 7c00 6a17 7c0b 7c09  ....t.j.|.j.|.|.
+00000790: 640d 8d03 0100 7c0a 5300 290e 4e29 02da  d.....|.S.).N)..
+000007a0: 0a72 6574 7572 6e5f 7572 6cda 0a63 616e  .return_url..can
+000007b0: 6365 6c5f 7572 6c63 0100 0000 0000 0000  cel_urlc........
+000007c0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+000007d0: 7314 0000 0067 007c 005d 0c7d 017c 01a0  s....g.|.].}.|..
+000007e0: 00a1 0091 0271 0453 0072 2b00 0000 2901  .....q.S.r+...).
+000007f0: da07 746f 5f64 6963 7429 02da 022e 30da  ..to_dict)....0.
+00000800: 0d70 7572 6368 6173 655f 756e 6974 722b  .purchase_unitr+
+00000810: 0000 0072 2b00 0000 722c 0000 00da 0a3c  ...r+...r,.....<
+00000820: 6c69 7374 636f 6d70 3e4b 0000 0073 0400  listcomp>K...s..
+00000830: 0000 0600 0200 7a2e 5061 7970 616c 5772  ......z.PaypalWr
+00000840: 6170 7065 722e 6372 6561 7465 5f6f 7264  apper.create_ord
+00000850: 6572 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  er.<locals>.<lis
+00000860: 7463 6f6d 703e 2902 722e 0000 0072 2f00  tcomp>).r....r/.
+00000870: 0000 7230 0000 0072 3100 0000 fa06 7b30  ..r0...r1.....{0
+00000880: 7d7b 317d da04 504f 5354 2903 da03 7572  }{1}..POST)...ur
+00000890: 6cda 0464 6174 61da 066d 6574 686f 6429  l..data..method)
+000008a0: 02da 086f 7264 6572 5f69 64da 0673 7461  ...order_id..sta
+000008b0: 7475 73a9 03da 056f 7264 6572 723b 0000  tus....orderr;..
+000008c0: 00da 0970 6f73 745f 6461 7461 a904 7241  ...post_data..rA
+000008d0: 0000 0072 3b00 0000 da0d 7265 7370 6f6e  ...r;.....respon
+000008e0: 7365 5f64 6174 61da 0470 6f73 74a9 03da  se_data..post...
+000008f0: 0673 656e 6465 7272 4100 0000 da08 7265  .senderrA.....re
+00000900: 7370 6f6e 7365 2918 da06 7061 7970 616c  sponse)...paypal
+00000910: da12 6578 7065 7269 656e 6365 5f63 6f6e  ..experience_con
+00000920: 7465 7874 7215 0000 0072 1b00 0000 7233  textr....r....r3
+00000930: 0000 0072 3400 0000 da06 7570 6461 7465  ...r4.....update
+00000940: 7235 0000 00da 0666 6f72 6d61 7472 2600  r5.....formatr&.
+00000950: 0000 da13 6f72 6465 7273 5f61 7069 5f65  ....orders_api_e
+00000960: 6e64 706f 696e 74da 0863 616c 6c5f 6170  ndpoint..call_ap
+00000970: 6972 1800 0000 da09 6672 6f6d 5f64 6963  ir......from_dic
+00000980: 7472 0e00 0000 da07 6f62 6a65 6374 73da  tr......objects.
+00000990: 0663 7265 6174 65da 0269 6472 3f00 0000  .create..idr?...
+000009a0: 720f 0000 0072 1000 0000 721d 0000 00da  r....r....r.....
+000009b0: 0473 656e 6472 2a00 0000 290d 7227 0000  .sendr*...).r'..
+000009c0: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+000009d0: 7231 0000 00da 0b73 7563 6365 7373 5f75  r1.....success_u
+000009e0: 726c da10 6361 6e63 656c 6c61 7469 6f6e  rl..cancellation
+000009f0: 5f75 726c 5a0a 6f72 6465 725f 6461 7461  _urlZ.order_data
+00000a00: 723b 0000 005a 136f 7264 6572 5f72 6573  r;...Z.order_res
+00000a10: 706f 6e73 655f 6469 6374 5a0e 6f72 6465  ponse_dictZ.orde
+00000a20: 725f 7265 7370 6f6e 7365 5a09 6e65 775f  r_responseZ.new_
+00000a30: 6f72 6465 72da 0870 6f73 745f 6f62 6a72  order..post_objr
+00000a40: 2b00 0000 722b 0000 0072 2c00 0000 da0c  +...r+...r,.....
+00000a50: 6372 6561 7465 5f6f 7264 6572 3600 0000  create_order6...
+00000a60: 732e 0000 0000 090e 0108 0102 0106 0106  s...............
+00000a70: fe0c 050a 010e 010a 010e 0214 0104 0112  ................
+00000a80: 0104 0112 0210 0110 010a 0114 0112 0114  ................
+00000a90: 0112 017a 1a50 6179 7061 6c57 7261 7070  ...z.PaypalWrapp
+00000aa0: 6572 2e63 7265 6174 655f 6f72 6465 7229  er.create_order)
+00000ab0: 0272 3e00 0000 7232 0000 0063 0200 0000  .r>...r2...c....
+00000ac0: 0000 0000 0000 0000 0700 0000 0600 0000  ................
+00000ad0: 4300 0000 7392 0000 0074 006a 016a 027c  C...s....t.j.j.|
+00000ae0: 0164 018d 017d 027c 006a 039b 007c 006a  .d...}.|.j...|.j
+00000af0: 049b 0064 027c 026a 059b 0064 039d 057d  ...d.|.j...d...}
+00000b00: 037c 006a 067c 0364 0464 058d 027d 0474  .|.j.|.d.d...}.t
+00000b10: 07a0 087c 04a1 017d 057c 056a 097c 025f  ...|...}.|.j.|._
+00000b20: 097c 026a 0a64 0667 0164 078d 0101 0074  .|.j.d.g.d.....t
+00000b30: 0b6a 016a 0c7c 027c 0369 0064 088d 037d  .j.j.|.|.i.d...}
+00000b40: 0674 0d6a 016a 0c7c 027c 037c 047c 0664  .t.j.j.|.|.|.|.d
+00000b50: 098d 0401 0074 0e6a 0f7c 006a 107c 027c  .....t.j.|.j.|.|
+00000b60: 0464 0a8d 0301 007c 0553 0029 0b4e a901  .d.....|.S.).N..
+00000b70: 723e 0000 00fa 012f 7a08 2f63 6170 7475  r>...../z./captu
+00000b80: 7265 723a 0000 00a9 0272 3b00 0000 723d  rer:.....r;...r=
+00000b90: 0000 0072 3f00 0000 2901 da0d 7570 6461  ...r?...)...upda
+00000ba0: 7465 5f66 6965 6c64 7372 4000 0000 7243  te_fieldsr@...rC
+00000bb0: 0000 0072 4600 0000 2911 720e 0000 0072  ...rF...).r....r
+00000bc0: 5000 0000 da03 6765 7472 2600 0000 724d  P.....getr&...rM
+00000bd0: 0000 0072 3e00 0000 724e 0000 0072 1900  ...r>...rN...r..
+00000be0: 0000 724f 0000 0072 3f00 0000 da04 7361  ..rO...r?.....sa
+00000bf0: 7665 720f 0000 0072 5100 0000 7210 0000  ver....rQ...r...
+00000c00: 0072 1c00 0000 7253 0000 0072 2a00 0000  .r....rS...r*...
+00000c10: 2907 7227 0000 0072 3e00 0000 7241 0000  ).r'...r>...rA..
+00000c20: 0072 3b00 0000 5a16 6f72 6465 725f 6361  .r;...Z.order_ca
+00000c30: 7074 7572 655f 7265 7370 6f6e 7365 5a0d  pture_responseZ.
+00000c40: 6f72 6465 725f 6361 7074 7572 6572 5600  order_capturerV.
+00000c50: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+00000c60: 00da 0d63 6170 7475 7265 5f6f 7264 6572  ...capture_order
+00000c70: 5a00 0000 7314 0000 0000 010e 011a 010e  Z...s...........
+00000c80: 010a 0108 010e 0112 0114 0112 017a 1b50  .............z.P
+00000c90: 6179 7061 6c57 7261 7070 6572 2e63 6170  aypalWrapper.cap
+00000ca0: 7475 7265 5f6f 7264 6572 6302 0000 0000  ture_orderc.....
+00000cb0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+00000cc0: 0000 0073 3e00 0000 7400 6a01 6a02 7c01  ...s>...t.j.j.|.
+00000cd0: 6401 8d01 7d02 7c00 6a03 9b00 7c00 6a04  d...}.|.j...|.j.
+00000ce0: 9b00 6402 7c02 6a05 9b00 9d04 7d03 7c00  ..d.|.j.....}.|.
+00000cf0: 6a06 7c03 6403 6404 8d02 7d04 7407 a008  j.|.d.d...}.t...
+00000d00: 7c04 a101 5300 2905 4e72 5800 0000 7259  |...S.).NrX...rY
+00000d10: 0000 00da 0347 4554 725a 0000 0029 0972  .....GETrZ...).r
+00000d20: 0e00 0000 7250 0000 0072 5c00 0000 7226  ....rP...r\...r&
+00000d30: 0000 0072 4d00 0000 723e 0000 0072 4e00  ...rM...r>...rN.
+00000d40: 0000 721a 0000 0072 4f00 0000 2905 7227  ..r....rO...).r'
+00000d50: 0000 0072 3e00 0000 7241 0000 0072 3b00  ...r>...rA...r;.
+00000d60: 0000 5a16 6f72 6465 725f 6465 7461 696c  ..Z.order_detail
+00000d70: 735f 7265 7370 6f6e 7365 722b 0000 0072  s_responser+...r
+00000d80: 2b00 0000 722c 0000 00da 1167 6574 5f6f  +...r,.....get_o
+00000d90: 7264 6572 5f64 6574 6169 6c73 6600 0000  rder_detailsf...
+00000da0: 7308 0000 0000 010e 0118 010e 017a 1f50  s............z.P
+00000db0: 6179 7061 6c57 7261 7070 6572 2e67 6574  aypalWrapper.get
+00000dc0: 5f6f 7264 6572 5f64 6574 6169 6c73 2904  _order_details).
+00000dd0: 725f 0000 0072 3a00 0000 da05 5041 5443  r_...r:.....PATC
+00000de0: 48da 0644 454c 4554 4529 0372 3b00 0000  H..DELETE).r;...
+00000df0: 723d 0000 0072 3200 0000 6304 0000 0000  r=...r2...c.....
+00000e00: 0000 0000 0000 0008 0000 000a 0000 0043  ...............C
+00000e10: 0000 0073 e200 0000 6401 7c00 a000 a100  ...s....d.|.....
+00000e20: 9b00 9d02 6402 6403 9c02 7d04 7a92 7c02  ....d.d...}.z.|.
+00000e30: 6404 6b02 722e 7401 6a02 7c01 7c04 6405  d.k.r.t.j.|.|.d.
+00000e40: 8d02 7d05 6e64 7c02 6406 6b02 7248 7401  ..}.nd|.d.k.rHt.
+00000e50: 6a03 7c01 7c04 7c03 6407 8d03 7d05 6e4a  j.|.|.|.d...}.nJ
+00000e60: 7c02 6408 6b02 7262 7401 6a04 7c01 7c04  |.d.k.rbt.j.|.|.
+00000e70: 7c03 6407 8d03 7d05 6e30 7c02 6409 6b02  |.d...}.n0|.d.k.
+00000e80: 728a 7401 6a05 7c01 7c04 6405 8d02 7d05  r.t.j.|.|.d...}.
+00000e90: 7c05 a006 a100 0100 640a 640b 6901 5700  |.......d.d.i.W.
+00000ea0: 5300 7407 640c 8301 8201 7c05 a006 a100  S.t.d.....|.....
+00000eb0: 0100 7c05 a008 a100 7d06 7c06 5700 5300  ..|.....}.|.W.S.
+00000ec0: 0400 7401 6a09 6b0a 72dc 0100 7d07 0100  ..t.j.k.r...}...
+00000ed0: 7a16 740a 740b 7c07 8301 7c07 6a0c 640d  z.t.t.|...|.j.d.
+00000ee0: 8d02 8201 5700 3500 6400 7d07 7e07 5800  ....W.5.d.}.~.X.
+00000ef0: 5900 6e02 5800 6400 5300 290e 4e7a 0742  Y.n.X.d.S.).Nz.B
+00000f00: 6561 7265 7220 fa10 6170 706c 6963 6174  earer ..applicat
+00000f10: 696f 6e2f 6a73 6f6e 2902 da0d 4175 7468  ion/json)...Auth
+00000f20: 6f72 697a 6174 696f 6efa 0c43 6f6e 7465  orization..Conte
+00000f30: 6e74 2d54 7970 6572 5f00 0000 2901 da07  nt-Typer_...)...
+00000f40: 6865 6164 6572 7372 3a00 0000 2902 7266  headersr:...).rf
+00000f50: 0000 00da 046a 736f 6e72 6100 0000 7262  .....jsonra...rb
+00000f60: 0000 00da 0764 656c 6574 6564 547a 0e49  .....deletedTz.I
+00000f70: 6e76 616c 6964 206d 6574 686f 64a9 0172  nvalid method..r
+00000f80: 4800 0000 290d da11 5f67 6574 5f61 6363  H...)..._get_acc
+00000f90: 6573 735f 746f 6b65 6eda 0872 6571 7565  ess_token..reque
+00000fa0: 7374 7372 5c00 0000 7245 0000 00da 0570  stsr\...rE.....p
+00000fb0: 6174 6368 da06 6465 6c65 7465 da10 7261  atch..delete..ra
+00000fc0: 6973 655f 666f 725f 7374 6174 7573 da0a  ise_for_status..
+00000fd0: 5661 6c75 6545 7272 6f72 7267 0000 00da  ValueErrorrg....
+00000fe0: 0948 5454 5045 7272 6f72 720c 0000 00da  .HTTPErrorr.....
+00000ff0: 0373 7472 7248 0000 0029 0872 2700 0000  .strrH...).r'...
+00001000: 723b 0000 0072 3d00 0000 723c 0000 0072  r;...r=...r<...r
+00001010: 6600 0000 7248 0000 00da 0d72 6573 706f  f...rH.....respo
+00001020: 6e73 655f 6a73 6f6e da01 6572 2b00 0000  nse_json..er+...
+00001030: 722b 0000 0072 2c00 0000 724e 0000 006c  r+...r,...rN...l
+00001040: 0000 0073 2400 0000 0001 1402 0201 0801  ...s$...........
+00001050: 1001 0801 1201 0801 1201 0801 0e01 0801  ................
+00001060: 0a02 0801 0801 0801 0601 1201 7a16 5061  ............z.Pa
+00001070: 7970 616c 5772 6170 7065 722e 6361 6c6c  ypalWrapper.call
+00001080: 5f61 7069 2902 da10 7765 6268 6f6f 6b5f  _api)...webhook_
+00001090: 6c69 7374 656e 6572 7232 0000 0063 0200  listenerr2...c..
+000010a0: 0000 0000 0000 0000 0000 0a00 0000 0a00  ................
+000010b0: 0000 4300 0000 732c 0100 0074 006a 016a  ..C...s,...t.j.j
+000010c0: 027c 017c 006a 0364 018d 02a0 04a1 0072  .|.|.j.d.......r
+000010d0: 2674 0564 027c 019b 0064 039d 0383 0182  &t.d.|...d......
+000010e0: 0164 0464 056c 066d 077d 0201 007c 0164  .d.d.l.m.}...|.d
+000010f0: 0664 0784 007c 026a 0844 0083 0164 089c  .d...|.j.D...d..
+00001100: 027d 0364 09a0 097c 006a 0a64 0aa1 027d  .}.d...|.j.d...}
+00001110: 047a 347c 006a 0b7c 0464 0b7c 0364 0c8d  .z4|.j.|.d.|.d..
+00001120: 037d 0574 006a 016a 0c7c 0564 0d19 007c  .}.t.j.j.|.d...|
+00001130: 006a 037c 0564 0e19 007c 0564 0f19 0064  .j.|.d...|.d...d
+00001140: 108d 0457 0053 0004 0074 0d6b 0a90 0172  ...W.S...t.k...r
+00001150: 2601 007d 0601 007a 7c7c 066a 0ea0 0fa1  &..}...z||.j....
+00001160: 007d 077c 07a0 1064 11a1 0164 126b 0290  .}.|...d...d.k..
+00001170: 0172 127c 006a 0b7c 0464 1364 148d 027d  .r.|.j.|.d.d...}
+00001180: 087c 08a0 1064 1567 00a1 0244 005d 3e7d  .|...d.g...D.]>}
+00001190: 097c 0964 0e19 007c 016b 0272 d274 006a  .|.d...|.k.r.t.j
+000011a0: 016a 0c7c 0964 0d19 007c 0964 0e19 007c  .j.|.d...|.d...|
+000011b0: 0964 0f19 007c 006a 0364 168d 0402 0001  .d...|.j.d......
+000011c0: 0006 0057 0059 00a2 0c53 0071 d27c 0682  ...W.Y...S.q.|..
+000011d0: 0157 0035 0064 007d 067e 0658 0059 006e  .W.5.d.}.~.X.Y.n
+000011e0: 0258 0064 0053 0029 174e a902 723b 0000  .X.d.S.).N..r;..
+000011f0: 00da 0961 7574 685f 6861 7368 7a12 5765  ...auth_hashz.We
+00001200: 6268 6f6f 6b20 6c69 7374 656e 6572 2028  bhook listener (
+00001210: 7a10 2920 616c 7265 6164 7920 6578 6973  z.) already exis
+00001220: 7473 7201 0000 0029 01da 0d57 6562 686f  tsr....)...Webho
+00001230: 6f6b 4576 656e 7473 6301 0000 0000 0000  okEventsc.......
+00001240: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00001250: 0073 1400 0000 6700 7c00 5d0c 7d01 6400  .s....g.|.].}.d.
+00001260: 7c01 6901 9102 7104 5300 2901 da04 6e61  |.i...q.S.)...na
+00001270: 6d65 722b 0000 0029 0272 3600 0000 da05  mer+...).r6.....
+00001280: 6576 656e 7472 2b00 0000 722b 0000 0072  eventr+...r+...r
+00001290: 2c00 0000 7238 0000 0087 0000 0073 0400  ,...r8.......s..
+000012a0: 0000 0600 0200 7a30 5061 7970 616c 5772  ......z0PaypalWr
+000012b0: 6170 7065 722e 7365 7475 705f 7765 6268  apper.setup_webh
+000012c0: 6f6f 6b73 2e3c 6c6f 6361 6c73 3e2e 3c6c  ooks.<locals>.<l
+000012d0: 6973 7463 6f6d 703e 2902 723b 0000 00da  istcomp>).r;....
+000012e0: 0b65 7665 6e74 5f74 7970 6573 7239 0000  .event_typesr9..
+000012f0: 007a 1a2f 7631 2f6e 6f74 6966 6963 6174  .z./v1/notificat
+00001300: 696f 6e73 2f77 6562 686f 6f6b 7372 3a00  ions/webhooksr:.
+00001310: 0000 a903 723b 0000 0072 3d00 0000 723c  ....r;...r=...r<
+00001320: 0000 0072 5200 0000 723b 0000 0072 7a00  ...rR...r;...rz.
+00001330: 0000 2904 da0a 7765 6268 6f6f 6b5f 6964  ..)...webhook_id
+00001340: 7276 0000 0072 3b00 0000 727a 0000 0072  rv...r;...rz...r
+00001350: 7800 0000 5a1a 5745 4248 4f4f 4b5f 5552  x...Z.WEBHOOK_UR
+00001360: 4c5f 414c 5245 4144 595f 4558 4953 5453  L_ALREADY_EXISTS
+00001370: 725f 0000 0072 5a00 0000 da08 7765 6268  r_...rZ.....webh
+00001380: 6f6f 6b73 2904 727c 0000 0072 3b00 0000  ooks).r|...r;...
+00001390: 727a 0000 0072 7600 0000 2911 7211 0000  rz...rv...).r...
+000013a0: 0072 5000 0000 da06 6669 6c74 6572 da0d  .rP.....filter..
+000013b0: 6170 695f 6175 7468 5f68 6173 68da 0665  api_auth_hash..e
+000013c0: 7869 7374 7372 6f00 0000 5a16 646a 616e  xistsro...Z.djan
+000013d0: 676f 5f70 6179 7061 6c2e 7765 6268 6f6f  go_paypal.webhoo
+000013e0: 6b73 7277 0000 005a 064f 5244 4552 5372  ksrw...Z.ORDERSr
+000013f0: 4c00 0000 7226 0000 0072 4e00 0000 7251  L...r&...rN...rQ
+00001400: 0000 0072 0c00 0000 7248 0000 0072 6700  ...r....rH...rg.
+00001410: 0000 725c 0000 0029 0a72 2700 0000 7274  ..r\...).r'...rt
+00001420: 0000 0072 7700 0000 723c 0000 005a 0b77  ...rw...r<...Z.w
+00001430: 6562 686f 6f6b 5f61 7069 da0d 7265 7370  ebhook_api..resp
+00001440: 6f6e 7365 5f64 6963 7472 7300 0000 7272  onse_dictrs...rr
+00001450: 0000 005a 0c77 6562 686f 6f6b 5f6c 6973  ...Z.webhook_lis
+00001460: 74da 0777 6562 686f 6f6b 722b 0000 0072  t..webhookr+...r
+00001470: 2b00 0000 722c 0000 00da 0e73 6574 7570  +...r,.....setup
+00001480: 5f77 6562 686f 6f6b 7382 0000 0073 3400  _webhooks....s4.
+00001490: 0000 0001 1601 1001 0c02 1601 0e01 0201  ................
+000014a0: 1001 0601 0601 0401 0601 06fc 0806 1201  ................
+000014b0: 0a01 1001 0e01 1001 0c01 0601 0600 0600  ................
+000014c0: 0600 04ff 1403 7a1c 5061 7970 616c 5772  ......z.PaypalWr
+000014d0: 6170 7065 722e 7365 7475 705f 7765 6268  apper.setup_webh
+000014e0: 6f6f 6b73 2903 727c 0000 00da 0a70 6174  ooks).r|.....pat
+000014f0: 6368 5f64 6174 6172 3200 0000 6303 0000  ch_datar2...c...
+00001500: 0000 0000 0000 0000 0007 0000 000a 0000  ................
+00001510: 0043 0000 0073 9400 0000 7a12 7400 6a01  .C...s....z.t.j.
+00001520: 6a02 7c01 6401 8d01 7d03 5700 6e3a 0400  j.|.d...}.W.n:..
+00001530: 7400 6a03 6b0a 724c 0100 7d04 0100 7a1a  t.j.k.rL..}...z.
+00001540: 7404 a005 6402 7c01 9b00 6403 9d03 a101  t...d.|...d.....
+00001550: 0100 7c04 8201 5700 3500 6400 7d04 7e04  ..|...W.5.d.}.~.
+00001560: 5800 5900 6e02 5800 6404 a006 7c00 6a07  X.Y.n.X.d...|.j.
+00001570: 6405 7c03 6a08 9b00 9d02 a102 7d05 7c00  d.|.j.......}.|.
+00001580: 6a09 7c05 6406 7c02 6407 8d03 7d06 7c06  j.|.d.|.d...}.|.
+00001590: 6408 1900 7c03 5f0a 7c06 6409 1900 7c03  d...|._.|.d...|.
+000015a0: 5f0b 7c03 a00c a100 0100 7c03 5300 290a  _.|.......|.S.).
+000015b0: 4e29 0172 7c00 0000 7a10 5765 6268 6f6f  N).r|...z.Webhoo
+000015c0: 6b20 7769 7468 2069 6420 7a4c 2064 6f65  k with id zL doe
+000015d0: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
+000015e0: 6865 2064 6174 6162 6173 652e 2053 6574  he database. Set
+000015f0: 2075 7020 7765 6268 6f6f 6b73 2062 7920   up webhooks by 
+00001600: 6361 6c6c 696e 6720 2273 6574 7570 5f77  calling "setup_w
+00001610: 6562 686f 6f6b 7322 7239 0000 00fa 1b2f  ebhooks"r9...../
+00001620: 7631 2f6e 6f74 6966 6963 6174 696f 6e73  v1/notifications
+00001630: 2f77 6562 686f 6f6b 732f 7261 0000 0072  /webhooks/ra...r
+00001640: 7b00 0000 723b 0000 0072 7a00 0000 290d  {...r;...rz...).
+00001650: 7211 0000 0072 5000 0000 725c 0000 00da  r....rP...r\....
+00001660: 0c44 6f65 734e 6f74 4578 6973 74da 0877  .DoesNotExist..w
+00001670: 6172 6e69 6e67 73da 0477 6172 6e72 4c00  arnings..warnrL.
+00001680: 0000 7226 0000 0072 7c00 0000 724e 0000  ..r&...r|...rN..
+00001690: 0072 3b00 0000 727a 0000 0072 5d00 0000  .r;...rz...r]...
+000016a0: 2907 7227 0000 0072 7c00 0000 7284 0000  ).r'...r|...r...
+000016b0: 00da 0e70 6179 7061 6c5f 7765 6268 6f6f  ...paypal_webhoo
+000016c0: 6b72 7300 0000 723b 0000 005a 1577 6562  krs...r;...Z.web
+000016d0: 686f 6f6b 5f72 6573 706f 6e73 655f 6469  hook_response_di
+000016e0: 6374 722b 0000 0072 2b00 0000 722c 0000  ctr+...r+...r,..
+000016f0: 00da 0d70 6174 6368 5f77 6562 686f 6f6b  ...patch_webhook
+00001700: 9c00 0000 7316 0000 0000 0102 0112 0112  ....s...........
+00001710: 0112 0116 0116 0110 010a 010a 0108 017a  ...............z
+00001720: 1b50 6179 7061 6c57 7261 7070 6572 2e70  .PaypalWrapper.p
+00001730: 6174 6368 5f77 6562 686f 6f6b 6302 0000  atch_webhookc...
+00001740: 0000 0000 0000 0000 0005 0000 000a 0000  ................
+00001750: 0043 0000 0073 7000 0000 7a16 7400 6a01  .C...sp...z.t.j.
+00001760: 6a02 7c01 7c00 6a03 6401 8d02 7d02 5700  j.|.|.j.d...}.W.
+00001770: 6e28 0400 7400 6a04 6b0a 723e 0100 7d03  n(..t.j.k.r>..}.
+00001780: 0100 7a08 7c03 8201 5700 3500 6400 7d03  ..z.|...W.5.d.}.
+00001790: 7e03 5800 5900 6e02 5800 6402 a005 7c00  ~.X.Y.n.X.d...|.
+000017a0: 6a06 6403 7c02 6a07 9b00 9d02 a102 7d04  j.d.|.j.......}.
+000017b0: 7c00 6a08 7c04 6404 6405 8d02 0100 7c02  |.j.|.d.d.....|.
+000017c0: a009 a100 0100 6406 5300 2907 4e72 7500  ......d.S.).Nru.
+000017d0: 0000 7239 0000 0072 8500 0000 7262 0000  ..r9...r....rb..
+000017e0: 0072 5a00 0000 5429 0a72 1100 0000 7250  .rZ...T).r....rP
+000017f0: 0000 0072 5c00 0000 727f 0000 0072 8600  ...r\...r....r..
+00001800: 0000 724c 0000 0072 2600 0000 727c 0000  ..rL...r&...r|..
+00001810: 0072 4e00 0000 726d 0000 0029 0572 2700  .rN...rm...).r'.
+00001820: 0000 7274 0000 0072 8900 0000 7273 0000  ..rt...r....rs..
+00001830: 0072 3b00 0000 722b 0000 0072 2b00 0000  .r;...r+...r+...
+00001840: 722c 0000 00da 0e64 656c 6574 655f 7765  r,.....delete_we
+00001850: 6268 6f6f 6ba9 0000 0073 1000 0000 0001  bhook....s......
+00001860: 0201 1601 1201 1601 1601 0e01 0801 7a1c  ..............z.
+00001870: 5061 7970 616c 5772 6170 7065 722e 6465  PaypalWrapper.de
+00001880: 6c65 7465 5f77 6562 686f 6f6b 2903 da07  lete_webhook)...
+00001890: 7265 7175 6573 7472 7c00 0000 7232 0000  requestr|...r2..
+000018a0: 0063 0300 0000 0000 0000 0000 0000 0d00  .c..............
+000018b0: 0000 0800 0000 4300 0000 739a 0000 007c  ......C...s....|
+000018c0: 016a 007d 037c 03a0 0164 01a1 017d 047c  .j.}.|...d...}.|
+000018d0: 03a0 0164 02a1 017d 057c 03a0 0164 03a1  ...d...}.|...d..
+000018e0: 017d 067c 03a0 0164 04a1 017d 077c 03a0  .}.|...d...}.|..
+000018f0: 0164 05a1 017d 0874 02a0 037c 016a 04a0  .d...}.t...|.j..
+00001900: 0564 06a1 01a1 017d 097c 047c 057c 067c  .d.....}.|.|.|.|
+00001910: 077c 087c 027c 0964 079c 077d 0a7c 006a  .|.|.|.d...}.|.j
+00001920: 069b 0064 089d 027d 0b7c 006a 077c 0b64  ...d...}.|.j.|.d
+00001930: 097c 0a64 0a8d 037d 0c7c 0ca0 0164 0ba1  .|.d...}.|...d..
+00001940: 0164 0c6b 0272 8c64 0d53 0074 0864 0e7c  .d.k.r.d.S.t.d.|
+00001950: 0c83 0282 0164 0053 0029 0f4e 7a10 5061  .....d.S.).Nz.Pa
+00001960: 7970 616c 2d41 7574 682d 416c 676f 7a0f  ypal-Auth-Algoz.
+00001970: 5061 7970 616c 2d43 6572 742d 5572 6c7a  Paypal-Cert-Urlz
+00001980: 1650 6179 7061 6c2d 5472 616e 736d 6973  .Paypal-Transmis
+00001990: 7369 6f6e 2d49 647a 1850 6179 7061 6c2d  sion-Idz.Paypal-
+000019a0: 5472 616e 736d 6973 7369 6f6e 2d54 696d  Transmission-Tim
+000019b0: 657a 1750 6179 7061 6c2d 5472 616e 736d  ez.Paypal-Transm
+000019c0: 6973 7369 6f6e 2d53 6967 7a05 7574 662d  ission-Sigz.utf-
+000019d0: 3829 07da 0961 7574 685f 616c 676f da08  8)...auth_algo..
+000019e0: 6365 7274 5f75 726c da0f 7472 616e 736d  cert_url..transm
+000019f0: 6973 7369 6f6e 5f69 64da 1174 7261 6e73  ission_id..trans
+00001a00: 6d69 7373 696f 6e5f 7469 6d65 da10 7472  mission_time..tr
+00001a10: 616e 736d 6973 7369 6f6e 5f73 6967 727c  ansmission_sigr|
+00001a20: 0000 005a 0d77 6562 686f 6f6b 5f65 7665  ...Z.webhook_eve
+00001a30: 6e74 7a2a 2f76 312f 6e6f 7469 6669 6361  ntz*/v1/notifica
+00001a40: 7469 6f6e 732f 7665 7269 6679 2d77 6562  tions/verify-web
+00001a50: 686f 6f6b 2d73 6967 6e61 7475 7265 723a  hook-signaturer:
+00001a60: 0000 0072 7b00 0000 5a13 7665 7269 6669  ...r{...Z.verifi
+00001a70: 6361 7469 6f6e 5f73 7461 7475 73da 0753  cation_status..S
+00001a80: 5543 4345 5353 547a 1b57 6562 686f 6f6b  UCCESSTz.Webhook
+00001a90: 2076 6572 6966 6963 6174 696f 6e20 6661   verification fa
+00001aa0: 696c 6564 2909 7266 0000 0072 5c00 0000  iled).rf...r\...
+00001ab0: 7267 0000 00da 056c 6f61 6473 da04 626f  rg.....loads..bo
+00001ac0: 6479 da06 6465 636f 6465 7226 0000 0072  dy..decoder&...r
+00001ad0: 4e00 0000 720d 0000 0029 0d72 2700 0000  N...r....).r'...
+00001ae0: 728c 0000 0072 7c00 0000 7266 0000 0072  r....r|...rf...r
+00001af0: 8d00 0000 728e 0000 0072 8f00 0000 7290  ....r....r....r.
+00001b00: 0000 0072 9100 0000 da0c 7265 7175 6573  ...r......reques
+00001b10: 745f 6461 7461 5a14 7665 7269 6669 6361  t_dataZ.verifica
+00001b20: 7469 6f6e 5f70 6179 6c6f 6164 723b 0000  tion_payloadr;..
+00001b30: 00da 0372 6573 722b 0000 0072 2b00 0000  ...resr+...r+...
+00001b40: 722c 0000 00da 1476 6572 6966 795f 7765  r,.....verify_we
+00001b50: 6268 6f6f 6b5f 6576 656e 74b3 0000 0073  bhook_event....s
+00001b60: 2800 0000 0001 0601 0a01 0a01 0a01 0a01  (...............
+00001b70: 0a01 1202 0201 0201 0201 0201 0201 0201  ................
+00001b80: 02f9 0609 0c01 1001 0e01 0401 7a22 5061  ............z"Pa
+00001b90: 7970 616c 5772 6170 7065 722e 7665 7269  ypalWrapper.veri
+00001ba0: 6679 5f77 6562 686f 6f6b 5f65 7665 6e74  fy_webhook_event
+00001bb0: 2901 7232 0000 0063 0100 0000 0000 0000  ).r2...c........
+00001bc0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001bd0: 730c 0000 007c 00a0 00a1 0001 0064 0153  s....|.......d.S
+00001be0: 0029 024e 5429 0172 6a00 0000 a901 7227  .).NT).rj.....r'
+00001bf0: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
+00001c00: 0000 da0f 7665 7269 6679 5f61 7069 5f6b  ....verify_api_k
+00001c10: 6579 73ca 0000 0073 0400 0000 0001 0801  eys....s........
+00001c20: 7a1d 5061 7970 616c 5772 6170 7065 722e  z.PaypalWrapper.
+00001c30: 7665 7269 6679 5f61 7069 5f6b 6579 7363  verify_api_keysc
+00001c40: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00001c50: 0500 0000 4300 0000 7358 0000 007c 006a  ....C...sX...|.j
+00001c60: 0073 147c 00a0 01a1 007d 017c 016a 0253  .s.|.....}.|.j.S
+00001c70: 007c 006a 036a 047c 006a 0564 018d 017d  .|.j.j.|.j.d...}
+00001c80: 0274 06a0 077c 02a1 017d 037c 0373 507c  .t...|...}.|.sP|
+00001c90: 00a0 01a1 007d 017c 016a 027d 0374 06a0  .....}.|.j.}.t..
+00001ca0: 087c 027c 037c 006a 00a1 0301 007c 0353  .|.|.|.j.....|.S
+00001cb0: 0064 0053 0029 024e 2901 7276 0000 0029  .d.S.).N).rv...)
+00001cc0: 09da 1261 7574 685f 6361 6368 655f 7469  ...auth_cache_ti
+00001cd0: 6d65 6f75 74da 115f 6175 7468 6f72 697a  meout.._authoriz
+00001ce0: 655f 636c 6965 6e74 da0c 6163 6365 7373  e_client..access
+00001cf0: 5f74 6f6b 656e da0e 6175 7468 5f63 6163  _token..auth_cac
+00001d00: 6865 5f6b 6579 724c 0000 0072 7f00 0000  he_keyrL...r....
+00001d10: 7207 0000 0072 5c00 0000 da03 7365 7429  r....r\.....set)
+00001d20: 0472 2700 0000 da0d 6175 7468 5f72 6573  .r'.....auth_res
+00001d30: 706f 6e73 65da 0963 6163 6865 5f6b 6579  ponse..cache_key
+00001d40: 729d 0000 0072 2b00 0000 722b 0000 0072  r....r+...r+...r
+00001d50: 2c00 0000 726a 0000 00ce 0000 0073 1400  ,...rj.......s..
+00001d60: 0000 0001 0601 0801 0602 1001 0a01 0401  ................
+00001d70: 0801 0601 1001 7a1f 5061 7970 616c 5772  ......z.PaypalWr
+00001d80: 6170 7065 722e 5f67 6574 5f61 6363 6573  apper._get_acces
+00001d90: 735f 746f 6b65 6e63 0100 0000 0000 0000  s_tokenc........
+00001da0: 0000 0000 0800 0000 0a00 0000 4300 0000  ............C...
+00001db0: 739e 0000 007c 006a 009b 007c 006a 019b  s....|.j...|.j..
+00001dc0: 009d 027d 0174 027c 006a 036a 047c 006a  ...}.t.|.j.j.|.j
+00001dd0: 036a 0583 027d 0264 0164 0264 039c 027d  .j...}.d.d.d...}
+00001de0: 0364 0464 0569 017d 047a 2e74 066a 077c  .d.d.i.}.z.t.j.|
+00001df0: 017c 037c 047c 0264 068d 047d 057c 05a0  .|.|.|.d...}.|..
+00001e00: 08a1 0001 007c 05a0 09a1 007d 0674 0a66  .....|.....}.t.f
+00001e10: 007c 068e 0157 0053 0004 0074 066a 0b6b  .|...W.S...t.j.k
+00001e20: 0a72 9801 007d 0701 007a 1674 0c74 0d7c  .r...}...z.t.t.|
+00001e30: 0783 017c 076a 0e64 078d 0282 0157 0035  ...|.j.d.....W.5
+00001e40: 0064 007d 077e 0758 0059 006e 0258 0064  .d.}.~.X.Y.n.X.d
+00001e50: 0053 0029 084e 7263 0000 007a 2161 7070  .S.).Nrc...z!app
+00001e60: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
+00001e70: 6f72 6d2d 7572 6c65 6e63 6f64 6564 2902  orm-urlencoded).
+00001e80: da06 4163 6365 7074 7265 0000 005a 0a67  ..Acceptre...Z.g
+00001e90: 7261 6e74 5f74 7970 655a 1263 6c69 656e  rant_typeZ.clien
+00001ea0: 745f 6372 6564 656e 7469 616c 7329 0372  t_credentials).r
+00001eb0: 6600 0000 723c 0000 0072 1f00 0000 7269  f...r<...r....ri
+00001ec0: 0000 0029 0f72 2600 0000 da08 6175 7468  ...).r&.....auth
+00001ed0: 5f75 726c 7209 0000 0072 1f00 0000 da09  _urlr....r......
+00001ee0: 636c 6965 6e74 5f69 64da 0d63 6c69 656e  client_id..clien
+00001ef0: 745f 7365 6372 6574 726b 0000 0072 4500  t_secretrk...rE.
+00001f00: 0000 726e 0000 0072 6700 0000 7212 0000  ..rn...rg...r...
+00001f10: 0072 7000 0000 720b 0000 0072 7100 0000  .rp...r....rq...
+00001f20: 7248 0000 0029 0872 2700 0000 723b 0000  rH...).r'...r;..
+00001f30: 005a 0861 7069 5f61 7574 6872 6600 0000  .Z.api_authrf...
+00001f40: 723c 0000 0072 4800 0000 7272 0000 0072  r<...rH...rr...r
+00001f50: 7300 0000 722b 0000 0072 2b00 0000 722c  s...r+...r+...r,
+00001f60: 0000 0072 9c00 0000 db00 0000 7316 0000  ...r........s...
+00001f70: 0000 0210 0212 010a 0108 0202 0112 0108  ................
+00001f80: 0108 010c 0112 017a 1f50 6179 7061 6c57  .......z.PaypalW
+00001f90: 7261 7070 6572 2e5f 6175 7468 6f72 697a  rapper._authoriz
+00001fa0: 655f 636c 6965 6e74 6301 0000 0000 0000  e_clientc.......
+00001fb0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001fc0: 0073 2200 0000 7400 a001 7c00 6a02 6a03  .s"...t...|.j.j.
+00001fd0: 9b00 7c00 6a02 6a04 9b00 9d02 a005 a100  ..|.j.j.........
+00001fe0: a101 a006 a100 5300 7220 0000 0029 07da  ......S.r ...)..
+00001ff0: 0768 6173 686c 6962 da03 6d64 3572 1f00  .hashlib..md5r..
+00002000: 0000 72a4 0000 0072 a500 0000 da06 656e  ..r....r......en
+00002010: 636f 6465 da09 6865 7864 6967 6573 7472  code..hexdigestr
+00002020: 9900 0000 722b 0000 0072 2b00 0000 722c  ....r+...r+...r,
+00002030: 0000 0072 7f00 0000 eb00 0000 7302 0000  ...r........s...
+00002040: 0000 027a 1b50 6179 7061 6c57 7261 7070  ...z.PaypalWrapp
+00002050: 6572 2e61 7069 5f61 7574 685f 6861 7368  er.api_auth_hash
+00002060: 2901 4e29 014e 2936 da08 5f5f 6e61 6d65  ).N).N)6..__name
+00002070: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00002080: 5f5f 7175 616c 6e61 6d65 5f5f 724c 0000  __qualname__rL..
+00002090: 0072 2300 0000 5a15 444a 414e 474f 5f50  .r#...Z.DJANGO_P
+000020a0: 4159 5041 4c5f 5645 5253 494f 4eda 1169  AYPAL_VERSION..i
+000020b0: 6e74 6572 6661 6365 5f76 6572 7369 6f6e  nterface_version
+000020c0: 5a0e 5041 5950 414c 5f41 5049 5f55 524c  Z.PAYPAL_API_URL
+000020d0: 7226 0000 005a 1650 4159 5041 4c5f 5341  r&...Z.PAYPAL_SA
+000020e0: 4e44 424f 585f 4150 495f 5552 4c72 2500  NDBOX_API_URLr%.
+000020f0: 0000 5a1a 5041 5950 414c 5f4f 5244 4552  ..Z.PAYPAL_ORDER
+00002100: 535f 4150 495f 454e 4450 4f49 4e54 724d  S_API_ENDPOINTrM
+00002110: 0000 005a 0f50 4159 5041 4c5f 4155 5448  ...Z.PAYPAL_AUTH
+00002120: 5f55 524c 72a3 0000 005a 1950 4159 5041  _URLr....Z.PAYPA
+00002130: 4c5f 4155 5448 5f43 4143 4845 5f54 494d  L_AUTH_CACHE_TIM
+00002140: 454f 5554 729b 0000 005a 1550 4159 5041  EOUTr....Z.PAYPA
+00002150: 4c5f 4155 5448 5f43 4143 4845 5f4b 4559  L_AUTH_CACHE_KEY
+00002160: 729e 0000 0072 1f00 0000 7217 0000 00da  r....r....r.....
+00002170: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00002180: 7222 0000 005a 1250 4159 5041 4c5f 5355  r"...Z.PAYPAL_SU
+00002190: 4343 4553 535f 5552 4c5a 1750 4159 5041  CCESS_URLZ.PAYPA
+000021a0: 4c5f 4341 4e43 454c 4c41 5449 4f4e 5f55  L_CANCELLATION_U
+000021b0: 524c 7203 0000 0072 0400 0000 7216 0000  RLr....r....r...
+000021c0: 0072 1300 0000 7214 0000 0072 1800 0000  .r....r....r....
+000021d0: 7257 0000 0072 7100 0000 7219 0000 0072  rW...rq...r....r
+000021e0: 5e00 0000 721a 0000 0072 6000 0000 7206  ^...r....r`...r.
+000021f0: 0000 0072 0500 0000 724e 0000 0072 1100  ...r....rN...r..
+00002200: 0000 7283 0000 0072 8a00 0000 da04 626f  ..r....r......bo
+00002210: 6f6c 728b 0000 0072 0800 0000 7298 0000  olr....r....r...
+00002220: 0072 9a00 0000 726a 0000 0072 1200 0000  .r....rj...r....
+00002230: 729c 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00002240: 7f00 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00002250: 6c5f 5f72 2b00 0000 722b 0000 0072 2900  l__r+...r+...r).
+00002260: 0000 722c 0000 0072 1e00 0000 2400 0000  ..r,...r....$...
+00002270: 733e 0000 000a 010c 0206 0106 0106 0106  s>..............
+00002280: 0106 0106 020c 0214 0b02 0104 0104 f902  ................
+00002290: 0206 0106 0102 0102 0302 f80c 2410 0c10  ............$...
+000022a0: 0620 1610 1a16 0d10 0a12 170e 040e 0d0e  . ..............
+000022b0: 1002 0172 1e00 0000 292e da0a 5f5f 6675  ...r....)...__fu
+000022c0: 7475 7265 5f5f 7202 0000 0072 a600 0000  ture__r....r....
+000022d0: 7267 0000 0072 8700 0000 da06 7479 7069  rg...r......typi
+000022e0: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
+000022f0: 0072 0600 0000 da11 646a 616e 676f 2e63  .r......django.c
+00002300: 6f72 652e 6361 6368 6572 0700 0000 726b  ore.cacher....rk
+00002310: 0000 00da 0b64 6a61 6e67 6f2e 6874 7470  .....django.http
+00002320: 7208 0000 005a 0d72 6571 7565 7374 732e  r....Z.requests.
+00002330: 6175 7468 7209 0000 00da 0d64 6a61 6e67  authr......djang
+00002340: 6f5f 7061 7970 616c 720a 0000 0072 2300  o_paypalr....r#.
+00002350: 0000 da18 646a 616e 676f 5f70 6179 7061  ....django_paypa
+00002360: 6c2e 6578 6365 7074 696f 6e73 720b 0000  l.exceptionsr...
+00002370: 0072 0c00 0000 720d 0000 00da 1464 6a61  .r....r......dja
+00002380: 6e67 6f5f 7061 7970 616c 2e6d 6f64 656c  ngo_paypal.model
+00002390: 7372 0e00 0000 720f 0000 0072 1000 0000  sr....r....r....
+000023a0: 7211 0000 00da 1764 6a61 6e67 6f5f 7061  r......django_pa
+000023b0: 7970 616c 2e61 7069 5f74 7970 6573 7212  ypal.api_typesr.
+000023c0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+000023d0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000023e0: 0072 1900 0000 721a 0000 005a 1364 6a61  .r....r....Z.dja
+000023f0: 6e67 6f5f 7061 7970 616c 2e75 7469 6c73  ngo_paypal.utils
+00002400: 721b 0000 005a 1564 6a61 6e67 6f5f 7061  r....Z.django_pa
+00002410: 7970 616c 2e73 6967 6e61 6c73 721c 0000  ypal.signalsr...
+00002420: 0072 1d00 0000 da06 6f62 6a65 6374 721e  .r......objectr.
+00002430: 0000 0072 2b00 0000 722b 0000 0072 2b00  ...r+...r+...r+.
+00002440: 0000 722c 0000 00da 083c 6d6f 6475 6c65  ..r,.....<module
+00002450: 3e01 0000 0073 1e00 0000 0c02 0801 0801  >....s..........
+00002460: 0801 1802 0c01 0801 0c01 0c02 0c01 1401  ................
+00002470: 1806 2c0b 0c01 1003                      ..,.....
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/api_types.py` & `django-paypal-plus-1.1.1/django_paypal/api_types.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0001_initial.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0002_auto_20171002_1551.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0002_auto_20171002_1551.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0003_auto_20200124_1528.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0003_auto_20200124_1528.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0004_paypalpayment_related_resource_state.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0004_paypalpayment_related_resource_state.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0005_auto_20240207_0630.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0005_auto_20240207_0630.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/0006_auto_20240424_0727.py` & `django-paypal-plus-1.1.1/django_paypal/migrations/0006_auto_20240424_0727.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0002_auto_20171002_1551.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0003_auto_20200124_1528.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0004_paypalpayment_related_resource_state.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0005_auto_20240207_0630.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr 23 04:40:19 2024 UTC, .py size: 4611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b33b 2766 0312 0000  U........;'f....
+00000000: 550d 0d0a 0000 0000 bf83 2e66 0312 0000  U..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 6400 6401 6c05 5a01 4700  m.Z...d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6503 6a06 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2905 e900 0000 004e 2902 da0a  d.S.)......N)...
 00000070: 6d69 6772 6174 696f 6e73 da06 6d6f 6465  migrations..mode
@@ -45,33 +45,33 @@
 000002c0: 6a06 6a14 6a15 643b 6433 6434 8d03 6602  j.j.j.d;d3d4..f.
 000002d0: 643c 6506 6a12 6404 6509 6a13 6a06 6a14  d<e.j.d.e.j.j.j.
 000002e0: 6a15 643d 643e 643f 8d04 6602 6706 6411  j.d=d>d?..f.g.d.
 000002f0: 8d02 6504 6a16 6440 6431 6506 6a12 6509  ..e.j.d@d1e.j.e.
 00000300: 6a13 6a06 6a14 6a15 6441 6433 6434 8d03  j.j.j.j.dAd3d4..
 00000310: 6442 8d03 670c 5a17 6443 5300 2944 da09  dB..g.Z.dCS.)D..
 00000320: 4d69 6772 6174 696f 6e29 02da 0d64 6a61  Migration)...dja
-00000330: 6e67 6f5f 7061 7970 616c da29 3030 3034  ngo_paypal.)0004
+00000330: 6e67 6f5f 7061 7970 616c 5a29 3030 3034  ngo_paypalZ)0004
 00000340: 5f70 6179 7061 6c70 6179 6d65 6e74 5f72  _paypalpayment_r
 00000350: 656c 6174 6564 5f72 6573 6f75 7263 655f  elated_resource_
 00000360: 7374 6174 65da 1150 6179 7061 6c41 5049  state..PaypalAPI
 00000370: 506f 7374 4461 7461 da02 6964 5446 da02  PostData..idTF..
 00000380: 4944 2904 da0c 6175 746f 5f63 7265 6174  ID)...auto_creat
 00000390: 6564 da0b 7072 696d 6172 795f 6b65 79da  ed..primary_key.
 000003a0: 0973 6572 6961 6c69 7a65 da0c 7665 7262  .serialize..verb
 000003b0: 6f73 655f 6e61 6d65 da03 7572 6ce9 ff00  ose_name..url...
 000003c0: 0000 da03 5552 4c29 03da 0562 6c61 6e6b  ....URL)...blank
-000003d0: da0a 6d61 785f 6c65 6e67 7468 720d 0000  ..max_lengthr...
+000003d0: da0a 6d61 785f 6c65 6e67 7468 720c 0000  ..max_lengthr...
 000003e0: 00da 0970 6f73 745f 6461 7461 7a09 506f  ...post_dataz.Po
-000003f0: 7374 2044 6174 6129 0172 0d00 0000 da0a  st Data).r......
+000003f0: 7374 2044 6174 6129 0172 0c00 0000 da0a  st Data).r......
 00000400: 6372 6561 7465 645f 6174 2901 da0c 6175  created_at)...au
 00000410: 746f 5f6e 6f77 5f61 6464 2902 da04 6e61  to_now_add)...na
 00000420: 6d65 da06 6669 656c 6473 da0b 5061 7970  me..fields..Payp
 00000430: 616c 4f72 6465 72da 086f 7264 6572 5f69  alOrder..order_i
-00000440: 647a 084f 7264 6572 2049 4429 0372 1200  dz.Order ID).r..
-00000450: 0000 da06 756e 6971 7565 720d 0000 00da  ....uniquer.....
+00000440: 647a 084f 7264 6572 2049 4429 0372 1100  dz.Order ID).r..
+00000450: 0000 da06 756e 6971 7565 720c 0000 00da  ....uniquer.....
 00000460: 0673 7461 7475 73da 0653 7461 7475 73da  .status..Status.
 00000470: 0d50 6179 7061 6c57 6562 686f 6f6b da0a  .PaypalWebhook..
 00000480: 7765 6268 6f6f 6b5f 6964 7a0a 5765 6268  webhook_idz.Webh
 00000490: 6f6f 6b20 4944 da0b 6576 656e 745f 7479  ook ID..event_ty
 000004a0: 7065 737a 1541 6374 6976 6520 5765 6268  pesz.Active Webh
 000004b0: 6f6f 6b20 4576 656e 7473 5a0a 5061 7970  ook EventsZ.Payp
 000004c0: 616c 4974 656d da10 4c65 6761 6379 5061  alItem..LegacyPa
@@ -81,17 +81,17 @@
 00000500: 6567 6163 7950 6179 7061 6c50 6179 6d65  egacyPaypalPayme
 00000510: 6e74 5a11 5061 7970 616c 5472 616e 7361  ntZ.PaypalTransa
 00000520: 6374 696f 6eda 174c 6567 6163 7950 6179  ction..LegacyPay
 00000530: 7061 6c54 7261 6e73 6163 7469 6f6e 5a10  palTransactionZ.
 00000540: 6c65 6761 6379 7061 7970 616c 6974 656d  legacypaypalitem
 00000550: 7a24 4c65 6761 6379 2050 6179 7061 6c20  z$Legacy Paypal 
 00000560: 4974 656d 2028 7061 796d 656e 7473 2076  Item (payments v
-00000570: 3120 4150 4929 2902 720d 0000 00da 1376  1 API)).r......v
+00000570: 3120 4150 4929 2902 720c 0000 00da 1376  1 API)).r......v
 00000580: 6572 626f 7365 5f6e 616d 655f 706c 7572  erbose_name_plur
-00000590: 616c 2902 7216 0000 00da 076f 7074 696f  al).r......optio
+00000590: 616c 2902 7215 0000 00da 076f 7074 696f  al).r......optio
 000005a0: 6e73 5a13 6c65 6761 6379 7061 7970 616c  nsZ.legacypaypal
 000005b0: 7061 796d 656e 747a 274c 6567 6163 7920  paymentz'Legacy 
 000005c0: 5061 7970 616c 2050 6179 6d65 6e74 2028  Paypal Payment (
 000005d0: 7061 796d 656e 7473 2076 3120 4150 4929  payments v1 API)
 000005e0: 7a28 4c65 6761 6379 2050 6179 7061 6c20  z(Legacy Paypal 
 000005f0: 5061 796d 656e 7473 2028 7061 796d 656e  Payments (paymen
 00000600: 7473 2076 3120 4150 4929 5a17 6c65 6761  ts v1 API)Z.lega
@@ -115,36 +115,36 @@
 00000720: 6f6f 6bda 1150 6179 7061 6c41 5049 5265  ook..PaypalAPIRe
 00000730: 7370 6f6e 7365 da0d 7265 7370 6f6e 7365  sponse..response
 00000740: 5f64 6174 617a 0d52 6573 706f 6e73 6520  _dataz.Response 
 00000750: 4461 7461 da0d 6170 695f 7265 7370 6f6e  Data..api_respon
 00000760: 7365 73da 0470 6f73 74da 0972 6573 706f  ses..post..respo
 00000770: 6e73 6573 7a1f 646a 616e 676f 5f70 6179  nsesz.django_pay
 00000780: 7061 6c2e 5061 7970 616c 4150 4950 6f73  pal.PaypalAPIPos
-00000790: 7444 6174 6129 04da 046e 756c 6c72 2d00  tData)...nullr-.
-000007a0: 0000 722e 0000 0072 2f00 0000 5a11 7061  ..r....r/...Z.pa
+00000790: 7444 6174 6129 04da 046e 756c 6c72 2c00  tData)...nullr,.
+000007a0: 0000 722d 0000 0072 2e00 0000 5a11 7061  ..r-...r....Z.pa
 000007b0: 7970 616c 6170 6970 6f73 7464 6174 61da  ypalapipostdata.
 000007c0: 0961 7069 5f70 6f73 7473 2903 da0a 6d6f  .api_posts)...mo
-000007d0: 6465 6c5f 6e61 6d65 7216 0000 00da 0566  del_namer......f
+000007d0: 6465 6c5f 6e61 6d65 7215 0000 00da 0566  del_namer......f
 000007e0: 6965 6c64 4e29 18da 085f 5f6e 616d 655f  ieldN)...__name_
 000007f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000800: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
 00000810: 656e 6465 6e63 6965 7372 0200 0000 da0b  endenciesr......
 00000820: 4372 6561 7465 4d6f 6465 6c72 0300 0000  CreateModelr....
 00000830: da09 4175 746f 4669 656c 64da 0943 6861  ..AutoField..Cha
 00000840: 7246 6965 6c64 da06 646a 616e 676f da07  rField..django..
 00000850: 636f 6e74 7269 62da 0870 6f73 7467 7265  contrib..postgre
-00000860: 7372 1700 0000 da05 6a73 6f6e 62da 094a  sr......jsonb..J
+00000860: 7372 1600 0000 da05 6a73 6f6e 62da 094a  sr......jsonb..J
 00000870: 534f 4e46 6965 6c64 da0d 4461 7465 5469  SONField..DateTi
 00000880: 6d65 4669 656c 64da 0b52 656e 616d 654d  meField..RenameM
 00000890: 6f64 656c da11 416c 7465 724d 6f64 656c  odel..AlterModel
 000008a0: 4f70 7469 6f6e 73da 0a46 6f72 6569 676e  Options..Foreign
 000008b0: 4b65 79da 0264 62da 0864 656c 6574 696f  Key..db..deletio
 000008c0: 6eda 0743 4153 4341 4445 da08 4164 6446  n..CASCADE..AddF
 000008d0: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
-000008e0: a900 7250 0000 0072 5000 0000 fa77 2f55  ..rP...rP....w/U
+000008e0: a900 724f 0000 0072 4f00 0000 fa77 2f55  ..rO...rO....w/U
 000008f0: 7365 7273 2f74 696d 7461 6d2f 2e70 7965  sers/timtam/.pye
 00000900: 6e76 2f76 6572 7369 6f6e 732f 7366 2d33  nv/versions/sf-3
 00000910: 2e38 2e31 322f 6c69 622f 7079 7468 6f6e  .8.12/lib/python
 00000920: 332e 382f 7369 7465 2d70 6163 6b61 6765  3.8/site-package
 00000930: 732f 646a 616e 676f 5f70 6179 7061 6c2f  s/django_paypal/
 00000940: 6d69 6772 6174 696f 6e73 2f30 3030 355f  migrations/0005_
 00000950: 6175 746f 5f32 3032 3430 3230 375f 3036  auto_20240207_06
@@ -157,14 +157,14 @@
 000009c0: 0102 0108 fe04 0404 0102 0108 fe04 0404  ................
 000009d0: 0102 0108 fe04 0404 0102 0214 0116 011a  ................
 000009e0: 011a fc02 fe04 0904 0102 0214 0112 0116  ................
 000009f0: 010e 011a 011c fa02 fe04 0b04 0102 0102  ................
 00000a00: 0116 fd04 b972 0400 0000 2907 5a24 646a  .....r....).Z$dj
 00000a10: 616e 676f 2e63 6f6e 7472 6962 2e70 6f73  ango.contrib.pos
 00000a20: 7467 7265 732e 6669 656c 6473 2e6a 736f  tgres.fields.jso
-00000a30: 6e62 7242 0000 00da 0964 6a61 6e67 6f2e  nbrB.....django.
+00000a30: 6e62 7241 0000 00da 0964 6a61 6e67 6f2e  nbrA.....django.
 00000a40: 6462 7202 0000 0072 0300 0000 da19 646a  dbr....r......dj
 00000a50: 616e 676f 2e64 622e 6d6f 6465 6c73 2e64  ango.db.models.d
-00000a60: 656c 6574 696f 6e72 0400 0000 7250 0000  eletionr....rP..
-00000a70: 0072 5000 0000 7250 0000 0072 5100 0000  .rP...rP...rQ...
+00000a60: 656c 6574 696f 6e72 0400 0000 724f 0000  eletionr....rO..
+00000a70: 0072 4f00 0000 724f 0000 0072 5000 0000  .rO...rO...rP...
 00000a80: da08 3c6d 6f64 756c 653e 0300 0000 7306  ..<module>....s.
 00000a90: 0000 0008 0110 0108 03                   .........
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc` & `django-paypal-plus-1.1.1/django_paypal/migrations/__pycache__/0006_auto_20240424_0727.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 24 05:27:38 2024 UTC, .py size: 755 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 4a98 2866 f302 0000  U.......J.(f....
+00000000: 550d 0d0a 0000 0000 2f19 2f66 f302 0000  U......././f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
 00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
 00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
 00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
@@ -10,44 +10,44 @@
 00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
 000000a0: 0564 0264 0365 066a 0764 0464 0564 0664  .d.d.e.j.d.d.d.d
 000000b0: 078d 0364 088d 0365 046a 0864 0264 0965  ...d...e.j.d.d.e
 000000c0: 066a 0764 0564 0a64 0b8d 0264 088d 0365  .j.d.d.d...d...e
 000000d0: 046a 0964 0264 0c68 0164 0d8d 0267 035a  .j.d.d.h.d...g.Z
 000000e0: 0a64 0e53 0029 0fda 094d 6967 7261 7469  .d.S.)...Migrati
 000000f0: 6f6e 2902 da0d 646a 616e 676f 5f70 6179  on)...django_pay
-00000100: 7061 6c5a 1730 3030 355f 6175 746f 5f32  palZ.0005_auto_2
+00000100: 7061 6cda 1730 3030 355f 6175 746f 5f32  pal..0005_auto_2
 00000110: 3032 3430 3230 375f 3036 3330 5a0d 7061  0240207_0630Z.pa
 00000120: 7970 616c 7765 6268 6f6f 6bda 0961 7574  ypalwebhook..aut
 00000130: 685f 6861 7368 da00 e9ff 0000 007a 0941  h_hash.......z.A
 00000140: 7574 6820 4861 7368 2903 da07 6465 6661  uth Hash)...defa
 00000150: 756c 74da 0a6d 6178 5f6c 656e 6774 68da  ult..max_length.
 00000160: 0c76 6572 626f 7365 5f6e 616d 6529 03da  .verbose_name)..
 00000170: 0a6d 6f64 656c 5f6e 616d 65da 046e 616d  .model_name..nam
 00000180: 65da 0566 6965 6c64 da03 7572 6cda 0355  e..field..url..U
-00000190: 524c 2902 720a 0000 0072 0b00 0000 2902  RL).r....r....).
-000001a0: 720f 0000 0072 0600 0000 2902 720d 0000  r....r....).r...
+00000190: 524c 2902 720b 0000 0072 0c00 0000 2902  RL).r....r....).
+000001a0: 7210 0000 0072 0700 0000 2902 720e 0000  r....r....).r...
 000001b0: 00da 0f75 6e69 7175 655f 746f 6765 7468  ...unique_togeth
 000001c0: 6572 4e29 0bda 085f 5f6e 616d 655f 5fda  erN)...__name__.
 000001d0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 000001e0: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
 000001f0: 6465 6e63 6965 7372 0200 0000 da08 4164  denciesr......Ad
 00000200: 6446 6965 6c64 7203 0000 00da 0943 6861  dFieldr......Cha
 00000210: 7246 6965 6c64 da0a 416c 7465 7246 6965  rField..AlterFie
 00000220: 6c64 da13 416c 7465 7255 6e69 7175 6554  ld..AlterUniqueT
 00000230: 6f67 6574 6865 72da 0a6f 7065 7261 7469  ogether..operati
-00000240: 6f6e 73a9 0072 1b00 0000 721b 0000 00fa  ons..r....r.....
+00000240: 6f6e 73a9 0072 1c00 0000 721c 0000 00fa  ons..r....r.....
 00000250: 772f 5573 6572 732f 7469 6d74 616d 2f2e  w/Users/timtam/.
 00000260: 7079 656e 762f 7665 7273 696f 6e73 2f73  pyenv/versions/s
 00000270: 662d 332e 382e 3132 2f6c 6962 2f70 7974  f-3.8.12/lib/pyt
 00000280: 686f 6e33 2e38 2f73 6974 652d 7061 636b  hon3.8/site-pack
 00000290: 6167 6573 2f64 6a61 6e67 6f5f 7061 7970  ages/django_payp
 000002a0: 616c 2f6d 6967 7261 7469 6f6e 732f 3030  al/migrations/00
 000002b0: 3036 5f61 7574 6f5f 3230 3234 3034 3234  06_auto_20240424
 000002c0: 5f30 3732 372e 7079 7204 0000 0006 0000  _0727.pyr.......
 000002d0: 0073 2200 0000 0803 02ff 0405 0401 0201  .s".............
 000002e0: 0201 0efd 0405 0401 0201 0201 0cfd 0405  ................
 000002f0: 0401 0201 04fe 04f5 7204 0000 004e 2904  ........r....N).
 00000300: da09 646a 616e 676f 2e64 6272 0200 0000  ..django.dbr....
-00000310: 7203 0000 0072 0400 0000 721b 0000 0072  r....r....r....r
-00000320: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
+00000310: 7203 0000 0072 0400 0000 721c 0000 0072  r....r....r....r
+00000320: 1c00 0000 721c 0000 0072 1d00 0000 da08  ....r....r......
 00000330: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
 00000340: 0010 03                                  ...
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/models.py` & `django-paypal-plus-1.1.1/django_paypal/models.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/ruff.toml` & `django-paypal-plus-1.1.1/django_paypal/ruff.toml`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/settings.py` & `django-paypal-plus-1.1.1/django_paypal/settings.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal/webhooks.py` & `django-paypal-plus-1.1.1/django_paypal/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class WebhookEvents:
     ORDERS = ['CHECKOUT.ORDER.COMPLETED', 'CHECKOUT.ORDER.APPROVED', 'CHECKOUT.PAYMENT-APPROVAL.REVERSED']
 
 
 def verify_and_save_webhook_event(request: HttpRequest, paypal_wrapper: PaypalWrapper, payload: Dict[str, Any]):
     if not settings.DEBUG:
-        paypal_webhook = PaypalWebhook.objects.get(url=request.build_absolute_uri())
+        paypal_webhook = PaypalWebhook.objects.get(url=request.build_absolute_uri(), auth_hash=paypal_wrapper.api_auth_hash)
         paypal_wrapper.verify_webhook_event(request, paypal_webhook.webhook_id)
         try:
             paypal_order = PaypalOrder.objects.get(order_id=payload['resource']['id'])
         except (KeyError, TypeError):  # if the payload does not contain the order id
             paypal_order = None
         event_data = {'payload': payload, 'webhook': paypal_webhook, 'order': paypal_order}
         PaypalWebhookEvent.objects.create(**event_data)
```

### Comparing `django-paypal-plus-1.1.0/django_paypal/wrappers.py` & `django-paypal-plus-1.1.1/django_paypal/wrappers.py`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/django_paypal_plus.egg-info/PKG-INFO` & `django-paypal-plus-1.1.1/django_paypal_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-paypal-plus
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django integration of PayPal's Orders v2 API
 Home-page: https://github.com/ParticulateSolutions/django-paypal-plus
 Author: Particulate Solutions GmbH
 Author-email: tech@particulate.me
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-paypal-plus-1.1.0/django_paypal_plus.egg-info/SOURCES.txt` & `django-paypal-plus-1.1.1/django_paypal_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-paypal-plus-1.1.0/setup.py` & `django-paypal-plus-1.1.1/setup.py`

 * *Files identical despite different names*

