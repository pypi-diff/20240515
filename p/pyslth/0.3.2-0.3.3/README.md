# Comparing `tmp/pyslth-0.3.2.tar.gz` & `tmp/pyslth-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.2.tar", last modified: Wed May  8 16:15:45 2024, max compression
+gzip compressed data, was "pyslth-0.3.3.tar", last modified: Wed May 15 17:37:18 2024, max compression
```

## Comparing `pyslth-0.3.2.tar` & `pyslth-0.3.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.949005 pyslth-0.3.2/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.2/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 16:15:45.948799 pyslth-0.3.2/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.917511 pyslth-0.3.2/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-08 16:15:45.000000 pyslth-0.3.2/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-08 16:15:45.000000 pyslth-0.3.2/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-08 16:15:45.000000 pyslth-0.3.2/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-08 16:15:45.000000 pyslth-0.3.2/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-08 16:15:45.000000 pyslth-0.3.2/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.2/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-08 16:15:45.949065 pyslth-0.3.2/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-08 16:15:34.000000 pyslth-0.3.2/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.924020 pyslth-0.3.2/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-05-05 12:13:46.000000 pyslth-0.3.2/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     7036 2024-05-06 09:18:10.000000 pyslth-0.3.2/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.924643 pyslth-0.3.2/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.2/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.3.2/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    22625 2024-05-08 13:37:06.000000 pyslth-0.3.2/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.3.2/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    22178 2024-05-05 11:07:40.000000 pyslth-0.3.2/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.925115 pyslth-0.3.2/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.925824 pyslth-0.3.2/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.2/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.2/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.928768 pyslth-0.3.2/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.2/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.2/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.2/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.2/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.2/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6529 2024-05-06 02:38:49.000000 pyslth-0.3.2/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.3.2/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.2/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19474 2024-05-05 01:08:32.000000 pyslth-0.3.2/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.2/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.929271 pyslth-0.3.2/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.2/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.2/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14274 2024-05-05 11:25:25.000000 pyslth-0.3.2/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.929658 pyslth-0.3.2/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.931667 pyslth-0.3.2/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.2/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.935826 pyslth-0.3.2/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.2/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.2/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.2/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.2/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1751 2024-05-08 15:54:37.000000 pyslth-0.3.2/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.2/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.2/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.938116 pyslth-0.3.2/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.2/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.2/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.2/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.2/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.2/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.947886 pyslth-0.3.2/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-08 16:07:08.000000 pyslth-0.3.2/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.2/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.2/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-08 16:07:08.000000 pyslth-0.3.2/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)    91338 2024-05-08 16:07:08.000000 pyslth-0.3.2/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.3.2/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-08 16:15:45.948491 pyslth-0.3.2/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-08 15:53:35.000000 pyslth-0.3.2/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.3.2/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.2/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.2/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.3.2/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.2/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.808873 pyslth-0.3.3/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.3/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-15 17:37:18.808606 pyslth-0.3.3/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.772220 pyslth-0.3.3/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.3/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-15 17:37:18.808940 pyslth-0.3.3/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-15 17:37:05.000000 pyslth-0.3.3/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.778876 pyslth-0.3.3/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.3/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9637 2024-05-13 08:40:08.000000 pyslth-0.3.3/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.779515 pyslth-0.3.3/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.3/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.3/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24149 2024-05-12 23:58:33.000000 pyslth-0.3.3/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.3.3/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26298 2024-05-14 12:48:00.000000 pyslth-0.3.3/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.779834 pyslth-0.3.3/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.780564 pyslth-0.3.3/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.3/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.3/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.783218 pyslth-0.3.3/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.3/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.3/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.3/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.3.3/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.3/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19846 2024-05-14 12:39:56.000000 pyslth-0.3.3/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.3/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.783760 pyslth-0.3.3/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.3/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.3/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.3/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.784086 pyslth-0.3.3/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.786029 pyslth-0.3.3/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.3/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.790325 pyslth-0.3.3/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.3/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.3/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.3/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.3/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.792484 pyslth-0.3.3/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.3/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.3/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.3/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.3/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.3/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.804614 pyslth-0.3.3/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.3/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.3/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   100211 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.806913 pyslth-0.3.3/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-08 15:53:35.000000 pyslth-0.3.3/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.3/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.3/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.3/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.3/slth/views.py
```

### Comparing `pyslth-0.3.2/PKG-INFO` & `pyslth-0.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.2
+Version: 0.3.3
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.2/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.3/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.2
+Version: 0.3.3
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.2/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.3/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/setup.py` & `pyslth-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.2/slth/__init__.py` & `pyslth-0.3.3/slth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,12 +117,12 @@
 
 def api_watchdog(sender, **kwargs):
     sender.extra_files.add(Path('application.yml'))
 
 autoreload_started.connect(api_watchdog)
 
 
-def meta(verbose_name):
+def meta(verbose_name=None):
     def decorate(function):
         function.verbose_name = verbose_name
         return function
     return decorate
```

### Comparing `pyslth-0.3.2/slth/db/models.py` & `pyslth-0.3.3/slth/db/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,24 +28,16 @@
 class ForeignKey(ForeignKey):
     def __init__(self, to, on_delete=None, **kwargs):
         self.pick = kwargs.pop('pick', False)
         self.addable = kwargs.pop('addable', False)
         super().__init__(to, on_delete or CASCADE, **kwargs)
     
     def formfield(self, *args, **kwargs):
-        field = super().formfield(*args, **kwargs)
-        return field
-
-class ManyToManyField(ManyToManyField):
-    def __init__(self, *args, **kwargs):
-        self.pick = kwargs.pop('pick', False)
-        self.addable = kwargs.pop('addable', False)
-        super().__init__(*args, **kwargs)
-
-    def formfield(self, *args, **kwargs):
+        from .. import forms
+        kwargs.update(form_class=forms.ModelChoiceField, pick=self.pick)
         field = super().formfield(*args, **kwargs)
         return field
 
 class OneToManyField(ManyToManyField):
     def __init__(self, *args, **kwargs):
         self.fields = kwargs.pop('fields', '__all__')
         super().__init__(*args, **kwargs)
@@ -67,14 +59,28 @@
         from .. import forms
         kwargs.update(form_class=forms.OneToOneField, fields=self.fields)
         field = super().formfield(*args, model=self.related_model, **kwargs)
         field.label = self.verbose_name
         field.required2 = not self.blank
         return field
 
+
+class ManyToManyField(ManyToManyField):
+    def __init__(self, *args, **kwargs):
+        self.pick = kwargs.pop('pick', False)
+        self.addable = kwargs.pop('addable', False)
+        super().__init__(*args, **kwargs)
+
+    def formfield(self, *args, **kwargs):
+        from .. import forms
+        kwargs.update(form_class=forms.ModelMultipleChoiceField, pick=self.pick)
+        field = super().formfield(*args, **kwargs)
+        return field
+
+
 class DecimalField(DecimalField):
     def __init__(self, *args, **kwargs):
         kwargs['decimal_places'] = kwargs.pop('decimal_places', 2)
         kwargs['max_digits'] = kwargs.pop('max_digits', 9)
         super().__init__(*args, **kwargs)
 
     def formfield(self, *args, **kwargs):
```

### Comparing `pyslth-0.3.2/slth/endpoints.py` & `pyslth-0.3.3/slth/endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import json
 import types
 import inspect
 from .models import Token
 from django.apps import apps
 from typing import TypeVar, Generic
 from django.core.cache import cache
@@ -13,66 +12,84 @@
 from django.views.decorators.csrf import csrf_exempt
 from .factory import FormFactory
 from django.core.exceptions import ValidationError
 from slth import forms
 from django.contrib.auth import authenticate
 from .forms import ModelForm, Form
 from .serializer import serialize, Serializer
-from .components import Application as Application_, Navbar, Menu, Footer, Response, Boxes, IconSet
+from .components import (
+    Application as Application_,
+    Navbar,
+    Menu,
+    Footer,
+    Response,
+    Boxes,
+    IconSet,
+)
 from .exceptions import JsonResponseException
 from .utils import build_url, append_url
 from .models import PushSubscription, Profile, User
 from slth.queryset import QuerySet
 from .notifications import send_push_web_notification
 from slth import APPLICATON, ENDPOINTS
 from . import oauth
 
 
 T = TypeVar("T")
 
+
 class ApiResponse(JsonResponse):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self["Access-Control-Allow-Origin"] = "*"
         self["Access-Control-Allow-Headers"] = "*"
-        self["Access-Control-Allow-Methods"] = "GET, POST, OPTIONS, PUT, DELETE, PATCH";
+        self["Access-Control-Allow-Methods"] = "GET, POST, OPTIONS, PUT, DELETE, PATCH"
         self["Access-Control-Max-Age"] = "600"
 
 
 class EnpointMetaclass(type):
     def __new__(mcs, name, bases, attrs):
         cls = super().__new__(mcs, name, bases, attrs)
         bases_names = [cls.__name__ for cls in bases]
-        if name not in ('Endpoint', 'ChildEndpoint') and '_ChildEndpoint' not in bases_names:
+        if (
+            name not in ("Endpoint", "ChildEndpoint")
+            and "_ChildEndpoint" not in bases_names
+        ):
             ENDPOINTS[cls.__name__.lower()] = cls
-        if 'AdminEndpoint' in bases_names[0:1]:
+        if "AdminEndpoint" in bases_names[0:1]:
             model = cls.__orig_bases__[0].__args__[0]
             items = (
-                ('Cadastrar', AddEndpoint[model], 'plus'),
-                ('Editar', EditEndpoint[model], 'pen'),
-                ('Visualizar', ViewEndpoint[model], 'eye'),
-                ('Excluir', DeleteEndpoint[model], 'trash')
+                ("Cadastrar", AddEndpoint[model], "plus"),
+                ("Editar", EditEndpoint[model], "pen"),
+                ("Visualizar", ViewEndpoint[model], "eye"),
+                ("Excluir", DeleteEndpoint[model], "trash"),
             )
             for prefix, base, icon in items:
-                endpoint = types.new_class(f'{prefix}{model.__name__}', (base,), {})
+                endpoint = types.new_class(f"{prefix}{model.__name__}", (base,), {})
                 endpoint.check_permission = lambda self: (
                     cls().instantiate(self.request, self).check_permission()
                 )
                 endpoint.Meta = type(
-                    'Meta', (), dict(
-                        icon=icon, modal=prefix != 'Visualizar',
-                        verbose_name=f'{prefix} {model._meta.verbose_name}'
-                    )
+                    "Meta",
+                    (),
+                    dict(
+                        icon=icon,
+                        modal=prefix != "Visualizar",
+                        verbose_name=f"{prefix} {model._meta.verbose_name}",
+                    ),
                 )
-            if 'Meta' not in attrs:
+            if "Meta" not in attrs:
                 cls.Meta = type(
-                    'Meta', (), dict(
-                        icon=getattr(model._meta, 'icon', None), modal=False,
-                        verbose_name=f'{model._meta.verbose_name_plural}'
-                    )
+                    "Meta",
+                    (),
+                    dict(
+                        icon=getattr(model._meta, "icon", None),
+                        modal=False,
+                        verbose_name=f"{model._meta.verbose_name_plural}",
+                    ),
                 )
         return cls
 
 
 class Endpoint(metaclass=EnpointMetaclass):
     cache = cache
 
@@ -90,563 +107,678 @@
 
     def contextualize(self, request):
         self.request = request
         return self
 
     def objects(self, model):
         return apps.get_model(model).objects
-        
+
     def get(self):
         return {}
-    
+
     def post(self):
-        return Response(message='Ação realizada com sucesso')
-    
+        return Response(message="Ação realizada com sucesso")
+
     def check_permission(self):
         return self.request.user.is_superuser
-    
+
     def check_role(self, *names, superuser=True):
         if self.request.user.is_superuser and superuser:
             return True
         for name in names:
-            if self.objects('slth.role').filter(username=self.request.user.username, name=name).exists():
+            if (
+                self.objects("slth.role")
+                .filter(username=self.request.user.username, name=name)
+                .exists()
+            ):
                 return True
         return False
-    
+
     def redirect(self, url):
-        raise JsonResponseException(dict(type='redirect', url=url))
-    
+        raise JsonResponseException(dict(type="redirect", url=url))
+
     def getform(self, form):
         return form
-    
+
     def process(self):
         data = self.get()
         title = self.get_verbose_name()
         if isinstance(data, models.QuerySet):
-            data = data.contextualize(self.request).settitle(title)
+            data = data.contextualize(self.request).settitle(title).apply_lookups(self.request.user)
         elif isinstance(data, Serializer):
             data = data.contextualize(self.request).settitle(title)
         elif isinstance(data, FormFactory):
             form = self.getform(data.settitle(title).form(self))
-            if self.request.method == 'POST' or self.request.GET.get('form') == title:
+            if self.request.method == "POST" or self.request.GET.get("form") == title:
                 try:
                     self.cleaned_data = form.submit()
                     return self.post()
                 except ValidationError as e:
-                    raise JsonResponseException(dict(type='error', text='\n'.join(e.messages), errors={}))
+                    raise JsonResponseException(
+                        dict(type="error", text="\n".join(e.messages), errors={})
+                    )
             else:
                 data = form
         elif isinstance(data, Form) or isinstance(data, ModelForm):
             data = data.settitle(title)
         return data
-    
+
     def serialize(self):
         return serialize(self.process())
-    
+
     def to_response(self):
         return ApiResponse(self.serialize(), safe=False)
-    
-    def formfactory(self, instance=None, method='POST') -> FormFactory:
+
+    def formfactory(self, instance=None, method="POST") -> FormFactory:
         return FormFactory(instance, method=method)
-    
+
     def serializer(self, instance=None) -> Serializer:
         return Serializer(instance or self).contextualize(self.request)
-    
+
     @classmethod
     def is_child(cls):
         return False
-    
+
     @classmethod
     def get_api_name(cls):
         return cls.__name__.lower()
-    
+
     @classmethod
     def get_api_url(cls, arg=None):
         if arg:
-            return f'/api/{cls.get_api_name()}/{arg}/'  
-        return f'/api/{cls.get_api_name()}/'    
-    
+            return f"/api/{cls.get_api_name()}/{arg}/"
+        return f"/api/{cls.get_api_name()}/"
+
     @classmethod
     def get_pretty_name(cls):
         name = []
         for c in cls.__name__:
             if name and c.isupper():
-                name.append(' ')
+                name.append(" ")
             name.append(c)
-        return ''.join(name)
-    
+        return "".join(name)
+
     @classmethod
     def get_qualified_name(cls):
-        return '{}.{}'.format(cls.__module__, cls.__name__).lower()
-    
+        return "{}.{}".format(cls.__module__, cls.__name__).lower()
+
     @classmethod
     def instantiate(cls, request, source):
         args = ()
         if cls.is_child():
             args = (source,) if cls.has_args() else ()
         else:
             args = (source.pk,) if cls.has_args() else ()
         return cls(*args).configure(source).contextualize(request)
-    
+
     @classmethod
     def has_args(cls):
         return len(inspect.getfullargspec(cls.__init__).args) > 1
-    
+
     @classmethod
     def get_api_url_pattern(cls):
         args = inspect.getfullargspec(cls.__init__).args[1:]
-        pattern = '{}/'.format(cls.get_api_name())
+        pattern = "{}/".format(cls.get_api_name())
         for arg in args:
-            pattern = '{}{}/'.format(pattern, '<int:{}>'.format(arg))
+            pattern = "{}{}/".format(pattern, "<int:{}>".format(arg))
         return pattern
-    
+
     @classmethod
     def get_api_metadata(cls, request, base_url, pk=None):
-        action_name = cls.get_metadata('verbose_name')
-        icon = cls.get_metadata('icon')
-        modal = cls.get_metadata('modal')
+        action_name = cls.get_metadata("verbose_name")
+        icon = cls.get_metadata("icon")
+        modal = cls.get_metadata("modal")
         if cls.is_child():
-            url = append_url(base_url, f'action={cls.get_api_name()}')
-            url = f'{url}&id={pk}' if pk else url
+            url = append_url(base_url, f"action={cls.get_api_name()}")
+            url = f"{url}&id={pk}" if pk else url
         else:
-            url = build_url(request, f'/api/{cls.get_api_name()}/')
-            url = f'{url}{pk}/' if pk else url
-        return dict(type='action', title=action_name, name=action_name, url=url, key=cls.get_api_name(), icon=icon, modal=modal)
-    
+            url = build_url(request, f"/api/{cls.get_api_name()}/")
+            url = f"{url}{pk}/" if pk else url
+        return dict(
+            type="action",
+            title=action_name,
+            name=action_name,
+            url=url,
+            key=cls.get_api_name(),
+            icon=icon,
+            modal=modal,
+        )
+
     @classmethod
     def get_metadata(cls, key, default=None):
         value = None
-        metaclass = getattr(cls, 'Meta', None)
+        metaclass = getattr(cls, "Meta", None)
         if metaclass:
             value = getattr(metaclass, key, None)
         if value is None:
-            if key == 'verbose_name':
+            if key == "verbose_name":
                 value = cls.get_pretty_name()
-            if key == 'modal':
-                value = issubclass(cls, EditEndpoint) or issubclass(cls, DeleteEndpoint) or issubclass(cls, Endpoint) or issubclass(cls, ChildEndpoint)
+            if key == "modal":
+                value = (
+                    issubclass(cls, EditEndpoint)
+                    or issubclass(cls, DeleteEndpoint)
+                    or issubclass(cls, Endpoint)
+                    or issubclass(cls, ChildEndpoint)
+                )
         return default if value is None else value
-    
+
     def get_verbose_name(self):
-        return self.get_metadata('verbose_name')
+        return self.get_metadata("verbose_name")
+
 
 class PublicEndpoint(Endpoint):
     def check_permission(self):
         return True
 
+
 class ModelEndpoint(Endpoint):
     def __init__(self):
         self.model = self.__orig_bases__[0].__args__[0]
         if isinstance(self.model, str):
             self.model = self.objects(self.model).get(pk=self.pk)
         super().__init__()
 
+
 class AdminEndpoint(Generic[T], ModelEndpoint):
 
     def get(self) -> QuerySet:
-        actions = [f'{prefix}{self.model.__name__.lower()}' for prefix in ('cadastrar', 'visualizar', 'editar', 'excluir')]
+        actions = [
+            f"{prefix}{self.model.__name__.lower()}"
+            for prefix in ("cadastrar", "visualizar", "editar", "excluir")
+        ]
         return self.model.objects.all().actions(*actions)
-    
+
+
 class ListEndpoint(Generic[T], ModelEndpoint):
     def get(self) -> QuerySet:
-        return self.model.objects
+        return self.model.objects.contextualize(self.request)
+
 
 class AddEndpoint(Generic[T], ModelEndpoint):
     def __init__(self):
         super().__init__()
         self.instance = self.model()
 
     def get(self) -> FormFactory:
         return self.model().formfactory()
-    
+
     def get_instance(self):
         return self.instance
 
+
 class ModelInstanceEndpoint(ModelEndpoint):
     def __init__(self, pk):
         super().__init__()
         self.instance = self.model.objects.get(pk=pk)
 
     def get_instance(self):
         return self.instance
 
+
 class InstanceEndpoint(Generic[T], ModelInstanceEndpoint):
 
     def formfactory(self) -> FormFactory:
         return FormFactory(self.get_instance())
 
     def serializer(self) -> Serializer:
         return Serializer(self.get_instance()).contextualize(self.request)
-    
+
 
 class ViewEndpoint(Generic[T], ModelInstanceEndpoint):
 
     class Meta:
-        icon = 'eye'
+        icon = "eye"
         modal = False
-        verbose_name = 'Visualizar'
+        verbose_name = "Visualizar"
 
     def get(self) -> Serializer:
         return self.get_instance().serializer().contextualize(self.request)
-    
+
     def get_verbose_name(self):
         return str(self.get_instance())
-        
+
+
 class EditEndpoint(Generic[T], ModelInstanceEndpoint):
     def get(self) -> FormFactory:
         return self.get_instance().formfactory()
-    
+
+
 class DeleteEndpoint(Generic[T], ModelInstanceEndpoint):
     def get(self) -> FormFactory:
         return self.formfactory(self.get_instance()).fields()
-    
+
     def post(self):
         self.get_instance().delete()
         return super().post()
 
-    
+
 class ChildEndpoint(Endpoint):
 
     @classmethod
     def is_child(cls):
         return True
-    
+
     def check_permission(self):
         return True
 
+
 class Add(ChildEndpoint):
     class Meta:
-        icon = 'plus'
-        verbose_name = 'Cadastrar'
+        icon = "plus"
+        verbose_name = "Cadastrar"
 
     def get(self) -> FormFactory:
         return self.source.model().formfactory()
-    
+
+
 class ChildInstanceEndpoint(ChildEndpoint):
     def __init__(self, instance):
         self.instance = instance
         super().__init__()
 
     def get_instance(self):
         return self.instance
-    
+
     def formfactory(self) -> FormFactory:
         return FormFactory(self.get_instance())
-    
+
     def serializer(self) -> Serializer:
         return Serializer(self.get_instance()).contextualize(self.request)
-    
+
+
 class View(ChildInstanceEndpoint):
     class Meta:
-        icon = 'eye'
+        icon = "eye"
         modal = False
-        verbose_name = 'Visualizar'
-    
+        verbose_name = "Visualizar"
+
     def get(self) -> Serializer:
         return self.get_instance().serializer()
 
+
 class Edit(ChildInstanceEndpoint):
     class Meta:
-        icon = 'pen'
-        verbose_name = 'Editar'
+        icon = "pen"
+        verbose_name = "Editar"
+
     def get(self) -> FormFactory:
         return self.get_instance().formfactory()
-   
+
+
 class Delete(ChildInstanceEndpoint):
     class Meta:
-        icon = 'trash'
-        verbose_name = 'Excluir'
-    
+        icon = "trash"
+        verbose_name = "Excluir"
+
     def get(self):
         return self.formfactory().fields()
-    
+
     def post(self):
         self.get_instance().delete()
         return super().post()
 
+
 class Login(PublicEndpoint):
-    username = forms.CharField(label='Username')
-    password = forms.CharField(label='Senha')
+    username = forms.CharField(label="Username")
+    password = forms.CharField(label="Senha")
 
     class Meta:
         modal = False
-        icon = 'sign-in'
-        verbose_name = 'Login'
+        icon = "sign-in"
+        verbose_name = "Login"
 
     def get(self):
-        code = self.request.GET.get('code')
+        code = self.request.GET.get("code")
         if code:
             user = oauth.authenticate(code)
             if user:
                 token = Token.objects.create(user=user)
-                return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=token.key, application=None))
-        return self.formfactory().fields('username', 'password')
-    
+                return Response(
+                    message="Bem-vindo!",
+                    redirect="/api/dashboard/",
+                    store=dict(token=token.key, application=None),
+                )
+        return self.formfactory().fields("username", "password")
+
     def post(self):
-        user = authenticate(self.request, username=self.cleaned_data.get('username'), password=self.cleaned_data.get('password'))
+        user = authenticate(
+            self.request,
+            username=self.cleaned_data.get("username"),
+            password=self.cleaned_data.get("password"),
+        )
         if user:
             token = Token.objects.create(user=user)
-            return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=token.key, application=None))
+            return Response(
+                message="Bem-vindo!",
+                redirect="/api/dashboard/",
+                store=dict(token=token.key, application=None),
+            )
         else:
-            raise ValidationError('Login e senha não conferem')
+            raise ValidationError("Login e senha não conferem")
+
 
 class Logout(Endpoint):
     class Meta:
         modal = False
-        verbose_name = 'Sair'
-        
+        verbose_name = "Sair"
+
     def get(self):
-        return Response(message='Logout realizado com sucesso.', redirect='/api/home/', store=dict(token=None, application=None))
+        return Response(
+            message="Logout realizado com sucesso.",
+            redirect="/api/home/",
+            store=dict(token=None, application=None),
+        )
 
     def check_permission(self):
         return self.request.user.is_authenticated
 
+
 class Icons(PublicEndpoint):
     class Meta:
         modal = True
-        verbose_name = 'Icons'
+        verbose_name = "Icons"
 
     def get(self):
         return IconSet()
-    
+
     def check_permission(self):
         return settings.DEBUG
 
 
 class Search(Endpoint):
     def get(self):
-        key = '_options_'
+        key = "_options_"
         options = self.cache.get(key, [])
-        term = self.request.GET.get('term')
-        if options is None and APPLICATON['dashboard']['search']:
+        term = self.request.GET.get("term")
+        if options is None and APPLICATON["dashboard"]["search"]:
             options = []
-            for endpoint in APPLICATON['dashboard']['search']:
+            for endpoint in APPLICATON["dashboard"]["search"]:
                 cls = ENDPOINTS[endpoint]
                 url = build_url(self.request, cls.get_api_url())
-                verbose_name = cls.get_metadata('verbose_name')
+                verbose_name = cls.get_metadata("verbose_name")
                 options.append(dict(id=url, value=verbose_name))
             self.cache.set(key, options)
         if term:
             result = []
             for option in options:
-                if slugify(term.lower()) in slugify(option['value'].lower()):
+                if slugify(term.lower()) in slugify(option["value"].lower()):
                     result.append(option)
         else:
             result = options
         return result[0:10]
-    
+
+
 class Users(ListEndpoint[User]):
 
     class Meta:
         modal = False
-        verbose_name = 'Usuários'
+        verbose_name = "Usuários"
 
     def get(self):
         return (
-            super().get().search('username', 'email')
-            .filters('is_superuser', 'is_active')
-            .fields('username', 'email', 'get_roles')
-            .actions('add', 'view', 'edit', 'delete', 'sendpushnotification', 'changepassword')
+            super()
+            .get()
+            .search("username", "email")
+            .filters("is_superuser", "is_active")
+            .fields("username", "email", "get_roles")
+            .actions(
+                "add",
+                "viewuser",
+                "edit",
+                "delete",
+                "sendpushnotification",
+                "changepassword",
+            )
         )
-    
+
+class ViewUser(ViewEndpoint[User]):
+    class Meta:
+        modal = False
+        icon = 'eye'
+        verbose_name = 'Visualizar '
+
+    def get(self):
+        return (
+            super().get()
+        )
+
+
 class ChangePassword(ChildInstanceEndpoint):
-    password = forms.CharField(label='Senha', required=False)
+    password = forms.CharField(label="Senha", required=False)
 
     class Meta:
-        icon = 'user-lock'
-        verbose_name = 'Alterar Senha'
+        icon = "user-lock"
+        verbose_name = "Alterar Senha"
 
     def get(self):
-        return self.formfactory().fields('password')
+        return self.formfactory().fields("password")
 
     def post(self):
-        self.instance.set_password(self.cleaned_data['password'])
+        self.instance.set_password(self.cleaned_data["password"])
         self.instance.save()
         return super().post()
 
+
 class Home(PublicEndpoint):
     class Meta:
-        verbose_name = ''
+        verbose_name = ""
 
     def get(self):
-        cls = ENDPOINTS[APPLICATON['index']]
+        cls = ENDPOINTS[APPLICATON["index"]]
         self.redirect(cls.get_api_url())
 
 
 class Dashboard(Endpoint):
     class Meta:
-        verbose_name = ''
-        
+        verbose_name = ""
+
     def get(self):
         if self.request.user.is_authenticated:
             serializer = Serializer(request=self.request)
-            if APPLICATON['dashboard']['boxes']:
-                boxes = Boxes('Acesso Rápido')
-                for endpoint in APPLICATON['dashboard']['boxes']:
+            if APPLICATON["dashboard"]["boxes"]:
+                boxes = Boxes("Acesso Rápido")
+                for endpoint in APPLICATON["dashboard"]["boxes"]:
                     cls = ENDPOINTS[endpoint]
                     if cls().contextualize(self.request).check_permission():
-                        icon = cls.get_metadata('icon', 'check')
-                        label = cls.get_metadata('verbose_name')
+                        icon = cls.get_metadata("icon", "check")
+                        label = cls.get_metadata("verbose_name")
                         url = build_url(self.request, cls.get_api_url())
                         boxes.append(icon, label, url)
-                serializer.append('Acesso Rápido', boxes)
-            if APPLICATON['dashboard']['top']:
-                group = serializer.group('Top')
-                for endpoint in APPLICATON['dashboard']['top']:
+                serializer.append("Acesso Rápido", boxes)
+            if APPLICATON["dashboard"]["top"]:
+                group = serializer.group("Top")
+                for endpoint in APPLICATON["dashboard"]["top"]:
                     cls = ENDPOINTS[endpoint]
-                    if cls.instantiate(self.request, self.request.user).check_permission():
-                        group.endpoint(cls.get_metadata('verbose_name'), cls, wrap=False)
+                    if cls.instantiate(
+                        self.request, self.request.user
+                    ).check_permission():
+                        group.endpoint(
+                            cls.get_metadata("verbose_name"), cls, wrap=False
+                        )
                 group.parent()
-            if APPLICATON['dashboard']['center']:
-                for endpoint in APPLICATON['dashboard']['center']:
+            if APPLICATON["dashboard"]["center"]:
+                for endpoint in APPLICATON["dashboard"]["center"]:
                     cls = ENDPOINTS[endpoint]
-                    serializer.endpoint(cls.get_metadata('verbose_name'), cls, wrap=False)
+                    serializer.endpoint(
+                        cls.get_metadata("verbose_name"), cls, wrap=False
+                    )
             return serializer
         else:
-            self.redirect('/api/login/')
+            self.redirect("/api/login/")
 
     def check_permission(self):
         return self.request.user.is_authenticated
-    
+
+
 class Application(PublicEndpoint):
     def get(self):
         user = None
         navbar = None
         menu = None
-        icon = build_url(self.request, APPLICATON['logo'])
-        logo = build_url(self.request, APPLICATON['logo'])
+        icon = build_url(self.request, APPLICATON["logo"])
+        logo = build_url(self.request, APPLICATON["logo"])
         if self.request.user.is_authenticated:
-            user = self.request.user.username.split()[0].split('@')[0]
+            user = self.request.user.username.split()[0].split("@")[0]
         navbar = Navbar(
-            title=APPLICATON['title'], subtitle=APPLICATON['subtitle'],
-            logo=logo, user=user
+            title=APPLICATON["title"],
+            subtitle=APPLICATON["subtitle"],
+            logo=logo,
+            user=user,
         )
-        for entrypoint in ['actions', 'usermenu', 'adder', 'settings', 'tools']:
-            if APPLICATON['dashboard'][entrypoint]:
-                for endpoint in APPLICATON['dashboard'][entrypoint]:
+        for entrypoint in ["actions", "usermenu", "adder", "settings", "tools", "toolbar"]:
+            if APPLICATON["dashboard"][entrypoint]:
+                for endpoint in APPLICATON["dashboard"][entrypoint]:
                     cls = ENDPOINTS[endpoint]
                     if cls().instantiate(self.request, self).check_permission():
-                        label = cls.get_metadata('verbose_name')
+                        label = cls.get_metadata("verbose_name")
                         url = build_url(self.request, cls.get_api_url())
-                        modal = cls.get_metadata('modal', False)
-                        icon = cls.get_metadata('icon', None)
+                        modal = cls.get_metadata("modal", False)
+                        icon = cls.get_metadata("icon", None)
                         navbar.add_action(entrypoint, label, url, modal, icon=icon)
-        if APPLICATON['menu']:
+        if APPLICATON["menu"]:
             items = []
+
             def get_item(k, v):
                 if isinstance(v, dict):
-                    icon, label = k.split(':') if ':' in k else (None, k)
+                    icon, label = k.split(":") if ":" in k else (None, k)
                     subitems = []
                     for k1, v1 in v.items():
                         subitem = get_item(k1, v1)
                         if subitem:
                             subitems.append(subitem)
                     if subitems:
                         return dict(dict(icon=icon, label=label, items=subitems))
                 else:
                     cls = ENDPOINTS.get(v)
                     if cls:
                         if cls().instantiate(self.request, self).check_permission():
-                            icon, label = k.split(':') if ':' in k else (None, k)
+                            icon, label = k.split(":") if ":" in k else (None, k)
                             url = build_url(self.request, cls.get_api_url())
                             return dict(dict(label=label, url=url, icon=icon))
                     else:
                         print(v)
-            for k, v in APPLICATON['menu'].items():
+
+            for k, v in APPLICATON["menu"].items():
                 item = get_item(k, v)
                 if item:
                     items.append(item)
-            profile = Profile.objects.filter(user=self.request.user).first() if user else None
-            photo_url = profile.photo.url if profile and profile.photo else '/static/images/user.svg'
+            profile = (
+                Profile.objects.filter(user=self.request.user).first() if user else None
+            )
+            photo_url = (
+                profile.photo.url
+                if profile and profile.photo
+                else "/static/images/user.svg"
+            )
             menu = Menu(items, user=user, image=build_url(self.request, photo_url))
 
-        footer = Footer(APPLICATON['version'])
-        return Application_(icon=icon, navbar=navbar, menu=menu, footer=footer, oauth=oauth.providers())
-    
+        footer = Footer(APPLICATON["version"])
+        return Application_(
+            icon=icon, navbar=navbar, menu=menu, footer=footer, oauth=oauth.providers(),
+            sponsors=APPLICATON.get("sponsors", ())
+        )
+
+
 class Manifest(PublicEndpoint):
 
     class Meta:
-        verbose_name = 'Manifest'
+        verbose_name = "Manifest"
 
     def get(self):
         return dict(
             {
-                "name": APPLICATON['title'],
-                "short_name": APPLICATON['title'],
-                "lang": 'pt-BR',
+                "name": APPLICATON["title"],
+                "short_name": APPLICATON["title"],
+                "lang": "pt-BR",
                 "start_url": build_url(self.request, "/app/home/"),
                 "scope": build_url(self.request, "/app/"),
                 "display": "standalone",
-                "icons": [{
-                    "src": build_url(self.request, APPLICATON['logo']),
-                    "sizes": "192x192",
-                    "type": "image/png"
-                }]
+                "icons": [
+                    {
+                        "src": build_url(self.request, APPLICATON["logo"]),
+                        "sizes": "192x192",
+                        "type": "image/png",
+                    }
+                ],
             }
         )
 
     def check_permission(self):
         return True
 
 
 class PushSubscribe(Endpoint):
 
     class Meta:
-        verbose_name = 'Subscrever para Notificações'
+        verbose_name = "Subscrever para Notificações"
 
     def post(self):
-        data = json.loads(self.request.POST.get('subscription'))
-        device = self.request.META.get('HTTP_USER_AGENT', '')
+        data = json.loads(self.request.POST.get("subscription"))
+        device = self.request.META.get("HTTP_USER_AGENT", "")
         qs = PushSubscription.objects.filter(user=User.objects.first(), device=device)
-        qs.update(data=data) if qs.exists() else PushSubscription.objects.create(
-            user=User.objects.first(), data=data, device=device
+        (
+            qs.update(data=data)
+            if qs.exists()
+            else PushSubscription.objects.create(
+                user=User.objects.first(), data=data, device=device
+            )
         )
         return Response()
 
     def check_permission(self):
         return True
-    
+
+
 class PushSubscriptions(ListEndpoint[PushSubscription]):
     class Meta:
-        verbose_name = 'Notificações'
+        verbose_name = "Notificações"
+
 
 class SendPushNotification(ChildInstanceEndpoint):
-    message = forms.CharField(label='Texto', widget=forms.Textarea())
+    message = forms.CharField(label="Texto", widget=forms.Textarea())
+
     class Meta:
-        icon = 'mail-bulk'
-        verbose_name = 'Enviar Notificação'
+        icon = "mail-bulk"
+        verbose_name = "Enviar Notificação"
 
     def get(self):
-        return self.formfactory().fields('message')
+        return self.formfactory().fields("message")
 
     def post(self):
-        send_push_web_notification(self.instance, self.cleaned_data['message'])
-        return Response(message='Notificação enviada com sucesso.')
+        send_push_web_notification(self.instance, self.cleaned_data["message"])
+        return Response(message="Notificação enviada com sucesso.")
+
 
 class EditProfile(Endpoint):
-    password = forms.CharField(label='Senha', required=False)
-    password2 = forms.CharField(label='Confirmação', required=False)
+    password = forms.CharField(label="Senha", required=False)
+    password2 = forms.CharField(label="Confirmação", required=False)
 
     class Meta:
-        verbose_name = 'Editar Perfil'
+        verbose_name = "Editar Perfil"
 
     def __init__(self, *args, **kwargs):
         self.instance = None
         super().__init__(*args, **kwargs)
-       
+
     def get(self):
-        self.instance = Profile.objects.filter(user=self.request.user).first() or Profile(user=self.request.user)
+        self.instance = Profile.objects.filter(
+            user=self.request.user
+        ).first() or Profile(user=self.request.user)
         return (
             self.formfactory(self.instance)
-            .fieldset('Dados Gerais', ('photo',))
-            .fieldset('Dados de Acesso', (('password', 'password2'),))
+            .fieldset("Dados Gerais", ("photo",))
+            .fieldset("Dados de Acesso", (("password", "password2"),))
         )
-    
+
     def post(self):
         self.instance.save()
-        if self.cleaned_data.get('password'):
-            self.instance.user.set_password(self.cleaned_data.get('password'))
+        if self.cleaned_data.get("password"):
+            self.instance.user.set_password(self.cleaned_data.get("password"))
             self.instance.user.save()
-        return Response(message='Ação realizada com sucesso.', redirect='/api/dashboard/', store=dict(application=None))
+        return Response(
+            message="Ação realizada com sucesso.",
+            redirect="/api/dashboard/",
+            store=dict(application=None),
+        )
 
     def check_permission(self):
         return self.request.user.is_authenticated
-
```

### Comparing `pyslth-0.3.2/slth/factory.py` & `pyslth-0.3.3/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/forms.py` & `pyslth-0.3.3/slth/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,387 +1,524 @@
-
 import json
 from typing import Any
 import datetime
 from django.forms import *
 from django.utils.translation import gettext_lazy as _
 from django.forms.models import ModelChoiceIterator, ModelMultipleChoiceField
 from django.db.models import Model, QuerySet, Manager
 from .models import Token, Profile
 from django.db import transaction
 from django.db.models import Manager
 from .exceptions import JsonResponseException
 from .utils import absolute_url, build_url
 from .serializer import Serializer
 from slth import ENDPOINTS
+from .components import Scheduler
 
 
 DjangoModelForm = ModelForm
 DjangoForm = Form
 DjangoModelChoiceField = ModelChoiceField
 DjangoMultipleChoiceField = MultipleChoiceField
 DjangoModelMultipleChoiceField = ModelMultipleChoiceField
 DjangoFileField = FileField
 DjangoImageField = ImageField
 
 MASKS = dict(
-    cpf_cnpj='999.999.999-99|99.999.999/9999-99',
-    cpf='999.999.999-99',
-    cnpj='99.999.999/9999-99',
-    telefone='(99) 99999-9999',
+    cpf_cnpj="999.999.999-99|99.999.999/9999-99",
+    cpf="999.999.999-99",
+    cnpj="99.999.999/9999-99",
+    telefone="(99) 99999-9999",
 )
 
+
 class FormController:
 
     def __init__(self, form):
         super().__init__()
         self.form = form
-        self.controls = dict(hide=[], show=[], set={})
-    
+        self.controls = dict(hide=[], show=[], reload=[], set={})
+
     def hide(self, *names):
-        self.controls['hide'].extend(names)
+        self.controls["hide"].extend(names)
 
     def show(self, *names):
-        self.controls['show'].extend(names)
+        self.controls["show"].extend(names)
+
+    def reload(self, *names):
+        self.controls["reload"].extend(names)
 
     def set(self, **kwargs):
         for k, v in kwargs.items():
             if isinstance(v, Model):
                 v = dict(id=v.id, value=str(v))
             elif isinstance(v, QuerySet) or isinstance(v, Manager):
                 v = [dict(id=v.id, value=str(v)) for v in v]
             elif isinstance(v, bool):
                 v = str(v).lower()
             elif isinstance(v, datetime.datetime):
-                v = v.strftime('%Y-%m-%d %H:%M')
+                v = v.strftime("%Y-%m-%d %H:%M")
             elif isinstance(v, datetime.date):
-                v = v.strftime('%Y-%m-%d')
-            self.controls['set'][k] = v
+                v = v.strftime("%Y-%m-%d")
+            self.controls["set"][k] = v
 
     def get(self, name, value, default=None):
         if value is None:
             return default
         else:
             try:
                 value = self.form.fields[name].to_python(value)
             except KeyError:
                 pass
             except ValidationError:
                 pass
             return default if value is None else value
-        
+
     def clear(self):
-        self.controls['show'].clear()
-        self.controls['hide'].clear()
-        self.controls['set'].clear()
+        self.controls["show"].clear()
+        self.controls["hide"].clear()
+        self.controls["set"].clear()
 
     def on_change(self, field_name):
         self.clear()
-        getattr(self.form._endpoint, f'on_{field_name}_change')(self, self.values())
+        getattr(self.form._endpoint, f"on_{field_name}_change")(self, self.values())
         return self.controls
-    
+
+
     def get_field_queryset(self, fname, qs):
         method_attr = None
-        method_name = f'get_{fname}_queryset'
+        method_name = f"get_{fname}_queryset"
         if hasattr(self.form._endpoint, method_name):
             method_attr = getattr(self.form._endpoint, method_name)
-        elif hasattr(self.form, 'instance') and hasattr(self.form.instance, method_name):
+        elif hasattr(self.form, "instance") and hasattr(
+            self.form.instance, method_name
+        ):
             method_attr = getattr(self.form.instance, method_name)
+        return method_attr(qs, self.values()) if method_attr else qs
 
-        if method_attr:
-            qs = method_attr(qs, self.values())
-        return qs
-    
     def values(self):
-        data = dict(**self.controls['set'])
+        data = dict(**self.controls["set"])
         for name in self.form.fields:
             value = self.get(name, self.form.request.GET.get(name))
             if value:
                 data[name] = value
         return data
 
+
 class FormMixin:
 
     def fieldset(self, title, fields):
         self.fieldsets[title] = fields
         return self
 
     def parse_json(self):
-        content_type = self.request.META.get('CONTENT_TYPE')
+        content_type = self.request.META.get("CONTENT_TYPE")
         method = self.request.method.lower()
-        if content_type and content_type.lower() in 'application/json':
-            if method == 'get' or method == 'post':
+        if content_type and content_type.lower() in "application/json":
+            if method == "get" or method == "post":
                 d1 = json.loads(self.request.body.decode()) if self.request.body else {}
-                d2 = self.request.GET if method == 'get' else self.request.POST
+                d2 = self.request.GET if method == "get" else self.request.POST
                 d2._mutable = True
                 d2.clear()
                 for k, v in d1.items():
                     if isinstance(v, list):
                         for i, item in enumerate(v):
-                            prefix = f'{k}__{i}'
-                            d2[f'{prefix}__id'] = item.get('id')
+                            prefix = f"{k}__{i}"
+                            d2[f"{prefix}__id"] = item.get("id")
                             for k1, v1 in item.items():
-                                d2[f'{prefix}__{k1}'] = v1
+                                d2[f"{prefix}__{k1}"] = v1
                     elif isinstance(v, dict):
                         prefix = k
-                        d2[f'{prefix}__id'] = v.get('id')
+                        d2[f"{prefix}__id"] = v.get("id")
                         for k1, v1 in v.items():
-                            d2[f'{prefix}__{k1}'] = v1
+                            d2[f"{prefix}__{k1}"] = v1
                     else:
                         d2[k] = v
                 d2._mutable = False
 
     @classmethod
     def get_metadata(cls, name, default=None):
-        metaclass = getattr(cls, 'Meta', None)
+        metaclass = getattr(cls, "Meta", None)
         return getattr(metaclass, name, default) if metaclass else default
 
     def serialize(self):
         return self.to_dict()
-        
+
     def display(self, serializable):
         self._display = serializable
         return self
 
     def to_dict(self, prefix=None):
-        field_name = self.request.GET.get('on_change')
+        field_name = self.request.GET.get("on_change")
         if field_name:
             raise JsonResponseException(self.controller.on_change(field_name))
-        
+
         data = dict(
-            type='form', key=self._key, method=self._method, title=self.get_metadata('title', self._title), icon=self.get_metadata('icon'),
-            style=self.get_metadata('style'), url=absolute_url(self.request), info=self._info
+            type="form",
+            key=self._key,
+            method=self._method,
+            title=self.get_metadata("title", self._title),
+            icon=self.get_metadata("icon"),
+            style=self.get_metadata("style"),
+            url=absolute_url(self.request),
+            info=self._info,
+        )
+        data.update(
+            controls=self.controller.controls, width=self.get_metadata("width", "100%")
         )
-        data.update(controls=self.controller.controls, width=self.get_metadata('width', '100%'))
         if self._display:
             if isinstance(self._display, Serializer):
                 # self._display.request = self.request
-                data.update(display=self._display.serialize(forward_exception=True)['data'])
-        choices_field_name = self.request.GET.get('choices')
+                data.update(
+                    display=self._display.serialize(forward_exception=True)["data"]
+                )
+        choices_field_name = self.request.GET.get("choices")
         if self.fieldsets:
             fieldsetlist = []
             for title, names in self.fieldsets.items():
                 fields = []
                 if prefix:
-                    value = self.instance.pk if isinstance(self, ModelForm) else ''
-                    fields.append([dict(type='hidden', name=f'{prefix}__id', value=value, label='ID')])
+                    value = self.instance.pk if isinstance(self, ModelForm) else ""
+                    fields.append(
+                        [
+                            dict(
+                                type="hidden",
+                                name=f"{prefix}__id",
+                                value=value,
+                                label="ID",
+                            )
+                        ]
+                    )
                 for name in names:
                     if isinstance(name, str):
-                        field = self.serialize_field(name, self.fields[name], prefix, choices_field_name)
+                        field = self.serialize_field(
+                            name, self.fields[name], prefix, choices_field_name
+                        )
                         fields.append([field])
                     else:
                         fields.append(
-                            [self.serialize_field(name, self.fields[name], prefix, choices_field_name) for name in name]
+                            [
+                                self.serialize_field(
+                                    name, self.fields[name], prefix, choices_field_name
+                                )
+                                for name in name
+                            ]
                         )
-                if len(fields)==1 and isinstance(fields[0], list) and fields[0][0]['type'] == 'inline':
+                if (
+                    len(fields) == 1
+                    and isinstance(fields[0], list)
+                    and fields[0][0]["type"] == "inline"
+                ):
                     fieldsetlist.append(fields[0][0])
                 else:
-                    fieldsetlist.append(dict(type='fieldset', title=title, fields=fields))
+                    fieldsetlist.append(
+                        dict(type="fieldset", title=title, fields=fields)
+                    )
             data.update(fieldsets=fieldsetlist)
         else:
             fields = []
             if prefix:
-                value = self.instance.pk if isinstance(self, ModelForm) else ''
-                fields.append(dict(type='hidden', name=f'{prefix}__id', value=value, label='ID'))
+                value = self.instance.pk if isinstance(self, ModelForm) else ""
+                fields.append(
+                    dict(type="hidden", name=f"{prefix}__id", value=value, label="ID")
+                )
             for name, field in self.fields.items():
-                fields.append(self.serialize_field(name, field, prefix, choices_field_name))
+                fields.append(
+                    self.serialize_field(name, field, prefix, choices_field_name)
+                )
             data.update(fields=fields)
         return data
-    
+
     def serialize_field(self, name, field, prefix, choices_field_name):
         if isinstance(field, InlineFormField) or isinstance(field, InlineModelField):
             value = []
             instances = []
             is_one_to_one = field.max == field.min == 1
             if isinstance(self, ModelForm):
                 if isinstance(field, OneToOneField):
-                    instances.append(getattr(self.instance, name) if self.instance.id else None)
+                    instances.append(
+                        getattr(self.instance, name) if self.instance.id else None
+                    )
                 elif isinstance(field, OneToManyField):
-                    instances.extend(getattr(self.instance, name).all() if self.instance.id else ())
+                    instances.extend(
+                        getattr(self.instance, name).all() if self.instance.id else ()
+                    )
             for i, instance in enumerate(instances):
-                prefix = name if is_one_to_one else f'{name}__{i}'
-                kwargs = dict(instance=instance, request=self.request) if isinstance(field, InlineModelField) else dict(endpoint=self._endpoint)
+                prefix = name if is_one_to_one else f"{name}__{i}"
+                kwargs = (
+                    dict(instance=instance, endpoint=self._endpoint)
+                    if isinstance(field, InlineModelField)
+                    else dict(endpoint=self._endpoint)
+                )
                 value.append(field.form(**kwargs).to_dict(prefix=prefix))
             if not is_one_to_one:
-                value.append(field.form(endpoint=self._endpoint).to_dict(prefix=f'{name}__n'))
-            required = getattr(field, 'required2', field.required)
+                value.append(
+                    field.form(endpoint=self._endpoint).to_dict(prefix=f"{name}__n")
+                )
+            required = getattr(field, "required2", field.required)
             label = field.label.title() if field.label else field.label
-            data = dict(type='inline', min=field.min, max=field.max, name=name, count=len(instances), label=label, required=required, value=value)
+            data = dict(
+                type="inline",
+                min=field.min,
+                max=field.max,
+                name=name,
+                count=len(instances),
+                label=label,
+                required=required,
+                value=value,
+            )
         else:
             extra = {}
-            ftype = FIELD_TYPES.get(type(field).__name__, 'text')
+            ftype = FIELD_TYPES.get(type(field).__name__, "text")
             if name in self._values:
-                ftype = 'hidden'
+                ftype = "hidden"
                 value = self._values[name]
                 value = value.pk if isinstance(value, Model) else value
             else:
                 value = field.initial or self.initial.get(name)
                 if callable(value):
                     value = value()
-                
-                if isinstance(field, ModelMultipleChoiceField) or isinstance(field, DjangoModelMultipleChoiceField):
-                    value = [dict(id=obj.id, label=str(obj)) for obj in value] if value else []
-                elif isinstance(field, MultipleChoiceField) or isinstance(field,DjangoMultipleChoiceField):
+
+                if isinstance(field, ModelMultipleChoiceField) or isinstance(
+                    field, DjangoModelMultipleChoiceField
+                ):
+                    value = (
+                        [dict(id=obj.id, label=str(obj).strip()) for obj in value]
+                        if value
+                        else []
+                    )
+                elif isinstance(field, MultipleChoiceField) or isinstance(
+                    field, DjangoMultipleChoiceField
+                ):
                     value = value if value else []
-                elif value and (isinstance(field, ModelChoiceField) or isinstance(field, DjangoModelChoiceField)):
+                elif value and (
+                    isinstance(field, ModelChoiceField)
+                    or isinstance(field, DjangoModelChoiceField)
+                ):
                     obj = field.queryset.get(pk=value)
-                    value = dict(id=obj.id, label=str(obj))
+                    value = dict(id=obj.id, label=str(obj).strip())
                 elif isinstance(field, DjangoImageField):
                     value = build_url(self.request, value.url) if value else None
-                    extra.update(extensions=field.extensions, width=field.width, height=field.height)
+                    extra.update(
+                        extensions=field.extensions,
+                        width=field.width,
+                        height=field.height,
+                    )
                 elif isinstance(field, DjangoFileField):
                     value = build_url(self.request, value.url) if value else None
                     extra.update(extensions=field.extensions, max_size=field.max_size)
-            
+
             if isinstance(field.widget, HiddenInput):
-                ftype = 'hidden'
-                value = value['id'] if isinstance(value, dict) else value
+                ftype = "hidden"
+                value = value["id"] if isinstance(value, dict) else value
 
-            fname = name if prefix is None else f'{prefix}__{name}'
-            data = dict(type=ftype, name=fname, label=field.label, required=field.required, value=value, help_text=field.help_text, mask=None)
+            fname = name if prefix is None else f"{prefix}__{name}"
+            data = dict(
+                type=ftype,
+                name=fname,
+                label=field.label,
+                required=field.required,
+                value=value,
+                help_text=field.help_text,
+                mask=None,
+            )
             data.update(**extra)
             for word in MASKS:
                 if word in name:
                     data.update(mask=MASKS[word])
-            for word in ('password', 'senha'):
+            for word in ("password", "senha"):
                 if word in name:
-                    data.update(type='password')
+                    data.update(type="password")
             if isinstance(field, CharField) or isinstance(field, IntegerField):
-                mask = getattr(field, 'mask', None)
+                mask = getattr(field, "mask", None)
                 if mask:
                     data.update(mask=mask)
             if isinstance(field, CharField) and isinstance(field.widget, Textarea):
-                data.update(type='textarea')
-            if ftype == 'decimal':
-                data.update(mask='decimal')
-            elif ftype == 'choice':
-                if name in self.request.GET:
-                    data.update(type='hidden', value=self.request.GET[name])
+                data.update(type="textarea")
+            if ftype == "decimal":
+                data.update(mask="decimal")
+            elif ftype == "scheduler":
+                data.update(scheduler=field.scheduler)
+            elif ftype == "choice":
+                if name in self.request.GET and not choices_field_name:
+                    data.update(type="hidden", value=self.request.GET[name])
                 else:
-                    pick = getattr(field, 'pick', False)
-                    if isinstance(field.choices, ModelChoiceIterator) and not pick:
+                    pick = getattr(field, "pick", False)
+                    if choices_field_name == fname or (isinstance(field.choices, ModelChoiceIterator) and not pick):
                         if choices_field_name == fname:
                             qs = field.choices.queryset
                             qs = self.controller.get_field_queryset(fname, qs)
-                            if 'term' in self.request.GET:
-                                qs = qs.apply_search(self.request.GET['term'])
-                            raise JsonResponseException([dict(id=obj.id, value=str(obj)) for obj in qs[0:10]])
+                            if "term" in self.request.GET:
+                                qs = qs.apply_search(self.request.GET["term"])
+                            raise JsonResponseException(
+                                [dict(id=obj.id, value=str(obj).strip()) for obj in qs[0:(50 if pick else 25)]]
+                            )
                         else:
-                            data['choices'] = absolute_url(self.request, f'choices={fname}')
+                            data["choices"] = absolute_url(
+                                self.request, f"choices={fname}"
+                            )
                     else:
-                        data['choices'] = [dict(id=str(k), value=v) for k, v in field.choices]
+                        if isinstance(field.choices, ModelChoiceIterator):
+                            data["choices"] = [
+                                dict(id=obj.id, value=str(obj).strip())
+                                for obj in self.controller.get_field_queryset(fname, field.choices.queryset)
+                            ]
+                        else:
+                            data["choices"] = [
+                                dict(id=str(k), value=v) for k, v in field.choices
+                            ]
                     if pick:
-                        data.update(pick=True)
-                    
-        attr_name = f'on_{name}_change'
+                        data.update(pick=absolute_url(
+                            self.request, f"choices={fname}"
+                        ))
+
+        attr_name = f"on_{name}_change"
         if hasattr(self._endpoint, attr_name):
-            data['onchange'] = absolute_url(self.request, f'on_change={name}')
+            data["onchange"] = absolute_url(self.request, f"on_change={name}")
         if name in self._actions:
             cls = ENDPOINTS[self._actions[name]]
             if cls.instantiate(self.request, self).check_permission():
-                data.update(action=cls.get_api_metadata(self.request, absolute_url(self.request)))
+                data.update(
+                    action=cls.get_api_metadata(
+                        self.request, absolute_url(self.request)
+                    )
+                )
         return data
-    
+
     def submit(self):
         data = {}
         errors = {}
-        inline_fields = {name: field for name, field in self.fields.items() if isinstance(field, InlineFormField) or isinstance(field, InlineModelField)}
+        inline_fields = {
+            name: field
+            for name, field in self.fields.items()
+            if isinstance(field, InlineFormField) or isinstance(field, InlineModelField)
+        }
         self.is_valid()
         errors.update(self.errors)
         for inline_field_name, inline_field in inline_fields.items():
             data[inline_field_name] = []
             for i in range(0, inline_field.max):
                 is_one_to_one = inline_field.max == inline_field.min == 1
-                prefix = inline_field_name if is_one_to_one else f'{inline_field_name}__{i}'
-                inline_form_field_name = f'{prefix}__id'
+                prefix = (
+                    inline_field_name if is_one_to_one else f"{inline_field_name}__{i}"
+                )
+                inline_form_field_name = f"{prefix}__id"
                 if inline_form_field_name in self.data:
                     inline_form_data = {}
                     pk = self.data.get(inline_form_field_name)
                     if pk:
                         pk = int(pk)
                         for name in inline_field.form.base_fields:
-                            inline_form_field_name = f'{prefix}__{name}'
-                            inline_form_data[name] = self.data.get(inline_form_field_name)
-                            if self.request.FILES and inline_form_field_name in self.request.FILES:
+                            inline_form_field_name = f"{prefix}__{name}"
+                            inline_form_data[name] = self.data.get(
+                                inline_form_field_name
+                            )
+                            if (
+                                self.request.FILES
+                                and inline_form_field_name in self.request.FILES
+                            ):
                                 self.request.FILES._mutable = True
-                                self.request.FILES[name] = self.request.FILES[inline_form_field_name]
+                                self.request.FILES[name] = self.request.FILES[
+                                    inline_form_field_name
+                                ]
                                 self.request.FILES._mutable = False
-                        instance = inline_field.form._meta.model.objects.get(pk=abs(pk)) if pk else None
+                        instance = (
+                            inline_field.form._meta.model.objects.get(pk=abs(pk))
+                            if pk
+                            else None
+                        )
                         if pk < 0:
-                            setattr(instance, 'deleting', True)
-                        inline_form = inline_field.form(data=inline_form_data, instance=instance, request=self.request)
+                            setattr(instance, "deleting", True)
+                        inline_form = inline_field.form(
+                            data=inline_form_data,
+                            instance=instance,
+                            request=self.request,
+                        )
                         if inline_form.is_valid():
                             if isinstance(inline_form, DjangoModelForm):
                                 data[inline_field_name].append(inline_form.instance)
                             else:
                                 data[inline_field_name].append(inline_form.cleaned_data)
                         else:
-                            errors.update({f'{prefix}__{name}': error for name, error in inline_form.errors.items()}) 
+                            errors.update(
+                                {
+                                    f"{prefix}__{name}": error
+                                    for name, error in inline_form.errors.items()
+                                }
+                            )
         if errors:
-            raise JsonResponseException(dict(type='error', text='Por favor, corrija os erros.', errors=errors))
+            raise JsonResponseException(
+                dict(type="error", text="Por favor, corrija os erros.", errors=errors)
+            )
         else:
-            data.update({field_name: self.cleaned_data.get(field_name) for field_name in self.fields if field_name not in inline_fields})
+            data.update(
+                {
+                    field_name: self.cleaned_data.get(field_name)
+                    for field_name in self.fields
+                    if field_name not in inline_fields
+                }
+            )
             with transaction.atomic():
                 self.cleaned_data = data
                 if isinstance(self, DjangoModelForm):
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             obj.save()
                             # set one-to-one
-                            if hasattr(self.instance, f'{inline_field_name}_id'):
-                                if hasattr(obj, 'deleting'):
+                            if hasattr(self.instance, f"{inline_field_name}_id"):
+                                if hasattr(obj, "deleting"):
                                     setattr(self.instance, inline_field_name, None)
                                 else:
                                     setattr(self.instance, inline_field_name, obj)
                     self.save()
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
-                            if hasattr(obj, 'deleting'):
+                            if hasattr(obj, "deleting"):
                                 obj.delete()
                 return self.cleaned_data
 
     def settitle(self, title):
-        self._title = title 
+        self._title = title
         return self
-    
+
     def setvalue(self, **kwargs):
         self._values.update(**kwargs)
         return self
-    
+
     def actions(self, **kwargs):
         self._actions.update(kwargs)
         return self
-    
+
 
 class Form(DjangoForm, FormMixin):
-    
+
     def __init__(self, *args, endpoint=None, **kwargs):
         self._display = []
         self._endpoint = endpoint
         self._info = None
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
-        self._method = 'POST'
+        self._method = "POST"
         self._key = self._title.lower()
 
         self.fieldsets = {}
         self.fields = {}
         self.request = endpoint.request
         self.controller = FormController(self)
-        self.instance = kwargs.pop('instance', None)
+        self.instance = kwargs.pop("instance", None)
 
         self.parse_json()
-        if 'data' not in kwargs:
-            if self.request.method.upper() == 'GET':
+        if "data" not in kwargs:
+            if self.request.method.upper() == "GET":
                 data = self.request.GET or None
-            elif self.request.method.upper() == 'POST':
+            elif self.request.method.upper() == "POST":
                 data = self.request.POST or {}
         else:
-            data = kwargs['data']
+            data = kwargs["data"]
         kwargs.update(data=data)
         if self.request:
             kwargs.update(files=self.request.FILES or None)
         super().__init__(*args, **kwargs)
 
 
 class ModelForm(DjangoModelForm, FormMixin):
@@ -389,132 +526,172 @@
     def __init__(self, instance=None, endpoint=None, **kwargs):
         self._display = []
         self._endpoint = endpoint
         self._info = None
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
-        self._method = 'POST'
+        self._method = "POST"
         self._key = self._title.lower()
 
         self.fieldsets = {}
         self.request = endpoint.request
         self.controller = FormController(self)
-        
+
         self.parse_json()
-        if 'data' not in kwargs:
-            if self.request.method.upper() == 'GET':
+        if "data" not in kwargs:
+            if self.request.method.upper() == "GET":
                 data = self.request.GET or None
-            elif self.request.method.upper() == 'POST':
+            elif self.request.method.upper() == "POST":
                 data = self.request.POST or {}
             else:
                 data = None
         else:
-            data = kwargs['data']
+            data = kwargs["data"]
         kwargs.update(data=data)
         if self.request:
             kwargs.update(files=self.request.FILES or None)
         super().__init__(instance=instance, **kwargs)
 
+
 class InlineFormField(Field):
     def __init__(self, *args, form=None, min=1, max=3, **kwargs):
         self.form = form
         self.max = max
         self.min = min
-        super().__init__(*args,  **kwargs)
+        super().__init__(*args, **kwargs)
         self.required = False
 
 
 class InlineModelField(Field):
-    def __init__(self, model, *args, fields='__all__', exclude=(), min=1, max=3, **kwargs):
-        if fields == '__all__':
-            self.form = modelform_factory(model, form=ModelForm, fields=fields, exclude=exclude)
+    def __init__(
+        self, model, *args, fields="__all__", exclude=(), min=1, max=3, **kwargs
+    ):
+        if fields == "__all__":
+            self.form = modelform_factory(
+                model, form=ModelForm, fields=fields, exclude=exclude
+            )
         else:
             field_names = []
             for field_name in fields:
                 if isinstance(field_name, str):
                     field_names.append(field_names)
                 else:
                     field_names.extend(field_name)
-            self.form = modelform_factory(model, form=ModelForm, fields=field_names, exclude=exclude)
+            self.form = modelform_factory(
+                model, form=ModelForm, fields=field_names, exclude=exclude
+            )
             self.form.fieldsets = {None: fields}
         self.max = max
         self.min = min
-        super().__init__(*args,  **kwargs)
+        super().__init__(*args, **kwargs)
         self.required = False
 
 
 class OneToManyField(InlineModelField):
-    def __init__(self, model, fields='__all__', exclude=(), min=1, max=3, **kwargs):
+    def __init__(self, model, fields="__all__", exclude=(), min=1, max=3, **kwargs):
         super().__init__(model, fields=fields, exclude=exclude, min=min, max=max)
 
+
 class OneToOneField(InlineModelField):
-    def __init__(self, model, fields='__all__', exclude=(), **kwargs):
+    def __init__(self, model, fields="__all__", exclude=(), **kwargs):
         super().__init__(model, fields=fields, exclude=exclude, min=1, max=1)
 
+
 class DecimalField(DecimalField):
     def to_python(self, value):
-        if isinstance(value, str) and ',' in value:
-            value = value.replace('.', '').replace(',', '.')
+        if isinstance(value, str) and "," in value:
+            value = value.replace(".", "").replace(",", ".")
         return super().to_python(value)
-    
+
+
 class ColorField(CharField):
     pass
 
+
 class FileField(FileField):
-    def __init__(self, *args, extensions=('pdf',), max_size=5, **kwargs):
+    def __init__(self, *args, extensions=("pdf",), max_size=5, **kwargs):
         self.extensions = extensions
         self.max_size = max_size
         super().__init__(*args, **kwargs)
 
+
 class ImageField(ImageField):
-    def __init__(self, *args, extensions=('png', 'jpg', 'jpeg'), width=None, height=None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        extensions=("png", "jpg", "jpeg"),
+        width=None,
+        height=None,
+        **kwargs,
+    ):
         self.extensions = extensions
         if width or height:
             self.width = width or height
             self.height = height or width
         else:
             self.width = self.height = 500
         super().__init__(*args, **kwargs)
 
+
 class ChoiceField(ChoiceField):
-    
+
     def __init__(self, *args, **kwargs):
-        self.pick = kwargs.pop('pick', False)
+        self.pick = kwargs.pop("pick", False)
         super().__init__(*args, **kwargs)
-    
+
+
 class MultipleChoiceField(MultipleChoiceField):
-    
+
     def __init__(self, *args, **kwargs):
-        self.pick = kwargs.pop('pick', False)
+        self.pick = kwargs.pop("pick", False)
         super().__init__(*args, **kwargs)
 
+
 class ModelChoiceField(ModelChoiceField):
-    
+
     def __init__(self, *args, **kwargs):
-        self.pick = kwargs.pop('pick', False)
+        self.pick = kwargs.pop("pick", False)
         super().__init__(*args, **kwargs)
 
+
 class ModelMultipleChoiceField(ModelMultipleChoiceField):
-    
+
     def __init__(self, *args, **kwargs):
-        self.pick = kwargs.pop('pick', False)
+        self.pick = kwargs.pop("pick", False)
+        super().__init__(*args, **kwargs)
+
+
+class SchedulerField(CharField):
+    def __init__(self, *args, scheduler=None, **kwargs):
+        self.scheduler = scheduler or Scheduler()
         super().__init__(*args, **kwargs)
-        
+
+    def clean(self, value):
+        values = dict(select=[], deselect=[])
+        if value:
+            data = json.loads(value)
+            for key in values.keys():
+                for date, hour in data[key]:
+                    data_string = "{} {}".format(date, hour)
+                    values[key].append(datetime.datetime.strptime(data_string, "%d/%m/%Y %H:%M"))
+        return values
+
 
 FIELD_TYPES = {
-    'CharField': 'text',
-    'EmailField': 'email',
-    'DecimalField': 'decimal',
-    'BooleanField': 'boolean',
-    'DateTimeField': 'datetime',
-    'DateField': 'date',
-    'IntegerField': 'number',
-    'ChoiceField': 'choice',
-    'TypedChoiceField' : 'choice',
-    'ModelChoiceField': 'choice',
-    'MultipleChoiceField': 'choice',
-    'ModelMultipleChoiceField': 'choice',
-    'ColorField': 'color',
-    'FileField': 'file',
-    'ImageField': 'file',
-}
+    "CharField": "text",
+    "EmailField": "email",
+    "DecimalField": "decimal",
+    "BooleanField": "boolean",
+    "DateTimeField": "datetime",
+    "DateField": "date",
+    "IntegerField": "number",
+    "ChoiceField": "choice",
+    "TypedChoiceField": "choice",
+    "ModelChoiceField": "choice",
+    "MultipleChoiceField": "choice",
+    "ModelMultipleChoiceField": "choice",
+    "ColorField": "color",
+    "FileField": "file",
+    "ImageField": "file",
+    "SchedulerField": "scheduler",
+}
```

### Comparing `pyslth-0.3.2/slth/management/commands/integration_test.py` & `pyslth-0.3.3/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/management/commands/sync.py` & `pyslth-0.3.3/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/migrations/0001_initial.py` & `pyslth-0.3.3/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.3/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.3/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/migrations/0006_user.py` & `pyslth-0.3.3/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/models.py` & `pyslth-0.3.3/slth/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.contrib.auth.models import User
 from django.apps import apps
 from datetime import datetime
 from django.utils.html import strip_tags
 from django.core.mail import EmailMultiAlternatives
 from slth import APPLICATON
 
-
 class RoleQuerySet(models.QuerySet):
 
     def contains(self, *names):
         _names = getattr(self, '_names', None)
         if _names is None:
             _names = set(self.filter(name__in=names, active=True).values_list('name', flat=True))
             setattr(self, '_names', _names)
@@ -183,9 +182,9 @@
     
     @meta('Inscrições de Notificação')
     def get_push_subscriptions(self):
         return self.pushsubscription_set.fields('device')
     
     @meta('Papéis')
     def get_roles(self):
-        return Role.objects.filter(username=self.username).fields('get_description')
+        return Role.objects.filter(username=self.username).fields('get_description').actions('delete')
```

### Comparing `pyslth-0.3.2/slth/oauth.py` & `pyslth-0.3.3/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/permissions.py` & `pyslth-0.3.3/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/queryset.py` & `pyslth-0.3.3/slth/queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
         self.metadata['title'] = name or str(self.model._meta.verbose_name_plural)
         return self
     
     def attrname(self, name):
         self.metadata['attrname'] = name
         return self
     
+    def reloadable(self):
+        self.metadata['reloadable'] = True
+        return self
+    
     def calendar(self, name):
         self.metadata['calendar'] = name
         return self
     
     def related_values(self, **kwargs):
         self.metadata['relations'] = {
             k: v if isinstance(v, int) else v.pk for k, v in kwargs.items()
@@ -172,15 +176,15 @@
 
         if choices_field_name:
             field = qs.model.get_field(choices_field_name)
             choices = field.related_model.objects.filter(pk__in=qs.values_list(choices_field_name, flat=True))
             term = self.request.GET.get('term')
             if term:
                 choices = choices.apply_search(term)
-            raise JsonResponseException([dict(id=obj.id, value=str(obj)) for obj in choices[0:20]])
+            raise JsonResponseException([dict(id=obj.id, value=str(obj).strip()) for obj in choices[0:20]])
 
 
         return qs
 
     def apply_filter(self, lookup, value):
         booleans = dict(true=True, false=False, null=None)
         if len(value) == 10 and '-' in value:
@@ -191,24 +195,25 @@
 
     def apply_search(self, term, lookups=None):
         if lookups is None:
             search_fields = getattr(self.model._meta, 'search_fields', None)
             if search_fields is None:
                 search_fields = [field.name for field in self.model._meta.get_fields() if isinstance(field, CharField)]
             lookups = [f'{name}__icontains' for name in search_fields]
+        else:
+            lookups = [name if name.endswith('__icontains') else f'{name}__icontains' for name in lookups]
         if lookups:
             terms = term.split(' ') if term else []
             conditions = []
             for term in terms:
                 queries = [
                     Q(**{lookup: term})
                     for lookup in lookups
                 ]
                 conditions.append(reduce(operator.or_, queries))
-
             return self.filter(reduce(operator.and_, conditions)) if conditions else self
         return self
     
     def parameter(self, name, default=None):
         return self.request.GET.get(name, default) if self.request else default
     
     def serialize(self, debug=False, forward_exception=False):
@@ -221,14 +226,15 @@
     
     def to_dict(self, debug=False):
         title = self.metadata.get('title', str(self.model._meta.verbose_name_plural))
         title = title.title() if title and title.islower() else title
         attrname = self.metadata.get('attrname')
         relations = self.metadata.get('relations')
         renderer = self.metadata.get('renderer')
+        reloadable = self.metadata.get('reloadable')
         bi = self.metadata.get('bi', [])
         subset = None
         actions = []
         filters = []
         search = []
         subsets = []
         aggregations = []
@@ -274,32 +280,34 @@
             if lookup.endswith('userrole'):
                 field = self.role_filter_field()
             else:
                 field = self.filter_field(lookup, base_url)
             if field:
                 filters.append(field)
 
-        total = self.count()
+        total = qs.count()
         for name in self.metadata.get('subsets', ()):
             attr = getattr(self, name)
             label = getattr(attr, 'verbose_name', name.title())
             subsets.append(dict(name=name, label=label, count=attr().count()))
         if subsets:
             subsets.insert(0, dict(name=None, label='Tudo', count=total))
 
         for name in self.metadata.get('aggregations', ()):
             api_name = name[4:] if name.startswith('get_') else name
             aggregation = dict(name=api_name, label=api_name, value=getattr(self, name)())
             if isinstance(aggregation['value'], Decimal):
                 aggregation['value'] = str(aggregation['value']).replace('.', ',')
             aggregations.append(aggregation)
 
-        data = dict(type='queryset', title=title, key=attrname, url=base_url, total=total, count=total, icon=None, actions=actions, filters=filters, search=search)
+        data = dict(type='queryset', title=title, key=attrname, url=base_url, total=total, count=total, icon=None, actions=actions, filters=filters, search=search, q=self.request.GET.get('q'))
         if renderer:
             data.update(renderer=renderer)
+        if reloadable:
+            data.update(reloadable=reloadable)
         if bi:
             bi_data = []
             for names in bi:
                 items = []
                 for name in names:
                     attr = getattr(qs, name)
                     title = getattr(attr, 'verbose_name', name.title())
```

### Comparing `pyslth-0.3.2/slth/roles.py` & `pyslth-0.3.3/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/selenium/__init__.py` & `pyslth-0.3.3/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/selenium/browser.py` & `pyslth-0.3.3/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/serializer.py` & `pyslth-0.3.3/slth/serializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,28 @@
 from django.utils.text import slugify
 from .exceptions import JsonResponseException
 from .utils import absolute_url, build_url
 from .components import Image, FileLink, FileViewer
 from django.db.models.fields.files import ImageFieldFile, FieldFile
 
 
+def getattrr(obj, args):
+    return getattr_rec(obj, args.split('__'))
+
+
+def getattr_rec(obj, args):
+    if obj is None:
+        return None
+    if len(args) > 1:
+        attr = args.pop(0)
+        return getattr_rec(getattrr(obj, attr), args)
+    else:
+        return getattr(obj, args[0])
+
+
 def to_snake_case(name):
     return slugify(name).replace('-', '_')
 
 
 def serialize(obj, primitive=False, request=None):
     if obj is None:
         return None
@@ -51,24 +65,24 @@
 
 def getfield(obj, name_or_names, request=None):
     if isinstance(name_or_names, str):
         if ':' in name_or_names:
             name_or_names, action_name = name_or_names.split(':')
         else:
             name_or_names, action_name = name_or_names, None
-        attr = getattr(obj, name_or_names)
+        attr = getattrr(obj, name_or_names)
         if type(attr) == types.MethodType:
             value = attr()
             label = getattr(attr, 'verbose_name', name_or_names.replace('get_', ''))
         elif name_or_names.startswith('get_') and name_or_names.endswith('_display'):
             value = attr()
             label = getattr(type(obj), name_or_names[4:-8]).field.verbose_name
         else:
             value = attr
-            label = getattr(type(obj), name_or_names).field.verbose_name
+            label = type(obj).get_field(name_or_names).verbose_name
         label = label.title().replace('_', ' ') if label and label.islower() else label
         field = dict(type='field', name=name_or_names, label=label, value=serialize(value, primitive=True, request=request))
         if action_name:
             cls = slth.ENDPOINTS[action_name]
             endpoint = cls.instantiate(request, obj)
             if endpoint.check_permission():
                 field.update(url=endpoint.get_api_url(obj.id))
@@ -77,15 +91,15 @@
         fields = []
         for name in name_or_names:
             fields.append(getfield(obj, name, request))
         return fields
 
 
 class Serializer:
-    def __init__(self, obj=None, request=None, serializer=None, type='object', title=None):
+    def __init__(self, obj=None, request=None, serializer=None, type='object', title=None, show_title=True):
         self.path = serializer.path.copy() if serializer else []
         self.obj = obj
         self.lazy = False
         self.ignore_only = False
         self.request = request
         self.metadata = dict(actions=[], content=[], allow=[])
         self.serializer:Serializer = serializer
@@ -93,55 +107,60 @@
         if title:
             self.title = title
             self.path.append(to_snake_case(title))
         elif isinstance(obj, Model):
             self.title = str(obj)
         else:
             self.title = None
+        self.show_title = show_title
 
     def actions(self, *actions) -> 'Serializer':
         self.metadata['actions'].extend(actions)
         self.metadata['allow'].extend(actions)
         return self
     
-    def field(self, name, reload=True) -> 'Serializer':
-        self.metadata['content'].append(('field', name, dict(name=name, reload=reload)))
+    def field(self, name, reload=True, condition=None, roles=()) -> 'Serializer':
+        self.metadata['content'].append(('field', name, dict(name=name, reload=reload, condition=condition, roles=roles)))
         return self
         
-    def fields(self, *names) -> 'Serializer':
-        self.metadata['content'].append(('fields', None, dict(names=names)))
+    def fields(self, *names, condition=None, roles=()) -> 'Serializer':
+        self.metadata['content'].append(('fields', None, dict(names=names, condition=condition, roles=roles)))
         return self
     
-    def fieldset(self, title, fields=(), actions=(), attr=None, reload=True) -> 'Serializer':
+    def fieldset(self, title, fields=(), actions=(), attr=None, reload=True, condition=None, roles=()) -> 'Serializer':
         self.metadata['allow'].extend(actions)
-        item = dict(title=title, names=fields, attr=attr, actions=actions, reload=reload)
+        item = dict(title=title, names=fields, attr=attr, actions=actions, reload=reload, condition=condition, roles=roles)
         self.metadata['content'].append(('fieldset', to_snake_case(title), item))
         return self
         
-    def queryset(self, title, name) -> 'Serializer':
-        self.metadata['content'].append(('queryset', name, dict(title=title)))
+    def queryset(self, title, name, condition=None, roles=()) -> 'Serializer':
+        self.metadata['content'].append(('queryset', name, dict(title=title, condition=condition, roles=roles)))
         return self
     
-    def endpoint(self, title, cls, wrap=True) -> 'Serializer':
+    def endpoint(self, title, cls, wrap=True, condition=None, roles=()) -> 'Serializer':
         if isinstance(cls, str):
             cls = slth.ENDPOINTS[cls]
-        self.metadata['content'].append(('endpoint', to_snake_case(title), dict(title=title, cls=cls, wrap=wrap)))
+        self.metadata['content'].append(('endpoint', to_snake_case(title), dict(title=title, cls=cls, wrap=wrap, condition=condition, roles=roles)))
         return self
     
-    def append(self, title, component) -> 'Serializer':
-        self.metadata['content'].append(('component', to_snake_case(title), dict(title=title, component=component)))
+    def append(self, title, component, condition=None, roles=()) -> 'Serializer':
+        self.metadata['content'].append(('component', to_snake_case(title), dict(title=title, component=component, condition=condition, roles=roles)))
     
     def section(self, title) -> 'Serializer':
         return Serializer(obj=self.obj, request=self.request, serializer=self, type='section', title=title)
     
-    def group(self, title) -> 'Serializer':
-        return Serializer(obj=self.obj, request=self.request, serializer=self, type='group', title=title)
+    def group(self, title=None) -> 'Serializer':
+        show_title = True
+        if title is None:
+            title = 'group'
+            show_title = False
+        return Serializer(obj=self.obj, request=self.request, serializer=self, type='group', title=title, show_title=show_title)
 
     def parent(self) -> 'Serializer':
-        self.serializer.metadata['content'].append(('serializer', to_snake_case(self.title), dict(serializer=self)))
+        self.serializer.metadata['content'].append(('serializer', to_snake_case(self.title), dict(serializer=self, condition=None, roles=())))
         return self.serializer
     
     def contextualize(self, request) -> 'Serializer':
         self.request = request
         return self
     
     def settitle(self, title) -> 'Serializer':
@@ -157,14 +176,28 @@
             if debug:
                 print(json.dumps(e.data, indent=2, ensure_ascii=False))
             return e.data
         
     def __str__(self):
         return f'{self.title} / {self.type}'
 
+    def check_condition(self, name):
+        if name:
+            deny = False
+            if name.startswith('not '):
+                deny, name = name.split()
+            attr = getattr(self.obj, name)
+            if callable(attr):
+                attr = attr()
+            return not attr if deny else attr
+        return True
+    
+    def check_role(self, names):
+        from slth.models import Role
+        return self.request.user.is_superuser or not names or Role.objects.filter(username=self.request.user.username, name__in=names).exists()
 
     def to_dict(self, debug=False):
         base_url = absolute_url(self.request)
         if self.request is None and self.serializer:
             self.request = self.serializer.request
         if self.ignore_only:
             only = []
@@ -194,14 +227,18 @@
             self.fields(*[field.name for field in type(self.obj)._meta.fields])
             for m2m in type(self.obj)._meta.many_to_many:
                 self.queryset(m2m.verbose_name, m2m.name)
         
         items = []
         if not self.lazy:
             for i, (datatype, key, item) in enumerate(self.metadata['content']):
+                if not self.check_condition(item['condition']):
+                    continue
+                if not self.check_role(item['roles']):
+                    continue
                 leaf = only and only[-1] == key
                 lazy = i and self.type == 'group' and not leaf
                 data = None
                 if datatype == 'field':
                     path = self.path + [item['name']]
                     data = getfield(self.obj, item['name'], self.request)
                     if item['reload']:
@@ -290,15 +327,15 @@
                         serializer.lazy = False
                         serializer.ignore_only = self.ignore_only or leaf
                         data = serializer.to_dict()
                         if leaf: raise JsonResponseException(data)
                 if data:
                     items.extend(data) if datatype == 'fields' else items.append(data)
 
-        output = dict(type=self.type, title=self.title)
+        output = dict(type=self.type, title=self.title if self.show_title else None)
         if self.serializer:
             datatype = to_snake_case(self.title)
             output.update(key=datatype)
         if self.path:
             url = absolute_url(self.request, 'only={}'.format('__'.join(self.path)))
         else:
             url = absolute_url(self.request)
```

### Comparing `pyslth-0.3.2/slth/static/css/.DS_Store` & `pyslth-0.3.3/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fontawesome.min.css` & `pyslth-0.3.3/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.3/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.3/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.3/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.3/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.3/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/css/slth.css` & `pyslth-0.3.3/slth/static/css/slth.css`

 * *Files 11% similar despite different names*

```diff
@@ -64,7 +64,19 @@
 
   form.login {
     width: 350px;
   }
   form.login h1{
     text-align: center;
   }
+
+
+  /* .object-viewer .object-fieldset {
+    border: solid 1px #2c3e50;
+    border-radius: 5px;
+  }
+
+  .object-viewer .object-fieldset .fieldset-title{
+    background-color: #2c3e50;
+    color: white;
+    padding: 5px;
+  } */
```

### Comparing `pyslth-0.3.2/slth/static/css/solid.min.css` & `pyslth-0.3.3/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/images/logo.png` & `pyslth-0.3.3/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/images/logo.svg` & `pyslth-0.3.3/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/images/user.png` & `pyslth-0.3.3/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/echarts.min.js` & `pyslth-0.3.3/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/index.min.js` & `pyslth-0.3.3/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/ios-splash.min.js` & `pyslth-0.3.3/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/peerjs.min.js` & `pyslth-0.3.3/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/qrcode.min.js` & `pyslth-0.3.3/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/react-trigger-change.js` & `pyslth-0.3.3/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/react.min.js` & `pyslth-0.3.3/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/slth.min.js` & `pyslth-0.3.3/slth/static/js/slth.min.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
-    c as F,
+    c as z,
     r as I,
-    R as Be
+    R as Te
 } from "./react.min.js";
-const S = {
+const k = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -34,15 +34,15 @@
         return t.jsx("div", {
             style: a
         })
     }
     return n()
 }
 
-function Le(e) {
+function Ie(e) {
     function n(r) {
         navigator.clipboard.writeText(r), te('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
@@ -62,104 +62,104 @@
                 className: "icon-text",
                 children: r
             })]
         }, Math.random()))
     })
 }
 
-function Ae(e) {
+function Be(e) {
     function n() {
         return t.jsx("i", {
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function j(e) {
+function S(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
 
-function fe(e) {
+function ge(e) {
     function n() {
         const a = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = S.colors.primary, a.color = "white"), e.default && (a.color = S.colors.primary, a.border = "solid 1px " + S.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = k.colors.primary, a.color = "white"), e.default && (a.color = k.colors.primary, a.border = "solid 1px " + k.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(j, {
+            children: t.jsx(S, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function Re(e) {
+function Le(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : S.colors.primary,
+            backgroundColor: e.isError ? "#e52207" : k.colors.success,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(j, {
+            children: [t.jsx(S, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
 function te(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), F.createRoot(document.body.appendChild(a)).render(t.jsx(Re, {
+    a.classList.add("message"), z.createRoot(document.body.appendChild(a)).render(t.jsx(Le, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function oe() {
+function le() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function de(e) {
+function oe(e) {
     function n() {
         const a = {
-            color: S.colors.info,
-            backgroundColor: S.background.info,
+            color: k.colors.info,
+            backgroundColor: k.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -171,510 +171,541 @@
             })]
         })
     }
     return n()
 }
 
 function Ne(e) {
-    return pe(e.data)
+    return we(e.data)
 }
 
-function q(e) {
+function A(e) {
     return e.replace("/app/", "/api/")
 }
 
 function U(e) {
     return e.replace("/api/", "/app/")
 }
 
-function B(e, n, a, r) {
-    const o = localStorage.getItem("token");
-    var i = {
+function L(e, n, a, r) {
+    const i = localStorage.getItem("token");
+    var l = {
         Accept: "application/json"
     };
-    o && (i.Authorization = "Token " + o);
-    const l = q(n);
-    var s = {
+    i && (l.Authorization = "Token " + i);
+    const d = A(n);
+    var c = {
         method: e,
-        headers: new Headers(i),
+        headers: new Headers(l),
         ajax: 1
     };
-    r && (s.body = r);
-    var c = null,
+    r && (c.body = r);
+    var s = null,
         u = null;
-    fetch(l, s).then(function(d) {
-        if (c = d, u = c.headers.get("Content-Type"), u == "application/json") return d.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return d.arrayBuffer();
-        d.text()
-    }).then(d => {
+    fetch(d, c).then(function(o) {
+        if (s = o, u = s.headers.get("Content-Type"), u == "application/json") return o.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
+        o.text()
+    }).then(o => {
         if (u == "application/json") {
-            var h = JSON.parse(d || "{}");
-            typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, c)
+            var h = JSON.parse(o || "{}");
+            typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var f = window.URL.createObjectURL(new Blob([new Uint8Array(d)], {
+            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
                     type: u
                 })),
                 w = document.createElement("a");
-            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, c)
-        } else a && a(d, c)
+            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
+        } else a && a(o, s)
     })
 }
 
-function pe(e) {
+function we(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
     }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = U(e.redirect)) : e.message && te(e.message)
 }
 
-function W(e) {
+function F(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
     if (typeof e == "string") {
-        if (e.length == 7 && e[0] == "#") return t.jsx(p, {
+        if (e.length == 7 && e[0] == "#") return t.jsx(x, {
             data: {
                 type: "color",
                 value: e
             }
         });
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
                 a = n[0],
                 r = n[1];
             return r == "00:00:00" ? a : a + " " + r
-        }
+        } else if (e.indexOf(`
+`) >= 0) return e.split(`
+`).map(function(i, l) {
+            return t.jsx("div", {
+                children: i
+            }, Math.random())
+        });
         return e
     }
-    return typeof e == "object" && e.type ? t.jsx(p, {
+    return typeof e == "object" && e.type ? t.jsx(x, {
         data: e
-    }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
+    }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : typeof e[0] == "object" && e[0].type != null ? t.jsx(t.Fragment, {
+        children: e.map(function(i) {
+            return t.jsx(x, {
+                data: i
+            }, Math.random())
+        })
+    }) : t.jsx("ul", {
         style: {
-            padding: 0
+            padding: 0,
+            marginLeft: 17
         },
-        children: e.map(function(o) {
+        children: e.map(function(i) {
             return t.jsx("li", {
-                children: o
+                children: i
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
-function se() {
-    document.querySelector(".layer") == null && F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {}))
+function de() {
+    document.querySelector(".layer") == null && z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
-function be(e, n) {
-    oe(), se(), window.reloader = n;
+function pe(e, n) {
+    le(), de(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
-        url: q(e)
+    z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+        url: A(e)
     }))
 }
 
-function Oe(e) {
-    oe(), se(), F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(We, {
-        url: q(e)
+function Ae(e) {
+    le(), de(), z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+        url: A(e)
     }))
 }
 
-function J(e) {
+function G(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function _e(e) {
-    oe(), se(), F.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(He, {
+function Re(e) {
+    le(), de(), z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
-function Fe(e) {
+function Oe(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
         opacity: .7,
         display: "none"
     };
     return t.jsx("div", {
         className: "layer",
         onClick: function() {
-            J()
+            G()
         },
         style: n
     })
 }
 
-function ze(e) {
-    const [n, a] = I.useState(null), [r, o] = I.useState(0);
+function _e(e) {
+    const [n, a] = I.useState(null), [r, i] = I.useState(0);
     I.useEffect(() => {
-        i(q(e.url)), document.querySelector(".layer").style.display = "block"
+        l(A(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
-    function i(c) {
-        B("GET", q(c), function(u) {
-            a(u), o(r + 1)
+    function l(s) {
+        L("GET", A(s), function(u) {
+            a(u), i(r + 1)
         })
     }
 
-    function l() {
-        const c = {
+    function d() {
+        const s = {
                 maxWidth: 800
             },
             u = {
                 textAlign: "right",
                 cursor: "pointer",
                 marginTop: -15
             };
         if (n) return t.jsxs("div", {
-            style: c,
+            style: s,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(j, {
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => J()
+                    onClick: () => G()
                 })
-            }), t.jsx(p, {
+            }), t.jsx(x, {
                 data: n
             })]
         })
     }
-    const s = {
-        minWidth: "50%",
+    const c = {
+        minWidth: window.innerWidth < 800 ? "calc(100% - 60px)" : 800,
         display: n ? "block" : "none",
         maxWidth: 800,
         top: window.scrollY + 40,
         border: 0
     };
     return t.jsx("dialog", {
-        style: s,
-        children: l()
+        style: c,
+        children: d()
     }, r)
 }
 
-function We(e) {
+function Fe(e) {
     var n = Math.random();
     I.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
-                minWidth: "50%",
+                minWidth: window.innerWidth < 800 ? "calc(100% - 60px)" : 800,
                 display: "block",
                 maxWidth: 800,
                 top: window.scrollY + 40,
                 border: 0
             },
-            o = {
+            i = {
                 float: "right",
                 cursor: "pointer",
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
-                style: o,
-                children: t.jsx(j, {
+                style: i,
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => J()
+                    onClick: () => G()
                 })
             }), t.jsx("iframe", {
-                src: q(e.url),
+                src: A(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
     }
     return a()
 }
 
-function He(e) {
+function ze(e) {
     const n = Math.random();
     I.useEffect(() => {
         document.querySelector(".layer").style.display = "block"
     }, []);
 
     function a() {
-        const i = {
+        const l = {
             width: "100%",
             borderBottom: "solid 1px #DDDD",
             padding: 20
         };
         return t.jsx("div", {
             align: "center",
             style: {},
-            children: e.actions.map(function(l) {
+            children: e.actions.map(function(d) {
                 return t.jsx("div", {
-                    style: i,
+                    style: l,
                     onClick: r,
                     children: t.jsx(_, {
-                        data: l,
+                        data: d,
                         strech: !0
                     })
                 }, Math.random())
             })
         })
     }
 
     function r() {
-        const i = document.getElementById(n);
-        i.close(), i.classList.remove("opened"), i.remove(), document.querySelector(".layer").style.display = "none"
+        const l = document.getElementById(n);
+        l.close(), l.classList.remove("opened"), l.remove(), document.querySelector(".layer").style.display = "none"
     }
-    const o = {
+    const i = {
         width: "auto",
         display: "block",
         position: "fixed",
         bottom: 0,
         border: 0,
         padding: 0
     };
     return t.jsx("dialog", {
         id: n,
-        style: o,
+        style: i,
         children: a()
     })
 }
 
-function T(e) {
+function M(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function _(e) {
     const n = e.id || Math.random(),
         [a, r] = I.useState(e.data.name);
 
-    function o(s) {
-        s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(U(e.data.url)) : be(e.data.url)
+    function i(c) {
+        c.preventDefault();
+        var s = e.data.url;
+        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
     }
 
-    function i() {
-        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(j, {
+    function l() {
+        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(j, {
+            children: [t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
-    function l() {
-        var s = {
+    function d() {
+        var c = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
-            margin: 5
+            margin: 5,
+            minWidth: 50
         };
-        return e.primary && (s.backgroundColor = S.colors.primary, s.color = "white"), e.default && (s.border = "solid 1px " + S.colors.primary, s.color = S.colors.primary), e.style && Object.keys(e.style).map(function(c) {
-            s[c] = e.style[c]
+        return e.primary && (c.backgroundColor = k.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + k.colors.primary, c.color = k.colors.primary), e.style && Object.keys(e.style).map(function(s) {
+            c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
             href: U(e.data.url) || "#",
-            onClick: o,
-            style: s,
-            "data-label": T(e.data.name),
-            children: i()
+            onClick: i,
+            style: c,
+            "data-label": M(e.data.name),
+            children: l()
         })
     }
-    return l()
+    return d()
 }
 
-function X(e) {
-    function n(i) {
-        var l = i.target.parentNode.querySelector(".dropdown");
-        return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
+function K(e) {
+    function n(l) {
+        var d = l.target.parentNode.querySelector(".dropdown");
+        return d == null && (d = l.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = l.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
     }
 
-    function a(i) {
-        const l = n(i);
-        if (l.style.display == "block") l.style.display = "none";
+    function a(l) {
+        const d = n(l);
+        if (d.style.display == "block") d.style.display = "none";
         else {
-            const s = i.target.getBoundingClientRect();
-            document.querySelectorAll(".dropdown").forEach(c => c.style.display = "none"), l.style.left = s.left - 150 + s.width + "px", l.style.display = "block"
+            const c = l.target.getBoundingClientRect();
+            document.querySelectorAll(".dropdown").forEach(s => s.style.display = "none"), d.style.left = c.left - 150 + c.width + "px", d.style.display = "block"
         }
     }
 
-    function r(i) {
-        const l = n(i);
-        l.style.display = "none"
+    function r(l) {
+        const d = n(l);
+        d.style.display = "none"
     }
 
-    function o() {
-        const i = {
+    function i() {
+        const l = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
                 boxShadow: "15px 15px 10px -15px #DDD",
                 display: "none"
             },
-            l = {
+            d = {
                 listStyleType: "none",
                 padding: 10
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": T(e.dataLabel),
+                "data-label": M(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
-                style: i,
+                style: l,
                 onMouseLeave: r,
                 className: "dropdown",
-                children: e.actions.map(s => t.jsx("li", {
-                    style: l,
+                children: e.actions.map(c => t.jsx("li", {
+                    style: d,
                     children: t.jsx(_, {
-                        data: s,
+                        data: c,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
-    return o()
+    return i()
 }
 
-function N({
+function O({
     id: e,
     href: n,
     modal: a,
     imodal: r,
-    children: o,
-    onClick: i,
-    dataLabel: l,
-    style: s
+    children: i,
+    onClick: l,
+    dataLabel: d,
+    style: c
 }) {
-    const c = n && n.indexOf("/media/") < 0 ? U(n) : n;
+    const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
-        c.indexOf("http") == 0 ? document.location.href = c : (h.preventDefault(), a ? be(c) : r ? Oe(c) : window.load(c))
+        s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
     }
 
-    function d() {
+    function o() {
         return t.jsx("a", {
             id: e,
-            onClick: i || u,
-            href: c || "#",
-            "data-label": T(l),
-            style: s,
-            children: o
+            onClick: l || u,
+            href: s || "#",
+            "data-label": M(d),
+            style: c,
+            children: i
         })
     }
-    return d()
+    return o()
 }
 
-function G(e) {
+function P(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
             gridTemplateColumns: "repeat(auto-fit, minmax(" + (e.width || 200) + "px, 1fr))",
             alignItems: e.alignItems || "end"
         };
         return t.jsx("div", {
             style: r,
             children: e.children
-        })
+        }, Math.random())
     }
     return n()
 }
 
-function Y(e) {
+function W(e) {
+    let n = "",
+        a = window.document.styleSheets[0];
+    e.split("}").forEach(r => {
+        let i = (r + "}").replace(/\r?\n|\r/g, "");
+        n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && (a.insertRule(n, a.cssRules.length), n = "")
+    })
+}
+
+function V(e) {
     function n() {
-        return e.data.url ? t.jsx(Pe, {
+        return e.data.url ? t.jsx(We, {
             data: e.data
-        }) : t.jsx(we, {
+        }) : t.jsx(je, {
             data: e.data
         })
     }
     return n()
 }
 
-function we(e) {
+function je(e) {
     function n() {
-        return e.data.url ? t.jsx(N, {
+        if (e.data.label) return t.jsxs(t.Fragment, {
+            children: [t.jsx("strong", {
+                children: e.data.label
+            }), ":", t.jsx("br", {})]
+        })
+    }
+
+    function a() {
+        return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(O, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
-                children: [W(e.data.value), t.jsx(j, {
+                children: [F(e.data.value), t.jsx(S, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
                 })]
             })
-        }) : W(e.data.value)
+        }) : F(e.data.value)
     }
 
-    function a() {
-        const r = {
+    function r() {
+        const i = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsxs("div", {
-            style: r,
-            children: [t.jsx("strong", {
-                children: e.data.label
-            }), ":", t.jsx("br", {}), n()]
+            style: i,
+            children: [n(), a()]
         })
     }
-    return a()
+    return r()
 }
 
-function Pe(e) {
+function We(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data);
 
-    function o(l) {
-        B("GET", l, function(s) {
-            r(s)
+    function i(d) {
+        L("GET", d, function(c) {
+            r(c)
         })
     }
 
-    function i() {
-        return window[n] = () => o(e.data.url), t.jsx("div", {
+    function l() {
+        return window[n] = () => i(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: t.jsx(we, {
+            children: t.jsx(je, {
                 data: a,
                 width: 100
             })
         })
     }
-    return i()
+    return l()
 }
 
-function je(e) {
+function se(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
                 textAlign: "right",
                 lineHeight: "3rem"
             },
@@ -686,631 +717,1265 @@
                 }, Math.random())
             })
         })
     }
     return n()
 }
 
-function ke(e) {
+function ce(e) {
     function n() {
         return e.data.map(function(a) {
-            if (Array.isArray(a)) return t.jsx(G, {
+            if (Array.isArray(a)) return t.jsx(P, {
                 width: 300,
                 alignItems: "start",
-                children: a.map(r => t.jsx(Y, {
+                children: a.map(r => t.jsx(V, {
                     data: r,
                     width: 100 / a.length
                 }, Math.random()))
             }, Math.random());
-            if (a.label != "ID" && a.label != e.exclude) return t.jsx("div", {
-                children: t.jsx(Y, {
+            if (a.label != "ID" && (e.exclude == null || a.label != e.exclude)) return t.jsx("div", {
+                children: t.jsx(V, {
                     data: a,
                     width: 100
                 })
             }, Math.random())
         })
     }
     return n()
 }
 
-function Ue(e) {
+function Pe(e) {
     function n() {
-        const i = {
+        const l = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
-            style: i,
+            style: l,
             children: e.data.title
         })
     }
 
     function a() {
-        return t.jsx(ke, {
+        return t.jsx(ce, {
             data: e.data.data
         })
     }
 
     function r() {
-        return t.jsx(je, {
+        return t.jsx(se, {
             data: e.data.actions
         })
     }
 
-    function o() {
-        const i = {
+    function i() {
+        const l = {
             border: "solid 1px #DDD",
             padding: 10,
             borderStyle: "dashed"
         };
         return t.jsxs("div", {
-            style: i,
+            style: l,
             children: [n(), a(), r()]
         })
     }
-    return o()
+    return i()
 }
 
-function Ge(e) {
+function He(e) {
+    W(`
+    .cards{
+      padding: 10px;
+      box-shadow: 0 1px 6px rgba( 0, 0, 0 , 0.16 );
+      margin: 10px;
+    }
+    .cards h3{
+      margin-top: 5px;
+      margin-bottom: 5px;
+      height: 3rem;
+      overflow-y: hidden;
+    }
+    .cards img{
+      width: 100% !important;
+      height: 150px !important;
+      object-fit: cover;
+    }
+  `);
+
     function n() {
-        const l = {
+        return t.jsx("h3", {
+            children: e.data.title
+        })
+    }
+
+    function a() {
+        return t.jsx(ce, {
+            data: e.data.data
+        })
+    }
+
+    function r() {
+        return t.jsx(se, {
+            data: e.data.actions
+        })
+    }
+
+    function i() {
+        return t.jsxs("div", {
+            className: "cards",
+            children: [n(), a(), r()]
+        })
+    }
+    return i()
+}
+
+function Ue(e) {
+    function n() {
+        const d = {
             paddingTop: 15,
             marginBottom: 10,
             color: "#1151b3"
         };
         return t.jsx("div", {
-            style: l,
+            style: d,
             children: t.jsx("strong", {
                 children: e.data.title
             })
         })
     }
 
     function a() {
-        return t.jsx(ke, {
+        return t.jsx(ce, {
             data: e.data.data,
             exclude: e.data.data[1].label
         })
     }
 
     function r() {
-        const l = {
+        const d = {
                 position: "absolute",
                 width: 140,
                 marginLeft: -128,
                 display: "flex",
                 justifyContent: "space-between",
                 marginTop: 10,
                 alignItems: "flex-end"
             },
-            s = {
+            c = {
                 maxWidth: 100
             },
-            c = {
+            s = {
                 width: 20,
                 height: 20,
                 border: "3px solid #1151b3",
                 backgroundColor: "white",
                 borderRadius: "50%"
             };
         return t.jsxs("div", {
-            style: l,
+            style: d,
             children: [t.jsx("div", {
-                style: s,
+                style: c,
                 children: e.data.data[1].value
             }), t.jsx("div", {
-                style: c
+                style: s
             })]
         })
     }
 
-    function o() {
-        return t.jsx(je, {
+    function i() {
+        return t.jsx(se, {
             data: e.data.actions
         })
     }
 
-    function i() {
-        const l = {
+    function l() {
+        const d = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
                 marginBottom: -10
             },
-            s = {
+            c = {
                 marginLeft: 20
             };
         return t.jsxs("div", {
-            style: l,
+            style: d,
             children: [r(), t.jsxs("div", {
-                style: s,
-                children: [n(), a(), o()]
+                style: c,
+                children: [n(), a(), i()]
             })]
         })
     }
-    return i()
+    return l()
 }
 
-function Ve(e) {
+function Ge(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data);
+    W(`
+    .object-fieldset{
+      margin-top: 10px;
+    }
+  `);
 
-    function o() {
-        return t.jsx(Se, {
+    function i() {
+        return t.jsx(ke, {
             data: a
         })
     }
 
-    function i() {
+    function l() {
         const u = {
             backgroundColor: "white",
             padding: 15,
             marginBottom: 15
         };
         return t.jsx("div", {
             style: u,
-            children: l()
+            children: d()
         })
     }
 
-    function l() {
+    function d() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
-            return Array.isArray(u) ? t.jsx(G, {
+            return Array.isArray(u) ? t.jsx(P, {
                 width: 300,
-                children: u.map(d => t.jsx(Y, {
-                    data: d,
+                children: u.map(o => t.jsx(V, {
+                    data: o,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
-                children: t.jsx(Y, {
+                children: t.jsx(V, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
-        }) : t.jsx(p, {
+        }) : t.jsx(x, {
             data: a.data
         })
     }
 
-    function s(u) {
-        B("GET", u, function(d) {
-            r(d)
+    function c(u) {
+        L("GET", u, function(o) {
+            r(o)
         })
     }
 
-    function c() {
-        return e.data.url ? (window[n] = () => s(e.data.url), t.jsxs("div", {
-            className: e.data.url && "reloadable",
+    function s() {
+        return e.data.url ? (window[n] = () => c(e.data.url), t.jsxs("div", {
+            className: e.data.url ? "reloadable object-fieldset" : "object-fieldset",
             id: n,
-            children: [o(), i()]
+            children: [i(), l()]
         })) : t.jsxs("div", {
-            children: [o(), i()]
+            className: "object-fieldset",
+            children: [i(), l()]
         })
     }
-    return c()
+    return s()
 }
 
-function $e(e) {
+function Ve(e) {
     const n = Math.random(),
         [a, r] = I.useState(e.data.actions);
 
-    function o() {
-        const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
-        return e.data.url + s + "only=actions"
+    function i() {
+        const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
+        return e.data.url + c + "only=actions"
     }
 
-    function i() {
-        B("GET", o(), function(s) {
-            r(s)
+    function l() {
+        L("GET", i(), function(c) {
+            r(c)
         })
     }
 
-    function l() {
-        return window[n] = () => i(), t.jsx("div", {
+    function d() {
+        return window[n] = () => l(), t.jsx("div", {
             className: "reloadable",
             id: n,
-            children: a.map(function(s) {
+            children: a.map(function(c) {
                 return t.jsx(_, {
-                    data: s,
+                    data: c,
                     default: !0
                 }, Math.random())
             })
         })
     }
-    return l()
+    return d()
 }
 
-function Je(e) {
+function $e(e) {
     function n() {
-        const a = {
-                display: "flex",
-                justifyContent: "space-between",
-                alignItems: "baseline"
-            },
-            r = {
-                margin: 0
-            };
-        return t.jsxs("div", {
-            style: a,
+        return W(`
+      .object-title {
+        display: flex;
+        justify-content: space-between;
+        align-items: baseline;
+      }
+      .object-title h1 {
+          margin: 0;
+          color: ${k.colors.primary};
+      }
+    `), t.jsxs("div", {
+            className: "object-title",
             children: [e.data.title && t.jsx("h1", {
-                style: r,
-                "data-label": T(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
-            }), t.jsx($e, {
+            }), t.jsx(Ve, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
-function Se(e) {
+function ke(e) {
+    W(`
+      .fieldset-title {
+        display: flex;
+        justify-content: space-between;
+        align-items: baseline;
+      }
+      .fieldset-title h2 {
+          margin: 0
+      }
+    `);
+
     function n() {
-        const a = {
-                display: "flex",
-                justifyContent: "space-between",
-                alignItems: "baseline"
-            },
-            r = {
-                marginBottom: 0,
-                marginTop: 15
-            };
         return t.jsxs("div", {
-            style: a,
+            className: "fieldset-title",
             children: [e.data.title && t.jsx("h2", {
-                style: r,
-                "data-label": T(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
-                children: e.data.actions.map(function(o) {
+                children: e.data.actions.map(function(a) {
                     return t.jsx(_, {
-                        data: o,
+                        data: a,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
 }
 
-function Ye(e) {
+function Je(e) {
     function n() {
-        return t.jsx(Je, {
+        return t.jsx($e, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(o, i) {
-            return t.jsx(p, {
-                data: o
+        return e.data.data.map(function(i, l) {
+            return t.jsx(x, {
+                data: i
             }, Math.random())
         })
     }
 
     function r() {
-        return t.jsxs(t.Fragment, {
+        return t.jsxs("div", {
+            className: "object-viewer",
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Qe(e) {
+function Ye(e) {
     function n() {
-        return t.jsx(Se, {
+        return t.jsx(ke, {
             data: e.data
         })
     }
 
     function a() {
-        const o = {
+        const i = {
             backgroundColor: "white"
         };
-        return e.data.data.map(function(i, l) {
+        return e.data.data.map(function(l, d) {
             return t.jsx("div", {
-                style: o,
-                children: t.jsx(p, {
-                    data: i
+                style: i,
+                children: t.jsx(x, {
+                    data: l
                 }, Math.random())
             })
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Xe(e) {
+function Qe(e) {
     const [n, a] = I.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
-            children: e.data.map(function(o, i) {
-                return t.jsx(N, {
-                    href: o.url,
+            children: e.data.map(function(i, l) {
+                return t.jsx(O, {
+                    href: i.url,
                     style: {
                         padding: 5,
-                        fontWeight: n == i ? "bold" : "normal",
-                        borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
+                        fontWeight: n == l ? "bold" : "normal",
+                        borderBottom: n == l ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
-                    onClick: function(l) {
-                        l.preventDefault(), a(i), e.loadContent(o.url)
+                    onClick: function(d) {
+                        d.preventDefault(), a(l), e.loadContent(i.url)
                     },
-                    dataLabel: T(o.title),
-                    children: o.title
+                    dataLabel: M(i.title),
+                    children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
-function Ke(e) {
+function Xe(e) {
     var n = Math.random();
     const [a, r] = I.useState(e.data.data[0]);
 
-    function o() {
+    function i() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": T(e.data.title),
+            "data-label": M(e.data.title),
             children: e.data.title
         })
     }
 
-    function i() {
-        return t.jsx(Xe, {
+    function l() {
+        return t.jsx(Qe, {
             data: e.data.data,
-            loadContent: c
+            loadContent: s
         })
     }
 
-    function l() {
-        var d = {
+    function d() {
+        var o = {
             ...a
         };
-        d.title = null;
+        o.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
-            children: t.jsx(p, {
-                data: d
+            children: t.jsx(x, {
+                data: o
             }, Math.random())
         })
     }
 
-    function s() {
-        const d = {
+    function c() {
+        const o = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: d
+            style: o
         })
     }
 
-    function c(d) {
-        B("GET", d, function(h) {
+    function s(o) {
+        L("GET", o, function(h) {
             r(h)
         })
     }
 
     function u() {
-        return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
+        return window[n] = () => s(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [o(), i(), l(), s()]
+            children: [i(), l(), d(), c()]
         })
     }
     return u()
 }
 
-function Ze() {
+function Ke() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
 function R({
     id: e,
     onClick: n,
     icon: a,
     label: r,
-    display: o,
-    primary: i,
-    compact: l,
-    spin: s
+    display: i,
+    primary: l,
+    compact: d,
+    spin: c
 }) {
-    function c() {
-        return a ? l || !r ? t.jsx(j, {
+    function s() {
+        return a ? d || !r ? t.jsx(S, {
             icon: a
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(Ae, {
+            children: [t.jsx(Be, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(j, {
+            }), t.jsx(S, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const d = {
+        const o = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
-            display: o || "block",
+            display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return i ? (d.backgroundColor = S.colors.primary, d.color = "white") : (d.border = "solid 1px " + S.colors.primary, d.color = S.colors.primary), t.jsx("a", {
+        return l ? (o.backgroundColor = k.colors.primary, o.color = "white") : (o.border = "solid 1px " + k.colors.primary, o.color = k.colors.primary), t.jsx("a", {
             id: e,
-            style: d,
-            "data-label": T(r || a),
+            style: o,
+            "data-label": M(r || a),
             onClick: h => {
-                h.preventDefault(), a && s && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
+                h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
-            children: c()
+            children: s()
         })
     }
     return u()
 }
-const et = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
-    Q = {
+
+function Ze(e) {
+    return t.jsx("img", {
+        src: e.data.src,
+        style: {
+            width: "100%"
+        }
+    })
+}
+
+function et(e) {
+    const n = {
+        width: "100%",
+        textAlign: "center"
+    };
+    return t.jsx("div", {
+        style: n,
+        children: t.jsx("img", {
+            src: e.data.src || e.data.placeholder,
+            style: {
+                width: e.data.width,
+                height: e.data.height,
+                borderRadius: e.data.round ? "50%" : 0
+            }
+        })
+    })
+}
+
+function tt(e) {
+    return e.data.latitude && e.data.longitude && t.jsx("iframe", {
+        width: e.data.width || "100%",
+        height: e.data.height || "400px",
+        id: "gmap_canvas",
+        src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
+        frameBorder: "0",
+        scrolling: "no",
+        marginHeight: "0",
+        marginWidth: "0"
+    })
+}
+
+function nt(e) {
+    function n(l) {
+        return e.data.icon ? l.done ? t.jsx(S, {
+            style: {
+                marginTop: 6
+            },
+            icon: e.data.icon
+        }) : t.jsx("span", {
+            children: " "
+        }) : t.jsx("div", {
+            style: {
+                marginTop: 6
+            },
+            children: l.number
+        })
+    }
+
+    function a(l) {
+        return {
+            border: "3px solid " + k.colors.primary,
+            borderRadius: "50%",
+            background: l.done ? k.colors.primary : "white",
+            color: l.done ? "white" : k.colors.primary,
+            textAlign: "center",
+            width: 50,
+            height: 50,
+            margin: "auto",
+            fontSize: "1.5rem"
+        }
+    }
+
+    function r(l) {
+        return {
+            listStyleType: "none",
+            display: "flex",
+            justifyContent: "center",
+            minWidth: l.length * 100
+        }
+    }
+
+    function i() {
+        const l = {
+                width: "100%",
+                margin: "auto",
+                overflowX: "auto",
+                "&::WebkitScrollbar": {
+                    width: 0
+                }
+            },
+            d = {
+                width: 100,
+                marginWidth: 100,
+                textAlign: "center"
+            },
+            c = {
+                position: "relative",
+                borderBottom: "2px solid #1151b3",
+                top: -28,
+                width: 45,
+                left: 77
+            };
+        return t.jsx("div", {
+            children: t.jsx("div", {
+                style: l,
+                children: t.jsx("ul", {
+                    style: r(e.data.steps),
+                    children: e.data.steps.map((s, u) => t.jsxs("li", {
+                        style: d,
+                        children: [t.jsx("div", {
+                            style: a(s),
+                            children: n(s)
+                        }), u < e.data.steps.length - 1 && t.jsx("div", {
+                            style: c
+                        }), t.jsx("div", {
+                            children: s.name
+                        })]
+                    }, Math.random()))
+                })
+            })
+        })
+    }
+    return i()
+}
+
+function at(e) {
+    function n() {
+        const a = {
+                display: "inline-block",
+                width: "100%",
+                backgroundColor: "#DDD",
+                borderRadius: 5,
+                marginTop: 5
+            },
+            r = {
+                marginLeft: 10
+            },
+            i = {
+                display: "block",
+                paddingTop: 2,
+                paddingBottom: 2,
+                color: "white",
+                borderRadius: 5,
+                width: e.data.value + "%",
+                backgroundColor: k.colors[e.data.style]
+            };
+        return t.jsx("span", {
+            style: a,
+            children: t.jsx("span", {
+                style: i,
+                children: t.jsxs("span", {
+                    style: r,
+                    children: [e.data.value, "%"]
+                })
+            })
+        })
+    }
+    return n()
+}
+
+function rt(e) {
+    function n() {
+        return e.data.color = k.colors[e.data.style], t.jsx(Se, {
+            data: e.data
+        })
+    }
+    return n()
+}
+
+function Se(e) {
+    function n() {
+        const a = {
+            color: "white",
+            width: "fit-content",
+            borderRadius: 0,
+            textWrap: "nowrap",
+            padding: 10,
+            whiteSpace: "nowrap",
+            backgroundColor: e.data.color,
+            display: "inline-flex",
+            border: "solid 3px white"
+        };
+        return t.jsxs("div", {
+            style: a,
+            children: [e.data.icon && t.jsx(S, {
+                icon: e.data.icon,
+                style: {
+                    marginRight: 5
+                }
+            }), e.data.label]
+        })
+    }
+    return n()
+}
+
+function it(e) {
+    function n() {
+        const a = {
+                padding: 20,
+                marginLeft: -20,
+                marginRight: -20,
+                textAlign: "center",
+                backgroundColor: "#f8f8f8"
+            },
+            r = {
+                padding: 20,
+                display: "inline-flex",
+                flexDirection: "column",
+                width: 250,
+                height: 250,
+                backgroundColor: "white",
+                boxShadow: "0px 15px 10px -15px #DDD",
+                margin: 10,
+                textDecoration: "none"
+            },
+            i = {
+                marginTop: 30,
+                fontSize: "3rem",
+                color: k.colors.auxiliary
+            },
+            l = {
+                marginTop: 40,
+                fontWeight: "bold",
+                fontSize: "1.2rem",
+                textTransform: "uppercase",
+                height: 70,
+                color: k.colors.primary
+            };
+        return e.data.items.length ? t.jsxs("div", {
+            style: a,
+            children: [t.jsx("h2", {
+                "data-label": M(e.data.title),
+                style: {
+                    color: k.colors.primary
+                },
+                children: e.data.title
+            }), t.jsx("div", {
+                children: e.data.items.map(d => t.jsxs(O, {
+                    href: d.url,
+                    style: r,
+                    dataLabel: d.label,
+                    children: [t.jsx("div", {
+                        children: t.jsx(S, {
+                            style: i,
+                            icon: d.icon
+                        })
+                    }), t.jsx("div", {
+                        style: l,
+                        children: d.label
+                    })]
+                }, Math.random()))
+            })]
+        }) : null
+    }
+    return n()
+}
+
+function lt(e) {
+    function n() {
+        return t.jsx("div", {
+            style: {
+                backgroundColor: "black",
+                color: "white",
+                padding: "10px",
+                minHeight: "300px",
+                fontFamily: "monospace, monospace",
+                marginBottom: "30px"
+            },
+            children: e.data.output.split(`
+`).map(a => t.jsx("div", {
+                children: a
+            }, Math.random()))
+        })
+    }
+    return n()
+}
+
+function ot(e) {
+    function n() {
+        return e.data.url ? t.jsx(O, {
+            href: e.data.url,
+            imodal: !!e.data.modal,
+            children: e.data.icon ? t.jsx(S, {
+                icon: e.data.icon
+            }) : e.data.url
+        }) : t.jsx("span", {
+            children: "-"
+        })
+    }
+    return n()
+}
+
+function dt(e) {
+    function n() {
+        return t.jsx("iframe", {
+            src: e.data.url,
+            width: "100%",
+            height: 500,
+            style: {
+                border: 0
+            }
+        })
+    }
+    return n()
+}
+
+function st(e) {
+    const n = Math.random();
+    I.useEffect(() => {
+        new QRCode(document.getElementById(n), {
+            text: e.data.text,
+            width: 128,
+            height: 128,
+            colorDark: "#333333",
+            colorLight: "#ffffff",
+            correctLevel: QRCode.CorrectLevel.H
+        })
+    }, []);
+
+    function a() {
+        return t.jsx("div", {
+            id: n
+        })
+    }
+    return a()
+}
+
+function ct(e) {
+    function n() {
+        const a = {
+                color: "white",
+                backgroundColor: k.colors.highlight,
+                margin: -20,
+                textAlign: "center",
+                paddingTop: 20,
+                paddingBottom: 70
+            },
+            r = {
+                fontSize: "4rem",
+                fontWeight: "bold",
+                marginTop: 25
+            },
+            i = {
+                fontSize: "1.2rem",
+                maxWidth: 200,
+                margin: "auto"
+            };
+        if (e.data) return t.jsxs("div", {
+            className: "indicators",
+            style: a,
+            children: [t.jsx("h1", {
+                "data-label": M(e.data.title),
+                children: e.data.title
+            }), t.jsx(P, {
+                width: 300,
+                children: e.data.items.map(l => t.jsxs("div", {
+                    children: [t.jsx("div", {
+                        style: r,
+                        children: F(l.value)
+                    }), t.jsx("div", {
+                        style: i,
+                        children: l.name
+                    })]
+                }, Math.random()))
+            }, Math.random()), t.jsx("div", {
+                className: "actions",
+                children: e.data.actions.map(l => t.jsx(O, {
+                    href: A(l.url),
+                    label: l.label,
+                    modal: l.modal,
+                    children: l.label
+                }, Math.random()))
+            })]
+        })
+    }
+    return n()
+}
+
+function ut(e) {
+    function n() {
+        return t.jsx(P, {
+            width: 400,
+            children: e.data.items.map((a, r) => t.jsx("div", {
+                children: t.jsx(x, {
+                    data: a
+                })
+            }, Math.random()))
+        })
+    }
+    return n()
+}
+
+function ht(e) {
+    function n() {
+        return t.jsxs("div", {
+            children: [t.jsx("h2", {
+                children: e.data.title
+            }), t.jsx("div", {
+                style: {
+                    fontSize: "12rem",
+                    textAlign: "center",
+                    color: "#5470c6"
+                },
+                children: e.data.value
+            })]
+        })
+    }
+    return n()
+}
+
+function Ce(e) {
+    const n = Math.random();
+    var a = !1;
+    const r = "rgb(219, 237, 255)",
+        i = "rgb(89, 154, 242)",
+        l = "rgb(246, 123, 135)",
+        d = [],
+        c = [];
+
+    function s(v) {
+        return e.data.readonly ? v == null ? r : i : v == null ? r : v.text == null ? i : l
+    }
+
+    function u(v) {
+        a = !0, v.preventDefault()
+    }
+
+    function o(v) {
+        a = !1, document.getElementById("input" + n).value = JSON.stringify({
+            select: d,
+            deselect: c
+        })
+    }
+
+    function h(v) {
+        e.data.readonly || e.data.single_selection && f().length > 0 && v.target.style.backgroundColor != i || a && v.target.style.backgroundColor != l && (v.target.style.backgroundColor == r ? (v.target.style.backgroundColor = i, console.log("MARCOU", v.target.dataset.day, v.target.dataset.time), d.push([v.target.dataset.day, v.target.dataset.time])) : (v.target.style.backgroundColor = r, console.log("DEMARCOU", v.target.dataset.day, v.target.dataset.time), c.push([v.target.dataset.day, v.target.dataset.time])))
+    }
+
+    function f() {
+        const v = [];
+        return document.getElementById(n).querySelectorAll("td").forEach(function(B) {
+            B.style.backgroundColor == i && v.push(B.dataset.day, B.dataset.time)
+        }), v
+    }
+
+    function w() {
+        const v = {
+                overflowX: "auto"
+            },
+            B = {
+                width: "100%",
+                borderSpacing: 0,
+                borderCollapse: "collapse",
+                marginTop: 15,
+                marginBottom: 15
+            },
+            g = {
+                border: "solid 4px white"
+            };
+        return t.jsxs("div", {
+            id: n,
+            style: v,
+            children: [t.jsx("input", {
+                id: "input" + n,
+                type: "hidden",
+                name: e.data.input_name
+            }), t.jsxs("table", {
+                style: B,
+                onMouseDown: u,
+                onMouseUp: o,
+                children: [t.jsx("thead", {
+                    children: t.jsx("tr", {
+                        children: e.data.matrix[0].map(function(j) {
+                            return t.jsx("th", {
+                                className: "bold",
+                                style: g,
+                                children: j.text
+                            }, Math.random())
+                        })
+                    })
+                }), t.jsx("tbody", {
+                    children: e.data.matrix.map(function(j, y) {
+                        if (y > 0) return t.jsx("tr", {
+                            children: j.map(function(D, b) {
+                                if (b == 0) return t.jsx("th", {
+                                    className: "bold",
+                                    align: "center",
+                                    style: g,
+                                    children: D.text
+                                }, Math.random());
+                                {
+                                    const C = {
+                                        backgroundColor: s(D),
+                                        border: "solid 4px white"
+                                    };
+                                    return t.jsx("td", {
+                                        align: "center",
+                                        style: C,
+                                        onMouseDown: h,
+                                        onMouseLeave: h,
+                                        onMouseUp: h,
+                                        "data-day": e.data.matrix[0][b].text,
+                                        "data-time": j[0].text,
+                                        children: D && D.text && t.jsx(mt, {
+                                            text: D.text,
+                                            children: t.jsx(S, {
+                                                icon: "stethoscope",
+                                                style: {
+                                                    color: "white",
+                                                    cursor: "help"
+                                                }
+                                            })
+                                        })
+                                    }, Math.random())
+                                }
+                            })
+                        }, Math.random())
+                    })
+                })]
+            })]
+        })
+    }
+    return w()
+}
+
+function mt(e) {
+    function n() {
+        return W(`
+      .tooltip {
+        position: relative;
+        display: inline-block;
+      }
+      .tooltip .tooltiptext {
+        visibility: hidden;
+        width: 220px;
+        background-color: ${k.colors.highlight};
+        color: #fff;
+        text-align: center;
+        border-radius: 6px;
+        padding: 5px 0;
+        position: absolute;
+        z-index: 1;
+        bottom: 150%;
+        left: 50%;
+        margin-left: -60px;
+        z-index: 9999;
+      }
+      .tooltip:hover .tooltiptext {
+        visibility: visible;
+      }
+    `), t.jsxs("div", {
+            className: "tooltip",
+            children: [e.children, t.jsx("div", {
+                className: "tooltiptext",
+                children: F(e.text)
+            })]
+        })
+    }
+    return n()
+}
+const ft = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
+    $ = {
         padding: 15,
         border: "solid 1px #d9d9d9",
-        borderRadius: 5
+        borderRadius: 5,
+        backgroundColor: "white"
     };
 
-function ie(e) {
+function gt(e) {
+    const n = new FormData(e);
+    for (let [a, r] of Array.from(n.entries())) {
+        const i = e[a];
+        (r === "" || !(i.tagName == "SELECT" || i.tagName == null)) && n.delete(a)
+    }
+    return new URLSearchParams(n).toString()
+}
+
+function Y(e, n) {
+    const a = e.indexOf("?") < 0 ? "?" : "&",
+        r = gt(n);
+    return e = e + (r ? a + r : ""), e
+}
+
+function re(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
-function ee(e, n) {
-    const a = e.closest("form"),
-        r = new FormData(a),
-        o = n.indexOf("?") >= 0 ? "&" : "?";
-    n += o + new URLSearchParams(r).toString(), B("GET", n, Ce)
+function J(e, n) {
+    L("GET", Y(n, e.closest("form")), Me)
 }
 
-function tt(e) {
+function xt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
         a && (a.style.display = "none")
     }
 }
 
-function nt(e) {
+function yt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "block");
         var a = document.querySelector(".form-group." + e);
-        a && (a.style.display = "flex")
+        a && (a.style.display = "block")
     }
 }
 
-function at(e, n) {
+function vt(e) {
+    window["reload-" + e + "-field"]()
+}
+
+function bt(e, n) {
     var a = document.querySelector(".form-group." + e),
         r = a.querySelector('*[name="' + e + '"]');
     if (r.tagName == "INPUT") r.value = n;
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
             }
         }));
         else
-            for (var o = 0; o < r.options.length; o++)
-                if (r.options[o].value == n) {
-                    r.selectedIndex = o;
+            for (var i = 0; i < r.options.length; i++)
+                if (r.options[i].value == n) {
+                    r.selectedIndex = i;
                     break
                 }
     }
 }
 
-function Ce(e) {
+function Me(e) {
     if (e) {
-        for (var n = 0; n < e.hide.length; n++) tt(e.hide[n]);
-        for (var n = 0; n < e.show.length; n++) nt(e.show[n]);
-        for (var a in e.set) at(a, e.set[a])
+        for (var n = 0; n < e.hide.length; n++) xt(e.hide[n]);
+        for (var n = 0; n < e.show.length; n++) yt(e.show[n]);
+        for (var n = 0; n < e.reload.length; n++) vt(e.reload[n]);
+        for (var a in e.set) bt(a, e.set[a])
     }
 }
 
-function rt(e) {
+function wt(e) {
     function n() {
         const a = {
-            color: S.colors.info,
-            backgroundColor: S.background.info,
+            color: k.colors.info,
+            backgroundColor: k.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(j, {
+                children: [t.jsx(S, {
                     icon: "circle-check",
                     style: {
-                        color: S.colors.info,
+                        color: k.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function it(e) {
+function pt(e) {
     function n() {
         const a = {
             color: "white",
             display: "none",
             backgroundColor: "#e52207",
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
             className: "error",
-            children: [t.jsx(j, {
+            children: [t.jsx(S, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
     return n()
 }
 
-function lt(e) {
+function jt(e) {
     function n() {
         const a = {
             marginTop: 2,
             marginBottom: 2,
             fontStyle: "italic"
         };
         return t.jsx("div", {
@@ -1319,889 +1984,919 @@
                 children: e.text
             })
         })
     }
     return n()
 }
 
-function K(e) {
+function Z(e) {
     const n = e.data.name + Math.random();
 
     function a() {
-        const s = {
+        const c = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
-        return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0), t.jsxs("div", {
-            style: s,
-            children: [t.jsx("label", {
-                className: e.data.required ? "bold" : "",
-                children: e.data.label
+        return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0, e.data.action.urlfunc = function() {
+            return Y(e.data.action.url, document.getElementById(n).closest("form"))
+        }), t.jsxs("div", {
+            style: c,
+            children: [t.jsxs("label", {
+                className: "bold",
+                children: [e.data.label, " ", e.data.required ? "*" : ""]
             }), e.data.action && t.jsx(_, {
                 data: e.data.action,
                 style: {
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), et.indexOf(e.data.type) >= 0 ? t.jsx(ge, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), ft.indexOf(e.data.type) >= 0 ? t.jsx(xe, {
             data: e.data
         }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
             data: e.data
-        }) : t.jsx(le, {
+        }) : t.jsx(ie, {
             data: e.data
-        }) : t.jsx(st, {
+        }) : t.jsx(Ct, {
             data: e.data
         }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
             data: e.data
-        }) : t.jsx(le, {
+        }) : t.jsx(ie, {
             data: e.data
-        }) : t.jsx(Te, {
+        }) : t.jsx(Ee, {
             data: e.data
-        }) : e.data.type == "decimal" ? t.jsx(ge, {
+        }) : e.data.type == "decimal" ? t.jsx(xe, {
             data: e.data
-        }) : e.data.type == "boolean" ? t.jsx(dt, {
+        }) : e.data.type == "boolean" ? t.jsx(St, {
             data: e.data
-        }) : e.data.type == "textarea" ? t.jsx(ot, {
+        }) : e.data.type == "textarea" ? t.jsx(kt, {
             data: e.data
-        }) : t.jsx("span", {
+        }) : e.data.type == "scheduler" ? (e.data.scheduler.input_name = e.data.name, t.jsx(Ce, {
+            data: e.data.scheduler
+        })) : t.jsx("span", {
             children: e.data.name
         })
     }
 
-    function o() {
+    function i() {
         return t.jsx("div", {
-            children: t.jsx(it, {
+            children: t.jsx(pt, {
                 id: e.data.name + "_error"
             })
         })
     }
 
-    function i() {
-        return e.data.help_text && t.jsx(lt, {
+    function l() {
+        return e.data.help_text && t.jsx(jt, {
             text: e.data.help_text
         })
     }
 
-    function l() {
-        const s = {
+    function d() {
+        const c = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
             padding: 5,
             width: "calc(100%-5px)"
         };
         return t.jsxs("div", {
             id: n,
-            style: s,
-            children: [a(), r(), i(), o()]
+            style: c,
+            children: [a(), r(), l(), i()]
         })
     }
-    return l()
+    return d()
 }
 
-function ge(e) {
+function xe(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), I.useEffect(() => {
-        function l(u, d, h) {
+        function d(u, o, h) {
             var f = h.target,
                 w = f.value.replace(/\D/g, ""),
-                M = f.value.length > d ? 1 : 0;
-            VMasker(f).unMask(), VMasker(f).maskPattern(u[M]), f.value = VMasker.toPattern(w, u[M])
+                v = f.value.length > o ? 1 : 0;
+            VMasker(f).unMask(), VMasker(f).maskPattern(u[v]), f.value = VMasker.toPattern(w, u[v])
         }
         if (e.data.mask) {
-            var s = document.getElementById(a);
-            if (e.data.mask == "decimal") VMasker(s).maskMoney({
+            var c = document.getElementById(a);
+            if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
             });
             else if (e.data.mask.indexOf("|") > 0) {
-                var c = e.data.mask.split("|");
-                VMasker(s).maskPattern(c[0]), s.addEventListener("input", l.bind(void 0, c, 14), !1)
-            } else VMasker(s).maskPattern(e.data.mask)
+                var s = e.data.mask.split("|");
+                VMasker(c).maskPattern(s[0]), c.addEventListener("input", d.bind(void 0, s, 14), !1)
+            } else VMasker(c).maskPattern(e.data.mask)
         }
     }, []);
 
-    function r(l) {
-        ee(l.target, e.data.onchange)
+    function r(d) {
+        J(d.target, e.data.onchange)
     }
 
-    function o(l) {
-        if (e.data.type == "file" && l.target.files) {
-            let c = l.target.files[0];
-            var s = new FileReader;
-            s.onload = function(u) {
-                if (ie(c.name)) {
+    function i(d) {
+        if (e.data.type == "file" && d.target.files) {
+            let s = d.target.files[0];
+            var c = new FileReader;
+            c.onload = function(u) {
+                if (re(s.name)) {
                     const w = "display" + a;
-                    var d = document.createElement("img");
-                    d.id = l.target.id + "img", d.style.width = "200px", d.style.display = "block", d.style.margin = "auto", d.style.marginTop = "20px", d.onload = function(M) {
-                        const D = e.data.width > e.data.height ? e.data.width / d.width : e.data.height / d.height;
-                        var y = document.createElement("canvas");
-                        const k = y.getContext("2d");
-                        y.height = y.width * (d.height / d.width);
-                        const x = document.createElement("canvas"),
-                            L = x.getContext("2d");
-                        x.width = d.width * D, x.height = d.height * D, L.drawImage(d, 0, 0, x.width, x.height), k.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, y.width, y.height), x.toBlob(function(m) {
-                            const v = new DataTransfer;
-                            v.items.add(new File([m], c.name)), l.target.files = v.files
+                    var o = document.createElement("img");
+                    o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(v) {
+                        const B = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                        var g = document.createElement("canvas");
+                        const j = g.getContext("2d");
+                        g.height = g.width * (o.height / o.width);
+                        const y = document.createElement("canvas"),
+                            D = y.getContext("2d");
+                        y.width = o.width * B, y.height = o.height * B, D.drawImage(o, 0, 0, y.width, y.height), j.drawImage(y, 0, 0, y.width * B, y.height * B, 0, 0, g.width, g.height), y.toBlob(function(C) {
+                            const T = new DataTransfer;
+                            T.items.add(new File([C], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
-                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(d), l.target.parentNode.appendChild(b)
-                    }, d.src = u.target.result
+                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
+                    }, o.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
-                var f = c.size / 1024;
-                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = c.name + " / " + f, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
-            }, s.readAsDataURL(c)
+                var f = s.size / 1024;
+                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + f, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
+            }, c.readAsDataURL(s)
         }
     }
 
-    function i() {
-        var l = e.data.type;
-        if (l == "datetime" && (l = "datetime-regional"), l == "decimal" && (l = "text"), l == "file") {
+    function l() {
+        var d = e.data.type;
+        if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
             const u = {
                 alignContent: "center",
                 minHeight: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
-            var s = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (s = e.data.extensions.map(d => "." + d).join(", ")), t.jsxs(t.Fragment, {
+            var c = null;
+            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(o => "." + o).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(j, {
+                        children: t.jsx(S, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: S.colors.primary
+                                color: k.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
-                        children: [e.data.value && ie(e.data.value) && t.jsx("div", {
+                        children: [e.data.value && re(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: t.jsx("img", {
                                 src: e.data.value,
                                 height: 50
                             })
-                        }), e.data.value && !ie(e.data.value) && t.jsx("div", {
+                        }), e.data.value && !re(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(d => "." + d).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(o => "." + o).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
                         children: t.jsx(R, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
-                    type: l,
+                    type: d,
                     name: e.data.name,
                     id: a,
-                    "data-label": T(e.data.label),
+                    "data-label": M(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
-                    onChange: o,
+                    onChange: i,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
-                    accept: s
+                    accept: c
                 })]
             })
         } else {
-            var c = Q;
-            return l == "color" && (c = {
-                ...Q
-            }, c.width = "100%", c.backgroundColor = "white", c.height = 47.5), t.jsx("input", {
+            var s = $;
+            return d == "color" && (s = {
+                ...$
+            }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
-                type: l,
+                type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": T(e.data.label),
+                "data-label": M(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
-                onChange: o,
-                style: c
+                onChange: i,
+                style: s
             })
         }
     }
-    return i()
+    return l()
 }
 
-function Te(e) {
+function Ee(e) {
     var n = [];
-    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, m) {
+    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, C) {
         n.push({
             id: b.id,
             value: b.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
-        o = Array.isArray(e.data.value),
-        [i, l] = I.useState(!1),
-        [s, c] = I.useState(null);
+        i = Array.isArray(e.data.value),
+        [l, d] = I.useState(!1),
+        [c, s] = I.useState(null);
     var u = !1;
-    let d;
+    let o;
     I.useEffect(() => {
-        k(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
-            k(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+        j(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
+            j(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
         const b = document.getElementById(a);
-        if (o) {
-            const m = {
+        if (i) {
+            const C = {
                     padding: 5,
                     display: "inline"
                 },
-                v = {
+                T = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                g = {
+                m = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((C, E) => t.jsxs("div", {
-                    style: m,
+                children: [b == null && n.map((p, E) => t.jsxs("div", {
+                    style: C,
                     children: [t.jsx("span", {
-                        onClick: () => x(E),
-                        style: v,
-                        children: t.jsx(j, {
+                        onClick: () => y(E),
+                        style: T,
+                        children: t.jsx(S, {
                             icon: "trash-can",
-                            style: g
+                            style: m
                         })
-                    }), C.value]
-                }, Math.random())), b != null && Array.from(b.options).map((C, E) => t.jsxs("div", {
-                    style: m,
+                    }), p.value]
+                }, Math.random())), b != null && Array.from(b.options).map((p, E) => t.jsxs("div", {
+                    style: C,
                     children: [t.jsx("span", {
-                        onClick: () => x(E),
-                        style: v,
-                        children: t.jsx(j, {
+                        onClick: () => y(E),
+                        style: T,
+                        children: t.jsx(S, {
                             icon: "trash-can",
-                            style: g
+                            style: m
                         })
-                    }), C.innerHTML]
+                    }), p.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function f() {
         return t.jsx("select", {
             id: a,
             name: e.data.name,
-            multiple: o,
+            multiple: i,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
     function w() {
         const b = {
-                ...Q,
+                ...$,
                 ...e.style || {}
             },
-            m = {
+            C = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
-                overflowY: "auto"
+                overflowY: "auto",
+                zIndex: 99999
             };
-        m.position = "absolute", m.backgroundColor = "white";
-        const v = document.getElementById(r);
-        if (e.data.icon && (b.paddingLeft = 30), v) {
-            let A = null,
-                z = v,
-                V = null;
-            for (; !V && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (V = z);
-            A = V;
-            const P = v.getBoundingClientRect();
-            var g = P.top + P.height,
-                C = P.left;
-            if (A) {
-                const $ = A.getBoundingClientRect();
-                g = g - $.top, C = C - $.left
-            } else g += window.scrollY, C += window.scrollX;
-            m.width = P.width, m.top = g, m.left = C
+        C.position = "absolute", C.backgroundColor = "white";
+        const T = document.getElementById(r);
+        if (e.data.icon && (b.paddingLeft = 30), T) {
+            let q = null,
+                Q = T,
+                ae = null;
+            for (; !ae && (Q = Q.parentElement) instanceof HTMLElement;) Q.matches("dialog") && (ae = Q);
+            q = ae;
+            const X = T.getBoundingClientRect();
+            var m = X.top + X.height,
+                p = X.left;
+            if (q) {
+                const fe = q.getBoundingClientRect();
+                m = m - fe.top, p = p - fe.left
+            } else m += window.scrollY, p += window.scrollX;
+            C.width = X.width, C.top = m, C.left = p
         }
         const E = {
                 cursor: "pointer",
                 padding: 10
             },
-            ae = !o && n.length > 0 && n[0].value || "";
+            N = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
-            children: [e.data.icon && t.jsx(j, {
+            children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: A => {
-                    A.target.select(), y(A)
+                onFocus: q => {
+                    q.target.select(), g(q)
                 },
-                onChange: y,
-                onMouseLeave: M,
-                onBlur: M,
-                defaultValue: ae,
+                onChange: g,
+                onMouseLeave: v,
+                onBlur: v,
+                defaultValue: N,
                 style: b,
-                "data-label": T(e.data.label)
-            }), s && i && t.jsxs("ul", {
-                style: m,
-                onMouseLeave: D,
-                onMouseEnter: function(A) {
+                "data-label": M(e.data.label)
+            }), c && l && t.jsxs("ul", {
+                style: C,
+                onMouseLeave: B,
+                onMouseEnter: function(q) {
                     u = !0
                 },
-                children: [s.length == 0 && t.jsx("li", {
+                children: [c.length == 0 && t.jsx("li", {
                     style: E,
                     children: "Nenhuma opção encontrada."
-                }), s.map(A => t.jsx("li", {
+                }), c.map(q => t.jsx("li", {
                     onClick: () => {
-                        l(!1), e.onSelect ? e.onSelect(A) : k(A)
+                        d(!1), e.onSelect ? e.onSelect(q) : j(q)
                     },
                     style: E,
                     className: "autocomplete-item",
-                    "data-label": T(A.value),
-                    children: A.value
+                    "data-label": M(q.value),
+                    children: q.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function M(b) {
+    function v(b) {
         u = !1, setTimeout(function() {
-            u || D(b)
+            u || B(b)
         }, 250)
     }
 
-    function D(b) {
-        const m = document.getElementById(a);
-        if (m) {
-            const v = document.getElementById(r);
-            o || m.options.length > 0 && v.value != m.options[0].innerHTML && (m.innerHTML = "", v.value = "", l(!1), e.data.onchange && ee(v, e.data.onchange)), b.target.tagName == "UL" ? l(!1) : u || l(!1)
+    function B(b) {
+        const C = document.getElementById(a);
+        if (C) {
+            const T = document.getElementById(r);
+            i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && J(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
-    function y(b) {
-        clearTimeout(d), d = setTimeout(function() {
-            const m = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            l(!0), B("GET", e.data.choices + m + "term=" + b.target.value, function(g) {
-                c(g)
+    function g(b) {
+        clearTimeout(o), o = setTimeout(function() {
+            const C = b.target.closest("form"),
+                T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
+            d(!0), L("GET", Y(e.data.choices + T + "term=" + b.target.value, C), function(p) {
+                s(p)
             })
         }, 1e3)
     }
 
-    function k(b, m = !1) {
-        const v = document.getElementById(a),
-            g = document.getElementById(r);
-        v.innerHTML == null && (v.innerHTML = ""), Array.isArray(b) ? v.innerHTML = b.map(C => `<option selected value="${C.id}">${C.value}</option>`).join("") : o ? (v.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, g.value = "") : (v.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, g.value = b.value), e.data.onchange && !m && ee(g, e.data.onchange)
+    function j(b, C = !1) {
+        const T = document.getElementById(a),
+            m = document.getElementById(r);
+        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !C && J(m, e.data.onchange)
     }
 
-    function x(b) {
-        const m = document.getElementById(a);
-        var v = Array.from(m.options);
-        m.innerHTML = v.slice(0, b).concat(v.slice(b + 1)).map(g => `<option selected value="${g.value}">${g.innerHTML}</option>`).join(""), c([])
+    function y(b) {
+        const C = document.getElementById(a);
+        var T = Array.from(C.options);
+        C.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(m => `<option selected value="${m.value}">${m.innerHTML}</option>`).join(""), s([])
     }
 
-    function L() {
+    function D() {
         return t.jsxs(t.Fragment, {
             children: [h(), f(), w()]
         })
     }
-    return L()
+    return D()
 }
 
-function ot(e) {
+function kt(e) {
     function n() {
         var a = {
-            ...Q
+            ...$
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": T(e.data.label),
+            "data-label": M(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
 
-function dt(e) {
+function St(e) {
     var n = e.data;
     return n.choices = [{
         id: !0,
         value: "Sim"
     }, {
         id: !1,
         value: "Não"
-    }], t.jsx(le, {
+    }], t.jsx(ie, {
         data: n
     })
 }
 
-function le(e) {
-    var n = Math.random(),
-        a = e.data;
+function ie(e) {
+    const [n, a] = I.useState(e.data.choices);
+    var r = Math.random(),
+        i = e.data;
 
-    function r(s) {
-        return a.value != null ? a.value == s.id ? !0 : a.value.id == s.id : !1
+    function l(u) {
+        return i.value != null ? i.value == u.id ? !0 : i.value.id == u.id : !1
     }
 
-    function o(s) {
-        var c = document.getElementById(s);
-        a.checked && (c.checked = !1), e.data.onchange && ee(c, e.data.onchange)
+    function d(u) {
+        var o = document.getElementById(u);
+        i.checked && (o.checked = !1), e.data.onchange && J(o, e.data.onchange)
     }
 
-    function i(s) {
-        var c = document.getElementById(s);
-        a.checked = c.checked
+    function c(u) {
+        var o = document.getElementById(u);
+        i.checked = o.checked
     }
 
-    function l() {
-        return a.choices.length > 0 ? t.jsx("div", {
-            className: "radio-group",
-            children: a.choices.map((s, c) => s.id && t.jsxs("div", {
+    function s() {
+        return window["reload-" + i.name + "-field"] = function() {
+            L("GET", Y(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(o) {
+                a(o)
+            })
+        }, n.length > 0 ? t.jsx("div", {
+            className: "radio-group " + i.name,
+            children: n.map((u, o) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
                     display: "inline-block",
-                    marginRight: 25
+                    marginRight: 25,
+                    width: window.innerWidth > 800 ? "auto" : "100%"
                 },
                 children: [t.jsx("input", {
-                    id: a.name + n + c,
+                    id: i.name + r + o,
                     type: "radio",
-                    name: a.name,
-                    defaultValue: s.id,
-                    defaultChecked: r(s),
-                    "data-label": T(s.value),
+                    name: i.name,
+                    defaultValue: u.id,
+                    defaultChecked: l(u),
+                    "data-label": M(u.value),
                     onClick: function() {
-                        o(a.name + n + c)
+                        d(i.name + r + o)
                     },
                     onMouseEnter: function() {
-                        i(a.name + n + c)
+                        c(i.name + r + o)
                     }
                 }), t.jsx("label", {
-                    htmlFor: a.name + n + c,
-                    children: s.value
+                    htmlFor: i.name + r + o,
+                    children: u.value
                 })]
-            }, n + c))
-        }) : t.jsx("i", {
-            children: "Nenhuma opção disponível para seleção."
+            }, r + o))
+        }) : t.jsx("div", {
+            className: "radio-group " + i.name,
+            children: t.jsx("i", {
+                children: "Nenhuma opção disponível para seleção."
+            })
         })
     }
-    return l()
+    return s()
 }
 
 function ye(e) {
-    var n = Math.random(),
-        a = e.data;
-
-    function r(i) {
-        var l = !1;
-        if (a.value)
-            for (var s = 0; s < a.value.length; s++) {
-                var c = a.value[s];
-                (c == i.id || c.id == i.id) && (l = !0)
+    const [n, a] = I.useState(e.data.choices);
+    var r = Math.random(),
+        i = e.data;
+
+    function l(s) {
+        var u = !1;
+        if (i.value)
+            for (var o = 0; o < i.value.length; o++) {
+                var h = i.value[o];
+                (h == s.id || h.id == s.id) && (u = !0)
             }
-        return l
+        return u
     }
 
-    function o() {
-        return a.choices.length > 0 ? t.jsx("div", {
-            className: "checkbox-group",
-            children: a.choices.map((i, l) => t.jsxs("div", {
+    function d(s) {
+        e.data.onchange && J(s.target, e.data.onchange)
+    }
+
+    function c() {
+        return window["reload-" + i.name + "-field"] = function() {
+            L("GET", Y(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
+                a(u)
+            })
+        }, n.length > 0 ? t.jsx("div", {
+            className: "checkbox-group " + i.name,
+            children: n.map((s, u) => (s.id || s.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
                     display: "inline-block",
-                    marginRight: 25
+                    marginRight: 25,
+                    width: window.innerWidth > 800 ? "auto" : "100%"
                 },
                 children: [t.jsx("input", {
-                    id: a.name + n + l,
+                    id: i.name + r + u,
                     type: "checkbox",
-                    name: a.name,
-                    defaultValue: i.id,
-                    defaultChecked: r(i),
-                    "data-label": T(i.value)
+                    name: i.name,
+                    onClick: d,
+                    defaultValue: s.id,
+                    defaultChecked: l(s),
+                    "data-label": M(s.value)
                 }), t.jsx("label", {
-                    htmlFor: a.name + n + l,
-                    children: i.value
+                    htmlFor: i.name + r + u,
+                    children: s.value
                 })]
-            }, n + l))
-        }) : t.jsx("i", {
-            children: "Nenhuma opção disponível para seleção."
+            }, r + u))
+        }) : t.jsx("div", {
+            className: "checkbox-group " + i.name,
+            children: t.jsx("i", {
+                children: "Nenhuma opção disponível para seleção."
+            })
         })
     }
-    return o()
+    return c()
 }
 
-function st(e) {
+function Ct(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": T(n.label),
+            "data-label": M(n.label),
             defaultValue: n.value,
-            style: Q,
+            style: $,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
 
-function ct(e) {
+function Mt(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
-    function o() {
+    function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(de, {
+            children: t.jsxs(oe, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
-                    onClick: () => i(!0),
+                    onClick: () => l(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => i(!1),
+                    onClick: () => l(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
-    function i(c) {
+    function l(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            d = document.getElementById("inline-form-" + n),
+            o = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
             f = document.getElementById("hide-" + n);
-        d.style.display = c ? "block" : "none", h.style.display = c ? "none" : "inline", f.style.display = c ? "inline" : "none", c ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
-    function l() {
-        const c = {
+    function d() {
+        const s = {
             display: r.value ? "block" : "none"
         };
-        return e.data.required && (c.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
+        return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
             className: "fieldset-inline-forms",
-            style: c,
+            style: s,
             id: "inline-form-" + n,
             children: e.data.value.map(function(u) {
-                return t.jsx(ce, {
+                return t.jsx(ue, {
                     data: u
                 }, Math.random())
             })
         })
     }
 
-    function s() {
-        const c = {
+    function c() {
+        const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: c,
-                "data-label": T(e.data.label),
+                style: s,
+                "data-label": M(e.data.label),
                 children: e.data.label
-            }), o(), l()]
+            }), i(), d()]
         })
     }
-    return s()
+    return c()
 }
 
-function ut(e) {
+function Et(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(d, h) {
+    function r(o, h) {
         const f = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
             id: "form-" + f + "-" + a,
-            children: [t.jsx(ce, {
-                data: d
+            children: [t.jsx(ue, {
+                data: o
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
-                    onClick: () => i(),
+                    onClick: () => l(),
                     id: "extra-add-" + f + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => l(f),
+                    onClick: () => d(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
-    function o() {
-        const d = s(),
-            h = d.length > 0 ? "none" : "inline";
+    function i() {
+        const o = c(),
+            h = o.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
         for (var f = 0; f < n; f++) {
             var w = document.getElementById("extra-add-" + f + "-");
             w.style.display = "none"
         }
-        if (d.length > 0) {
-            var w = document.getElementById("extra-add-" + d[d.length - 1] + "-");
+        if (o.length > 0) {
+            var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
-    function i() {
-        o();
-        var d = JSON.parse(JSON.stringify(e.data.template));
-        d.fields ? (d.fields.map(function(h) {
+    function l() {
+        i();
+        var o = JSON.parse(JSON.stringify(e.data.template));
+        o.fields ? (o.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
-        }), d.fields[0].value = 0) : d.fieldsets.map(function(h) {
+        }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
             h.fields.map(function(f) {
                 f.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
                 }), f[0].value = 0
             })
-        }), F.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(d, "inline")), setTimeout(o, 100)
+        }), z.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
     }
 
-    function l(d) {
+    function d(o) {
         const h = e.data.template,
-            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + d + "__"),
-            M = document.querySelector("input[name=" + w + "]");
-        parseInt(M.value) == 0 ? M.value = "" : M.value = -parseInt(M.value), document.getElementById("form-" + d + "-" + a).style.display = "none", o()
+            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
+            v = document.querySelector("input[name=" + w + "]");
+        parseInt(v.value) == 0 ? v.value = "" : v.value = -parseInt(v.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
     }
 
-    function s() {
-        for (var d = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && d.push(h);
-        return d
+    function c() {
+        for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
+        return o
     }
 
-    function c() {
+    function s() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(de, {
+            children: t.jsx(oe, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
-                    onClick: () => i(),
+                    onClick: () => l(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const d = {
+        const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: d,
-                "data-label": T(e.data.label),
+                style: o,
+                "data-label": M(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [c(), e.data.value.map(function(h, f) {
+                children: [s(), e.data.value.map(function(h, f) {
                     return r(h, f == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
-function ce(e) {
+function ue(e) {
     I.useEffect(() => {
-        e.data.controls && Ce(e.data.controls)
+        e.data.controls && Me(e.data.controls)
     }, []);
 
     function n(r) {
-        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(ct, {
+        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Mt, {
             data: r
-        }, Math.random()) : t.jsx(ut, {
+        }, Math.random()) : t.jsx(Et, {
             data: r
-        }, Math.random()) : t.jsx(K, {
+        }, Math.random()) : t.jsx(Z, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": T(r.title),
+                    "data-label": M(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
-                }), r.fields.map(o => t.jsx("div", {
-                    children: o.map(i => t.jsx("div", {
-                        className: "form-group " + i.name,
+                }), r.fields.map(i => t.jsx("div", {
+                    children: i.map(l => t.jsx("div", {
+                        className: "form-group " + l.name,
                         style: {
-                            width: 100 / o.length + "%",
-                            display: i.type == "hidden" ? "none" : "inline-block"
+                            width: 100 / i.length + "%",
+                            display: l.type == "hidden" ? "none" : "inline-block"
                         },
-                        children: n(i)
+                        children: n(l)
                     }, Math.random()))
                 }, Math.random()))]
             })
         }, Math.random()))
     }
     return a()
 }
 
-function ht(e) {
+function Tt(e) {
     const n = Math.random();
 
     function a() {
         const h = {
-            margin: 0
+            margin: 0,
+            color: k.colors.primary
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
     function r() {
-        return e.data.info && t.jsx(rt, {
+        return e.data.info && t.jsx(wt, {
             data: {
                 text: e.data.info
             }
         })
     }
 
-    function o() {
+    function i() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(h => t.jsx(p, {
+            children: [e.data.display.map(h => t.jsx(x, {
                 data: h
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
-    function i() {
-        return t.jsx(ce, {
+    function l() {
+        return t.jsx(ue, {
             data: e.data
         })
     }
 
-    function l() {
+    function d() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
             children: [t.jsx(R, {
                 onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
             }), t.jsx(R, {
-                onClick: d,
+                onClick: o,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
     }
 
-    function s() {
+    function c() {
         return t.jsx("div", {
             id: "output",
             style: {
                 marginTop: 30
             }
         })
     }
 
-    function c() {
+    function s() {
         return t.jsxs("form", {
             id: n,
             className: e.data.key,
             action: e.data.url,
             style: {
                 margin: "auto",
                 backgroundColor: "white"
@@ -2209,58 +2904,290 @@
             method: e.data.method,
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 5
                 },
-                children: [a(), r(), o(), i(), l(), s()]
+                children: [a(), r(), i(), l(), d(), c()]
             })]
         })
     }
 
     function u() {
-        J()
+        G()
     }
 
-    function d(h) {
+    function o(h) {
         h.preventDefault();
         var f = e.data.url,
             w = document.getElementById(n),
-            M = new FormData(w);
+            v = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
-            const D = f.indexOf("?") >= 0 ? "&" : "?";
-            f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(M).toString(), M = null
+            const B = f.indexOf("?") >= 0 ? "&" : "?";
+            f = f + B + "form=" + e.data.title + "&" + new URLSearchParams(v).toString(), v = null
         }
-        B(w.method.toUpperCase(), f, function(y) {
-            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), y.type == "response") return J(), Ze(), pe(y);
-            if (y.type == "error") {
-                var k = y.text;
-                console.log(y), Object.keys(y.errors).map(function(x) {
-                    if (x == "__all__") k = y.errors[x];
+        L(w.method.toUpperCase(), f, function(g) {
+            if (w.querySelectorAll(".error").forEach(y => y.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), g.type == "response") return G(), Ke(), we(g);
+            if (g.type == "error") {
+                var j = g.text;
+                console.log(g), Object.keys(g.errors).map(function(y) {
+                    if (y == "__all__") j = g.errors[y];
                     else {
-                        const L = w.querySelector("#" + x + "_error");
-                        L.querySelector("span").innerHTML = y.errors[x], L.style.display = "block"
+                        const D = w.querySelector("#" + y + "_error");
+                        D.querySelector("span").innerHTML = g.errors[y], D.style.display = "block"
                     }
-                }), te(k, !0)
+                }), te(j, !0)
             } else {
-                const x = document.querySelector("#output");
-                x.innerHTML = "", F.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(p, {
-                    data: y
+                const y = document.querySelector("#output");
+                y.innerHTML = "", z.createRoot(y.appendChild(document.createElement("div"))).render(t.jsx(x, {
+                    data: g
                 }))
             }
-        }, M)
+        }, v)
     }
-    return c()
+    return s()
 }
 
-function mt(e) {
+function Dt(e) {
+    W(`
+        .calendar table{
+            width: 100%;
+            border-spacing: 0px;
+            border-collapse: collapse;
+            margin-top: 15px;
+            margin-bottom: 15px;
+        }
+        .calendar .day{
+            margin-left: 17px;
+            text-align: right;
+            padding-right: 2px;
+            padding-top: 2px;
+            float: right;
+            font-size: 0.8rem;
+        }
+        .calendar td{
+            vertical-align: top;
+            width: 14.2%;
+            height: 55px;
+            border: solid 1px #EEE;
+        }
+        .calendar .number{
+            border-radius: 50%;
+            color: white;
+            display: block;
+            width: 30px;
+            height: 30px;
+            margin: auto;
+            cursor: pointer;
+            line-height: 2rem;
+        }
+        .calendar .total{
+            padding: 10px;
+            text-align: center;
+        }
+        .calendar .arrows{
+            display: flex;
+            justify-content: space-between;
+            align-items: baseline;
+        }
+        .calendar h3{
+            margin: 0px;
+        }       
+    `);
+    const n = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+        a = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
+        r = new Date,
+        i = e.data.day ? new Date(e.data.year, e.data.month - 1, e.data.day) : null;
+    for (var l = [
+            [],
+            [],
+            [],
+            [],
+            [],
+            []
+        ], d = e.data.month - 1, c = new Date(e.data.year, e.data.month - 1, 1); c.getDay() > 1;) c.setDate(c.getDate() - 1);
+    for (var s = 0;
+        (c.getMonth() <= d || l[s].length < 7) && (l[s].length == 7 && (s += 1), s != 5);) l[s].push({
+        date: c.getDate(),
+        total: e.data.total[c.toLocaleDateString("pt-BR")],
+        today: c.getDate() === r.getDate(),
+        selected: i ? c.getDate() == i.getDate() : !1
+    }), c.setDate(c.getDate() + 1);
+
+    function u() {
+        return t.jsxs("div", {
+            className: "calendar",
+            children: [t.jsxs("div", {
+                className: "arrows",
+                children: [t.jsx("div", {
+                    children: t.jsx(ge, {
+                        default: !0,
+                        icon: "arrow-left",
+                        onClick: () => e.onChange(null, e.data.previous.month, e.data.previous.year)
+                    })
+                }), t.jsxs("div", {
+                    children: [t.jsxs("h3", {
+                        align: "center",
+                        children: [a[e.data.month - 1], " ", e.data.year]
+                    }), e.data.day && t.jsxs("div", {
+                        align: "center",
+                        className: "day",
+                        children: [new Date(e.data.year, e.data.month - 1, e.data.day).toLocaleDateString("pt-BR"), t.jsx(S, {
+                            default: !0,
+                            icon: "x",
+                            onClick: () => e.onChange(null, e.data.month, e.data.year),
+                            style: {
+                                marginLeft: 10,
+                                cursor: "pointer"
+                            }
+                        })]
+                    })]
+                }), t.jsx("div", {
+                    children: t.jsx(ge, {
+                        default: !0,
+                        icon: "arrow-right",
+                        onClick: () => e.onChange(null, e.data.next.month, e.data.next.year)
+                    })
+                })]
+            }), t.jsxs("table", {
+                children: [t.jsx("thead", {
+                    children: t.jsx("tr", {
+                        children: n.map(o => t.jsx("th", {
+                            children: o
+                        }, Math.random()))
+                    })
+                }), t.jsx("tbody", {
+                    children: l.map(o => t.jsx("tr", {
+                        children: o.map(h => t.jsxs("td", {
+                            children: [t.jsx("div", {
+                                className: "day",
+                                children: h.today ? t.jsx("span", {
+                                    style: {
+                                        textDecoration: "underline"
+                                    },
+                                    children: h.date
+                                }) : h.date + h.today
+                            }), h.total && t.jsx("div", {
+                                className: "total",
+                                onClick: () => e.onChange(h.date, e.data.month, e.data.year),
+                                children: t.jsx("div", {
+                                    className: "number",
+                                    style: {
+                                        backgroundColor: k.colors.primary
+                                    },
+                                    children: t.jsx("span", {
+                                        style: {
+                                            textDecoration: h.selected ? "underline" : "normal"
+                                        },
+                                        children: h.total
+                                    })
+                                })
+                            }), !h.total && t.jsx("div", {
+                                className: "total",
+                                children: " "
+                            })]
+                        }, Math.random()))
+                    }, Math.random()))
+                })]
+            })]
+        })
+    }
+    return u()
+}
+
+function It(e) {
+    W(`
+      .paginator{
+        display: flex;
+        justify-content: space-between;
+        line-height: 4rem;
+        align-items: baseline;
+      }
+      .paginator .inline{
+        display: inline;
+        padding-right: 10px;
+      }
+      .paginator select{
+        margin-left: 10px;
+        margin-right: 10px;
+        height: 2.5rem;
+        padding-left: 5px;
+        padding-right: 5px;
+        text-align: center;
+      }
+    `);
+
+    function n() {
+        return e.data.page.total > 1 && t.jsxs("div", {
+            className: "paginator",
+            children: [t.jsxs("div", {
+                children: [window.innerWidth > 800 && t.jsxs("div", {
+                    className: "inline",
+                    children: ["Exibir", t.jsx("select", {
+                        name: "page_size",
+                        onChange: () => e.onChange(1),
+                        value: e.data.page.size,
+                        children: e.data.page.sizes.map(function(a) {
+                            return t.jsx("option", {
+                                children: a
+                            }, Math.random())
+                        })
+                    })]
+                }), window.innerWidth > 800 && t.jsx("div", {
+                    className: "inline",
+                    children: "|"
+                }), t.jsxs("div", {
+                    className: "inline",
+                    children: [e.data.start, " - ", e.data.end, " de ", e.total]
+                })]
+            }), t.jsx("div", {
+                children: t.jsxs("div", {
+                    className: "inline",
+                    children: [t.jsx("span", {
+                        children: "Página"
+                    }), t.jsx("input", {
+                        type: "text",
+                        name: "page",
+                        defaultValue: e.data.page.current,
+                        style: {
+                            width: 30,
+                            marginLeft: 10,
+                            marginRight: 10,
+                            height: "2rem",
+                            textAlign: "center"
+                        },
+                        onKeyDown: function(a) {
+                            a.key == "Enter" && (a.preventDefault(), e.onChange(a.target.value < 0 ? 1 : Math.min(a.target.value, e.data.page.total)))
+                        }
+                    }), t.jsx("div", {
+                        className: "inline",
+                        children: "|"
+                    }), e.data.page.previous && t.jsx(R, {
+                        icon: "chevron-left",
+                        default: !0,
+                        display: "inline",
+                        onClick: () => e.onChange(e.data.page.previous)
+                    }), e.data.page.next && t.jsx(R, {
+                        icon: "chevron-right",
+                        default: !0,
+                        display: "inline",
+                        onClick: () => e.onChange(e.data.page.next)
+                    })]
+                })
+            })]
+        })
+    }
+    return n()
+}
+
+function Bt(e) {
     function n() {
         const a = {
-            backgroundColor: S.colors.primary,
+            backgroundColor: k.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -2272,450 +3199,254 @@
             style: a,
             children: e.total
         })
     }
     return n()
 }
 
-function ft(e) {
-    e.data.id == null && (e.data.id = Math.random());
+function qt(e) {
+    W(`
+    .queryset h1, .queryset h2{
+      margin: 0px;
+    }
+    .queryset .title{
+      display: flex;
+      justify-content: space-between;
+      align-items: center;
+    }
+    .queryset .title .fa-spin{
+      display: none;
+    }
+    .queryset .tabs{
+      text-align: center;
+      width: 100%;
+      margin: auto;
+      padding-bottom: 20px;
+      line-height: 2.5rem;
+    }
+    .queryset .tabs .a{
+        padding-bottom: 5px;
+        padding-left: 15px;
+        padding-right: 15px;
+        font-weight: active ? bold : normal;
+        text-decoration: none;
+    }
+  `), e.data.id == null && (e.data.id = Math.random());
     const [n, a] = I.useState(e.data);
 
     function r() {
-        const m = {
-            margin: 0
-        };
         return n.attrname ? t.jsx("h2", {
-            style: m,
-            "data-label": T(n.title),
-            children: n.title
-        }) : t.jsx("h1", {
-            style: m,
-            "data-label": T(n.title),
+            "data-label": M(n.title),
             children: n.title
+        }) : t.jsxs("h1", {
+            "data-label": M(n.title),
+            children: [n.title, " ", n.total > 10 && "(" + n.total + ")"]
         })
     }
 
-    function o() {
-        const m = {
-            display: "flex",
-            justifyContent: "space-between",
-            alignItems: "center"
-        };
+    function i() {
         return t.jsxs("div", {
-            style: m,
+            className: "title",
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
-                style: {
-                    display: "none"
-                },
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function i(m) {
+    function l(m) {
         document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
     }
 
-    function l() {
+    function d() {
         return n.subsets && t.jsx("div", {
-            style: {
-                textAlign: "center",
-                width: "100%",
-                margin: "auto",
-                paddingBottom: 20,
-                lineHeight: "2.5rem"
-            },
-            children: n.subsets.map(function(m, v) {
-                var g = n.subset === m.name || !n.subset && v == 0;
-                return t.jsxs(N, {
+            className: "tabs",
+            children: n.subsets.map(function(m, p) {
+                var E = n.subset === m.name || !n.subset && p == 0;
+                return t.jsxs(O, {
                     href: "#",
                     style: {
-                        paddingBottom: 5,
-                        paddingLeft: 15,
-                        paddingRight: 15,
-                        fontWeight: g ? "bold" : "normal",
-                        borderBottom: g ? "solid 3px #2670e8" : 0,
-                        textDecoration: "none",
+                        borderBottom: E ? "solid 3px #2670e8" : 0,
                         color: "#0c326f"
                     },
-                    onClick: function(C) {
-                        C.preventDefault(), s(m.name)
+                    onClick: function(N) {
+                        N.preventDefault(), c(m.name)
                     },
-                    dataLabel: T(m.label),
-                    children: [m.label, " ", t.jsx(mt, {
+                    dataLabel: M(m.label),
+                    children: [m.label, " ", t.jsx(Bt, {
                         total: m.count
                     })]
                 }, Math.random())
             })
         })
     }
 
-    function s(m) {
-        const v = document.getElementById("subset-" + e.data.id);
-        v.value = m || "", x()
+    function c(m) {
+        const p = document.getElementById("subset-" + e.data.id);
+        p.value = m || "", D()
     }
 
-    function c(m, v, g) {
-        const C = document.getElementById("form-" + e.data.id);
-        C.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", C.querySelector("input[name=" + n.calendar.field + "__month]").value = v || "", C.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", x()
+    function s(m, p, E) {
+        const N = document.getElementById("form-" + e.data.id);
+        N.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", N.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", N.querySelector("input[name=" + n.calendar.field + "__year]").value = E || "", v(1)
     }
 
     function u() {
-        if (n.calendar) {
-            const E = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
-                ae = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
-                A = {
-                    width: "100%",
-                    borderSpacing: 0,
-                    borderCollapse: "collapse",
-                    marginTop: 15,
-                    marginBottom: 15
-                },
-                z = {
-                    marginLeft: "17",
-                    textAlign: "right",
-                    paddingRight: 2,
-                    paddingTop: 2,
-                    float: "right",
-                    fontSize: "0.8rem"
-                },
-                V = {
-                    verticalAlign: "top",
-                    width: "14.2%",
-                    height: 55,
-                    border: "solid 1px #EEE"
-                },
-                P = {
-                    backgroundColor: S.colors.primary,
-                    borderRadius: "50%",
-                    color: "white",
-                    display: "block",
-                    width: 30,
-                    height: 30,
-                    margin: "auto",
-                    cursor: "pointer",
-                    lineHeight: "2rem"
-                },
-                $ = {
-                    padding: 10,
-                    textAlign: "center"
-                },
-                Ee = {
-                    display: "flex",
-                    justifyContent: "space-between",
-                    alignItems: "baseline"
-                },
-                Ie = new Date,
-                me = n.calendar.day ? new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day) : null;
-            for (var m = [
-                    [],
-                    [],
-                    [],
-                    [],
-                    [],
-                    []
-                ], v = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
-            for (var C = 0;
-                (g.getMonth() <= v || m[C].length < 7) && (m[C].length == 7 && (C += 1), C != 5);) m[C].push({
-                date: g.getDate(),
-                total: n.calendar.total[g.toLocaleDateString("pt-BR")],
-                today: g.getDate() === Ie.getDate(),
-                selected: me ? g.getDate() == me.getDate() : !1
-            }), g.setDate(g.getDate() + 1);
-            return t.jsxs("div", {
-                className: "calendar",
-                children: [t.jsxs("div", {
-                    style: Ee,
-                    children: [t.jsx("div", {
-                        children: t.jsx(fe, {
-                            default: !0,
-                            icon: "arrow-left",
-                            onClick: () => c(null, n.calendar.previous.month, n.calendar.previous.year)
-                        })
-                    }), t.jsxs("div", {
-                        children: [t.jsxs("h3", {
-                            align: "center",
-                            style: {
-                                margin: 0
-                            },
-                            children: [ae[n.calendar.month - 1], " ", n.calendar.year]
-                        }), n.calendar.day && t.jsxs("div", {
-                            align: "center",
-                            className: z,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(j, {
-                                default: !0,
-                                icon: "x",
-                                onClick: () => c(null, n.calendar.month, n.calendar.year),
-                                style: {
-                                    marginLeft: 10,
-                                    cursor: "pointer"
-                                }
-                            })]
-                        })]
-                    }), t.jsx("div", {
-                        children: t.jsx(fe, {
-                            default: !0,
-                            icon: "arrow-right",
-                            onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
-                        })
-                    })]
-                }), t.jsxs("table", {
-                    style: A,
-                    children: [t.jsx("thead", {
-                        children: t.jsx("tr", {
-                            children: E.map(re => t.jsx("th", {
-                                children: re
-                            }, Math.random()))
-                        })
-                    }), t.jsx("tbody", {
-                        children: m.map(re => t.jsx("tr", {
-                            children: re.map(O => t.jsxs("td", {
-                                style: V,
-                                children: [t.jsx("div", {
-                                    style: z,
-                                    children: O.today ? t.jsx("span", {
-                                        style: {
-                                            textDecoration: "underline"
-                                        },
-                                        children: O.date
-                                    }) : O.date + O.today
-                                }), O.total && t.jsx("div", {
-                                    style: $,
-                                    onClick: () => c(O.date, n.calendar.month, n.calendar.year),
-                                    children: t.jsx("div", {
-                                        style: P,
-                                        children: t.jsx("span", {
-                                            style: {
-                                                textDecoration: O.selected ? "underline" : "normal"
-                                            },
-                                            children: O.total
-                                        })
-                                    })
-                                }), !O.total && t.jsx("div", {
-                                    style: $,
-                                    children: " "
-                                })]
-                            }, Math.random()))
-                        }, Math.random()))
-                    })]
-                })]
-            })
-        }
+        if (n.calendar) return t.jsx(Dt, {
+            data: n.calendar,
+            onChange: s
+        })
     }
 
-    function d(m) {
-        const v = {
+    function o(m) {
+        const p = {
             textAlign: "left",
             verticalAlign: "top",
-            lineHeight: "3rem",
-            color: S.colors.primary,
+            lineHeight: "1.2rem",
+            color: k.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [m.map(function(g) {
-                return g.label != "ID" && t.jsx("th", {
-                    style: v,
+            children: [m.map(function(E) {
+                return E.label != "ID" && t.jsx("th", {
+                    style: p,
                     className: "bold",
-                    children: g.label
+                    children: E.label
                 }, Math.random())
             }), t.jsx("th", {
-                style: v
+                style: p
             })]
         })
     }
 
     function h(m) {
-        const v = {
+        const p = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
-            g = {
+            E = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
-                style: v,
+                style: p,
                 children: m.title
             }, Math.random()), t.jsx("td", {
-                style: g,
+                style: E,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: t.jsx(j, {
+                    children: t.jsx(S, {
                         icon: "chevron-right",
-                        onClick: () => _e(m.actions),
+                        onClick: () => Re(m.actions),
                         style: {
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [m.data.map(function(C) {
-                return C.label != "ID" && t.jsx("td", {
-                    style: v,
-                    children: W(C.value)
+            children: [m.data.map(function(N) {
+                return N.label != "ID" && t.jsx("td", {
+                    style: p,
+                    children: F(N.value)
                 }, Math.random())
             }), t.jsx("td", {
-                style: g,
+                style: E,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: m.actions.map(function(C) {
+                    children: m.actions.map(function(N) {
                         return t.jsx(_, {
-                            data: C,
+                            data: N,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
     }
 
     function f() {
-        return n.data.length > 0 ? n.renderer ? t.jsx("div", {
+        return n.data.length > 0 ? (n.render == null && window.innerWidth < 800 && (n.renderer = "rows"), n.renderer ? n.renderer == "cards" ? t.jsx(P, {
+            width: 300,
+            alignItems: "start",
+            children: n.data.map(function(m) {
+                return m.type = n.renderer, t.jsx("div", {
+                    children: t.jsx(x, {
+                        data: m
+                    })
+                }, Math.random())
+            })
+        }) : t.jsx("div", {
             style: {
                 marginBottom: 15
             },
             children: n.data.map(function(m) {
-                return m.type = n.renderer, t.jsx(p, {
+                return m.type = n.renderer, t.jsx(x, {
                     data: m
                 }, Math.random())
             })
-        }) : w() : t.jsx(de, {
+        }) : w()) : t.jsx(oe, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
         const m = {
                 width: "100%",
                 overflowX: "auto"
             },
-            v = {
+            p = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: m,
             children: t.jsxs("table", {
-                style: v,
+                style: p,
                 children: [t.jsx("thead", {
-                    children: d(n.data[0].data)
+                    children: o(n.data[0].data)
                 }), t.jsx("tbody", {
-                    children: n.data.map(function(g) {
-                        return h(g)
+                    children: n.data.map(function(E) {
+                        return h(E)
                     })
                 })]
             })
         })
     }
 
-    function M(m) {
-        const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        g.value = m, x()
+    function v(m) {
+        const E = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
+        E && (E.value = m), D(), j()
     }
 
-    function D() {
+    function B() {
         const m = document.getElementById("form-" + e.data.id);
         if (m) {
-            const E = m.querySelector("input[name=page]");
-            E && (E.value = n.pagination.page.current)
+            const p = m.querySelector("input[name=page]");
+            p && (p.value = n.pagination.page.current)
         }
-        const v = {
-                display: "flex",
-                justifyContent: "space-between",
-                lineHeight: "4rem",
-                alignItems: "baseline"
-            },
-            g = {
-                display: "inline",
-                paddingRight: 10
-            },
-            C = {
-                marginLeft: 10,
-                marginRight: 10,
-                height: "2.5rem",
-                paddingLeft: 5,
-                paddingRight: 5,
-                textAlign: "center"
-            };
-        return n.pagination.page.total > 1 && t.jsxs("div", {
-            style: v,
-            children: [t.jsxs("div", {
-                children: [window.innerWidth > 800 && t.jsxs("div", {
-                    style: g,
-                    children: ["Exibir", t.jsx("select", {
-                        style: C,
-                        name: "page_size",
-                        onChange: () => M(1),
-                        value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(E) {
-                            return t.jsx("option", {
-                                children: E
-                            }, Math.random())
-                        })
-                    })]
-                }), window.innerWidth > 800 && t.jsx("div", {
-                    style: g,
-                    children: "|"
-                }), t.jsxs("div", {
-                    style: g,
-                    children: [n.pagination.start, " - ", n.pagination.end, " de ", n.total]
-                })]
-            }), t.jsx("div", {
-                children: t.jsxs("div", {
-                    style: g,
-                    children: [t.jsx("span", {
-                        children: "Página"
-                    }), t.jsx("input", {
-                        type: "text",
-                        name: "page",
-                        defaultValue: n.pagination.page.current,
-                        style: {
-                            width: 30,
-                            marginLeft: 10,
-                            marginRight: 10,
-                            height: "2rem",
-                            textAlign: "center"
-                        },
-                        onKeyDown: function(E) {
-                            E.key == "Enter" && (E.preventDefault(), M(E.target.value < 0 ? 1 : Math.min(E.target.value, n.pagination.page.total)))
-                        }
-                    }), t.jsx("div", {
-                        style: g,
-                        children: "|"
-                    }), n.pagination.page.previous && t.jsx(R, {
-                        icon: "chevron-left",
-                        default: !0,
-                        display: "inline",
-                        onClick: () => M(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(R, {
-                        icon: "chevron-right",
-                        default: !0,
-                        display: "inline",
-                        onClick: () => M(n.pagination.page.next)
-                    })]
-                })
-            })]
+        return t.jsx(It, {
+            data: n.pagination,
+            onChange: v,
+            total: n.total
         })
     }
 
-    function y() {
+    function g() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(m) {
@@ -2723,289 +3454,317 @@
                     data: m,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function k() {
+    function j() {
+        const m = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
+        console.log(m), console.log(e.data.id), window.scrollTo({
+            top: m,
+            behavior: "smooth"
+        })
+    }
+
+    function y() {
         const m = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
-            v = n.search.length > 0,
-            g = n.filters.length > 0;
-        if ((n.bi || n.data.length >= 0) && (v || g)) {
-            const C = {
+            p = n.search.length > 0,
+            E = n.filters.length > 0;
+        if ((n.bi || n.data.length >= 0) && (p || E)) {
+            const N = {
                 name: "q",
-                value: "",
                 mask: null,
                 type: "text",
-                label: "Palavras-chaves"
+                label: "Palavras-chaves",
+                value: n.q
             };
             return t.jsxs("div", {
                 style: m,
-                children: [t.jsxs(G, {
+                children: [t.jsxs(P, {
                     width: 250,
-                    children: [v && t.jsx("div", {
-                        children: t.jsx(K, {
-                            data: C
+                    children: [p && t.jsx("div", {
+                        children: t.jsx(Z, {
+                            data: N
                         })
-                    }), g && n.filters.map(function(E) {
-                        return E.type != "hidden" && t.jsx("div", {
-                            children: t.jsx(K, {
-                                data: E
+                    }), E && n.filters.map(function(q) {
+                        return q.type != "hidden" && t.jsx("div", {
+                            children: t.jsx(Z, {
+                                data: q
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: x,
+                            onClick: D,
                             label: "Filtrar",
-                            icon: "filter",
-                            primary: !0
+                            icon: "filter"
                         })
                     })]
-                }), g && n.filters.map(function(E) {
-                    return E.type == "hidden" && t.jsx("div", {
-                        children: t.jsx(K, {
-                            data: E
+                }), E && n.filters.map(function(q) {
+                    return q.type == "hidden" && t.jsx("div", {
+                        children: t.jsx(Z, {
+                            data: q
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function x() {
-        i(!0);
+    function D() {
+        l(!0);
         var m;
-        const v = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + v : m = e.data.url + "?" + v, B("GET", m, function(g) {
-            a(g), i(!1)
+        const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
+        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + p : m = e.data.url + "?" + p, L("GET", m, function(E) {
+            a(E), l(!1)
         })
     }
 
-    function L() {
+    function b() {
+        const m = {
+            color: k.colors.primary
+        };
+        return e.data.reloadable && t.jsxs("div", {
+            align: "center",
+            children: [t.jsxs("i", {
+                children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
+            }), t.jsx("div", {
+                children: t.jsx(O, {
+                    style: m,
+                    onClick: p => {
+                        p.preventDefault(), D()
+                    },
+                    children: "Atualizar agora"
+                })
+            })]
+        })
+    }
+
+    function C() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [k(), n.bi.map(function(m) {
-                return t.jsx(G, {
+            children: [y(), n.bi.map(function(m) {
+                return t.jsx(P, {
                     width: 300,
                     alignItems: "start",
-                    children: m.map(function(v) {
+                    children: m.map(function(p) {
                         return t.jsx("div", {
-                            children: t.jsx(p, {
-                                data: v
+                            children: t.jsx(x, {
+                                data: p
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
-        }) : t.jsxs(t.Fragment, {
-            children: [y(), l(), k(), u(), f(), D()]
+        }) : t.jsxs("div", {
+            className: "content",
+            children: [b(), g(), d(), y(), u(), f(), B()]
         })
     }
 
-    function b() {
-        window[e.data.id] = () => x();
+    function T() {
+        window[e.data.id] = () => D();
         const m = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
-            className: "reloadable",
+            className: "reloadable queryset",
             id: e.data.id,
             sytle: m,
             children: t.jsxs("form", {
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), o(), L()]
+                }), i(), C()]
             })
         })
     }
-    return b()
+    return T()
 }
 
 function ne(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
-            var o = echarts.init(r);
-            o.setOption(e.option)
+            var i = echarts.init(r);
+            i.setOption(e.option)
         } else setTimeout(a, 1e3)
     }
     return setTimeout(a, 1e3), t.jsx("div", {
         id: n,
         style: {
             width: "100%",
             height: 300
         }
     })
 }
 
-function ue(e) {
+function he(e) {
     var n = [
         ["70%", "78%"],
         ["60%", "68%"],
         ["50%", "58%"],
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(o, i) {
+        return e.headers ? e.headers.slice(1).map(function(i, l) {
             return {
-                name: o,
+                name: i,
                 type: "pie",
-                radius: n[i],
+                radius: n[l],
                 emphasis: {
                     label: {
                         show: !0,
-                        formatter: function(l) {
-                            return l.value.toLocaleString("pt-BR")
+                        formatter: function(d) {
+                            return d.value.toLocaleString("pt-BR")
                         },
                         fontWeight: "bold"
                     }
                 },
                 roseType: null,
-                data: e.rows.map(function(l) {
+                data: e.rows.map(function(d) {
                     return {
-                        name: l[0],
-                        value: l[i + 1]
+                        name: d[0],
+                        value: d[l + 1]
                     }
                 })
             }
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
             emphasis: {
                 label: {
                     show: !0,
-                    formatter: function(o) {
-                        return o.value.toLocaleString("pt-BR")
+                    formatter: function(i) {
+                        return i.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(o, i) {
+            data: e.rows.map(function(i, l) {
                 return {
-                    name: o[0],
-                    value: o[1]
+                    name: i[0],
+                    value: i[1]
                 }
             })
         }
     }
 
     function r() {
-        var o = {
+        var i = {
             tooltip: {
                 trigger: "item",
-                formatter: function(i) {
-                    return `${i.name}: <b>${i.data.value.toLocaleString("pt-BR")}</b> (${i.percent.toLocaleString("pt-BR")}%)`
+                formatter: function(l) {
+                    return `${l.name}: <b>${l.data.value.toLocaleString("pt-BR")}</b> (${l.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(i) {
-                    return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
+                formatter(l) {
+                    return l.name + " (" + l.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(ne, {
-            option: o
+            option: i
         })
     }
     return r()
 }
 
-function gt(e) {
-    return t.jsx(ue, {
+function Lt(e) {
+    return t.jsx(he, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function yt(e) {
-    return t.jsx(ue, {
+function Nt(e) {
+    return t.jsx(he, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function H(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
-        o = {
+        i = {
             type: "value"
         },
-        i = {
+        l = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
                 },
                 saveAsImage: {
                     show: !0
                 }
             }
         },
-        l = e.area ? {} : null;
+        d = e.area ? {} : null;
 
-    function s() {
+    function c() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(d) {
-                return d[0]
+            data: e.rows.map(function(o) {
+                return o[0]
             })
         }
     }
 
-    function c() {
-        return e.headers ? e.rows.map(function(d) {
+    function s() {
+        return e.headers ? e.rows.map(function(o) {
             return {
-                name: d[0],
-                data: d.slice(1),
+                name: o[0],
+                data: o.slice(1),
                 type: a,
                 stack: r,
-                areaStyle: l
+                areaStyle: d
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(d) {
-                return d[1]
+            data: e.rows.map(function(o) {
+                return o[1]
             }),
             type: a,
             stack: r,
-            areaStyle: l
+            areaStyle: d
         }]
     }
 
     function u() {
-        var d = {
-            toolbox: i,
+        var o = {
+            toolbox: l,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(h) {
                     return `${h[0].name}: <b>${h[0].value.toLocaleString("pt-BR")}</b>`
@@ -3014,88 +3773,88 @@
             legend: {},
             label: {
                 show: !0,
                 formatter: function(h) {
                     return h.value.toLocaleString("pt-BR")
                 }
             },
-            xAxis: n ? o : s(),
-            yAxis: n ? s() : o,
-            series: c()
+            xAxis: n ? i : c(),
+            yAxis: n ? c() : i,
+            series: s()
         };
         return t.jsx(ne, {
-            option: d
+            option: o
         })
     }
     return u()
 }
 
-function xt(e) {
+function At(e) {
     return t.jsx(H, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function vt(e) {
+function Rt(e) {
     return t.jsx(H, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function pt(e) {
+function Ot(e) {
     return t.jsx(H, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function bt(e) {
+function _t(e) {
     return t.jsx(H, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function wt(e) {
+function Ft(e) {
     return t.jsx(H, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function jt(e) {
+function zt(e) {
     return t.jsx(H, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function kt(e) {
+function Wt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
-            data: e.headers.slice(1).map(function(r, o) {
+            data: e.headers.slice(1).map(function(r, i) {
                 return {
                     name: r,
                     type: "pie",
-                    children: e.rows.map(function(i) {
+                    children: e.rows.map(function(l) {
                         return {
-                            name: i[0],
-                            value: i[o + 1]
+                            name: l[0],
+                            value: l[i + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -3113,28 +3872,28 @@
         var r = {
             tooltip: {
                 trigger: "item"
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(o) {
-                    return o.name + " (" + o.value.toLocaleString("pt-BR") + ")"
+                formatter(i) {
+                    return i.name + " (" + i.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
         return t.jsx(ne, {
             option: r
         })
     }
     return a()
 }
 
-function St(e) {
+function Pt(e) {
     function n() {
         var a = {
             series: [{
                 type: "gauge",
                 startAngle: 0,
                 endAngle: 360,
                 min: 0,
@@ -3175,69 +3934,69 @@
         return t.jsx(ne, {
             option: a
         })
     }
     return n()
 }
 
-function xe(e) {
+function ve(e) {
     function n() {
         switch (e.type) {
             case "pie":
-                return t.jsx(ue, {
+                return t.jsx(he, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(yt, {
+                return t.jsx(Nt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(gt, {
+                return t.jsx(Lt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
-                return t.jsx(xt, {
+                return t.jsx(At, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_bar":
-                return t.jsx(bt, {
+                return t.jsx(_t, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "column":
-                return t.jsx(wt, {
+                return t.jsx(Ft, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "stacked_column":
-                return t.jsx(jt, {
+                return t.jsx(zt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "tree_map":
-                return t.jsx(kt, {
+                return t.jsx(Wt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "line":
-                return t.jsx(vt, {
+                return t.jsx(Rt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "area":
-                return t.jsx(pt, {
+                return t.jsx(Ot, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
-                return t.jsx(St, {
+                return t.jsx(Pt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
                 return t.jsx(H, {
                     headers: e.headers,
                     rows: e.rows
@@ -3256,369 +4015,376 @@
                 children: e.title
             }), n()]
         })
     }
     return a()
 }
 
-function Ct(e) {
+function Ht(e) {
     function n() {
-        for (var r = [], o = 0; o < e.data.series.length; o++) r.push([e.data.series[o][0], e.data.series[o][1]]);
-        return e.data.chart ? t.jsx(xe, {
+        for (var r = [], i = 0; i < e.data.series.length; i++) r.push([e.data.series[i][0], e.data.series[i][1]]);
+        return e.data.chart ? t.jsx(ve, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": T(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
-                    children: r.map(i => t.jsx("tr", {
-                        children: i.map((l, s) => s == 0 ? t.jsx("th", {
+                    children: r.map(l => t.jsx("tr", {
+                        children: l.map((d, c) => c == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
                                 lineHeight: "2rem"
                             },
-                            children: l
+                            children: d
                         }, Math.random()) : t.jsx("td", {
-                            children: W(l)
+                            children: F(d)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], o = [], i = Object.keys(e.data.series), l = [], s = 0; s < i.length; s++) {
-            s == 0 && r.push("");
-            for (var c = [i[s]], u = 0, d = 0; d < e.data.series[i[s]].length; d++) {
-                var h = e.data.series[i[s]];
-                s == 0 && r.push(h[d][0]), c.push(h[d][1]), u += h[d][1], i.length > 1 && (s == 0 ? l.push(h[d][1]) : l[d] += h[d][1], d > 0 && d == e.data.series[i[s]].length - 1 && (s == 0 ? l.push(u) : l[d + 1] += u))
+        for (var r = [], i = [], l = Object.keys(e.data.series), d = [], c = 0; c < l.length; c++) {
+            c == 0 && r.push("");
+            for (var s = [l[c]], u = 0, o = 0; o < e.data.series[l[c]].length; o++) {
+                var h = e.data.series[l[c]];
+                c == 0 && r.push(h[o][0]), s.push(h[o][1]), u += h[o][1], l.length > 1 && (c == 0 ? d.push(h[o][1]) : d[o] += h[o][1], o > 0 && o == e.data.series[l[c]].length - 1 && (c == 0 ? d.push(u) : d[o + 1] += u))
             }
-            c.length > 2 && (s == 0 && r.push("TOTAL"), c.push(u)), o.push(c)
+            s.length > 2 && (c == 0 && r.push("TOTAL"), s.push(u)), i.push(s)
         }
-        return e.data.chart ? t.jsx(xe, {
+        return e.data.chart ? t.jsx(ve, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
-            rows: o
+            rows: i
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": T(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%"
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: r.map(f => t.jsx("th", {
                             children: f
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [o.map(f => t.jsx("tr", {
-                        children: f.map((w, M) => M == 0 ? t.jsx("th", {
+                    children: [i.map(f => t.jsx("tr", {
+                        children: f.map((w, v) => v == 0 ? t.jsx("th", {
                             children: w
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
-                                backgroundColor: M == f.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                backgroundColor: v == f.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
-                            children: W(w)
+                            children: F(w)
                         }, Math.random()))
-                    }, Math.random())), l.length > 0 && t.jsxs("tr", {
+                    }, Math.random())), d.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
-                        }), l.map(f => t.jsxs("td", {
+                        }), d.map(f => t.jsxs("td", {
                             align: "center",
                             style: {
                                 backgroundColor: "var(--info-color)"
                             },
-                            children: [W(f), " "]
+                            children: [F(f), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
 
-function Tt() {
+function Ut() {
     function e() {
-        const i = {
+        const l = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: S.colors.primary
+            backgroundColor: k.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
-                    style: i
+                    style: l
                 })
             }), t.jsx("div", {
-                children: t.jsx(N, {
+                children: t.jsx(O, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
             })]
         })
     }
 
-    function n(i) {
-        var l = i.target;
-        const s = l.querySelector(":scope > ul, :scope > li");
-        if (s) {
-            s.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(d) {
-                d.style.display = "block"
-            }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(d) {
-                d.style.display = "none"
+    function n(l) {
+        var d = l.target;
+        const c = d.querySelector(":scope > ul, :scope > li");
+        if (c) {
+            c.offsetParent === null ? d.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(o) {
+                o.style.display = "block"
+            }) : d.querySelectorAll(":scope > ul, :scope > li").forEach(function(o) {
+                o.style.display = "none"
             });
-            const c = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
-                u = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
-            return c && (c.classList.remove("fa-chevron-right"), c.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
+            const s = d.querySelector(":scope > i.fa-solid.fa-chevron-right"),
+                u = d.querySelector(":scope > i.fa-solid.fa-chevron-up");
+            return s && (s.classList.remove("fa-chevron-right"), s.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), l.preventDefault(), l.stopPropagation(), l.cancelBubble = !0, !1
         } else {
-            const c = document.querySelector("aside");
-            c.style.display = window.innerWidth < 800 ? "none" : "block"
+            const s = document.querySelector("aside");
+            s.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
-    function a(i, l) {
-        const s = {
-                display: l == 0 ? "block" : "none",
+    function a(l, d) {
+        const c = {
+                display: d == 0 ? "block" : "none",
                 cursor: "pointer",
-                paddingLeft: 5,
+                paddingLeft: 15,
+                paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: S.colors.primary
+                color: k.colors.primary
             },
-            c = {
+            s = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
-        return i.url ? t.jsx("li", {
-            style: s,
+        return l.url ? t.jsx("li", {
+            style: c,
             onClick: n,
-            children: t.jsxs(N, {
-                href: i.url,
-                dataLabel: T(i.label),
+            className: "item",
+            children: t.jsxs(O, {
+                href: l.url,
+                dataLabel: M(l.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [l == 0 && t.jsx(j, {
-                    icon: i.icon || "dot-circle",
-                    style: c
-                }), i.label]
+                children: [d == 0 && t.jsx(S, {
+                    icon: l.icon || "dot-circle",
+                    style: s
+                }), l.label]
             })
-        }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
+        }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
             onClick: n,
-            style: s,
-            "data-label": T(i.label),
-            children: [l == 0 && t.jsx(j, {
-                icon: i.icon || "dot-circle",
-                style: c
-            }), i.label, t.jsx(j, {
+            style: c,
+            "data-label": M(l.label),
+            children: [d == 0 && t.jsx(S, {
+                icon: l.icon || "dot-circle",
+                style: s
+            }), l.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
                     display: "none",
                     paddingLeft: 15
                 },
-                children: i.items.map(function(u) {
-                    return a(u, l + 1)
+                children: l.items.map(function(u) {
+                    return a(u, d + 1)
                 })
             })]
         }, Math.random())
     }
 
     function r() {
-        const i = {
+        const l = {
             padding: 0
         };
         return window.application.menu.items.length > 0 && t.jsx("ul", {
-            style: i,
-            children: window.application.menu.items.map(function(l) {
-                return a(l, 0)
+            style: l,
+            children: window.application.menu.items.map(function(d) {
+                return a(d, 0)
             })
         })
     }
 
-    function o() {
-        const i = {
-            padding: 25,
+    function i() {
+        const l = {
+            marginTop: 10,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
-            style: i,
+            style: l,
+            className: "menu",
             children: [e(), r()]
         })
     }
-    return o()
+    return i()
 }
 
-function Mt(e) {
+function Gt(e) {
     var n;
 
-    function a(i) {
-        const l = "=".repeat((4 - i.length % 4) % 4),
-            s = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
-            c = window.atob(s),
-            u = new Uint8Array(c.length);
-        for (let d = 0; d < c.length; ++d) u[d] = c.charCodeAt(d);
+    function a(l) {
+        const d = "=".repeat((4 - l.length % 4) % 4),
+            c = (l + d).replace(/\-/g, "+").replace(/_/g, "/"),
+            s = window.atob(c),
+            u = new Uint8Array(s.length);
+        for (let o = 0; o < s.length; ++o) u[o] = s.charCodeAt(o);
         return u
     }
 
     function r() {
-        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
-            if (i) {
-                const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
-                i.pushManager.subscribe({
+        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(l) {
+            if (l) {
+                const d = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
+                l.pushManager.subscribe({
                     userVisibleOnly: !0,
-                    applicationServerKey: l
-                }).then(function(s) {
-                    if (console.log(s), n = JSON.stringify(s), console.log(n), s) {
+                    applicationServerKey: d
+                }).then(function(c) {
+                    if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
-                        var c = new FormData;
-                        c.append("subscription", n), B("POST", "/api/pushsubscribe/", function(u) {
+                        var s = new FormData;
+                        s.append("subscription", n), L("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
-                        }, c)
+                        }, s)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
-                }).catch(function(s) {
-                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", s)
+                }).catch(function(c) {
+                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", c)
                 })
             } else console.log("No registered service worker.")
-        }).catch(function(i) {
-            alert("Erro"), console.error("Service Worker Error", i)
+        }).catch(function(l) {
+            alert("Erro"), console.error("Service Worker Error", l)
         }) : alert("Push messaging is not supported")
     }
 
-    function o() {
-        if (window.Notification == null || window.Notification.permission !== "granted") return t.jsx(j, {
+    function i() {
+        if (window.Notification == null || window.Notification.permission !== "granted") return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: S.colors.primary
+                color: k.colors.primary
             }
         })
     }
-    return o()
+    return i()
 }
 
-function Et(e) {
+function Vt(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: S.colors.primary,
+                backgroundColor: k.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
                 paddingTop: 12,
                 fontSize: "1.8rem"
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
-                    bottom: 80
+                    bottom: 100
                 },
                 onClick: () => history.back(),
-                children: t.jsx(j, {
+                children: t.jsx(S, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
-                onClick: () => window.scrollTo(0, 0),
-                children: t.jsx(j, {
+                onClick: () => window.scrollTo({
+                    top: 0,
+                    behavior: "smooth"
+                }),
+                children: t.jsx(S, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
-function It(e) {
+function $t(e) {
     const [n, a] = I.useState(e.data);
-    window.loaddata = o => a(o);
+    window.loaddata = i => a(i);
 
     function r() {
-        const o = {
+        const i = {
             minHeight: 400,
-            margin: 20
+            margin: window.innerWidth > 800 ? 20 : 5
         };
         return t.jsx("div", {
-            style: o,
+            style: i,
             id: "container",
-            children: t.jsx(p, {
+            children: t.jsx(x, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function Bt(e) {
+function Jt(e) {
     I.useEffect(() => {
-        const d = localStorage.getItem("message");
-        d && (localStorage.removeItem("message"), te(d)), window.addEventListener("resize", () => {
+        const o = localStorage.getItem("message");
+        o && (localStorage.removeItem("message"), te(o)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         })
     }, []);
 
     function a() {
-        const d = document.querySelector("aside");
-        d.style.display = d.style.display == "none" ? "block" : "none"
+        const o = document.querySelector("aside");
+        o.style.display = o.style.display == "none" ? "block" : "none"
     }
 
-    function r(d) {
-        d.preventDefault(), window.load(d.target.href)
+    function r(o) {
+        const h = o.target.tagName == "A" ? o.target : o.target.closest("a");
+        o.preventDefault(), window.load(h.href)
     }
 
-    function o() {
-        const d = {
+    function i() {
+        const o = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
             h = {
@@ -3628,20 +4394,20 @@
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice",
                 icon: "search"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: d,
+            style: o,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [e.data.menu && t.jsx(j, {
+                children: [e.data.menu && t.jsx(S, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3670,273 +4436,296 @@
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(K, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(j, {
+                        children: t.jsx(S, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(Mt, {})
+                    children: t.jsx(Gt, {})
+                }), e.data.navbar.toolbar && window.innerWidth > 800 && e.data.navbar.toolbar.length > 0 && t.jsx("div", {
+                    className: "toolbar",
+                    children: e.data.navbar.toolbar.map(function(f) {
+                        return t.jsx(_, {
+                            data: f,
+                            primary: !0,
+                            compact: !0
+                        }, Math.random())
+                    })
                 }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
                     return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(_, {
                             data: f,
                             primary: !0
                         }, Math.random())
-                    })
+                    }, Math.random())
                 }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
-                    return t.jsx(N, {
+                    return t.jsx(O, {
                         href: f.url,
+                        style: {
+                            marginRight: 10
+                        },
                         children: f.label
-                    })
+                    }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(K, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(j, {
+                        children: t.jsx(S, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(K, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(j, {
+                        children: t.jsx(S, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
-                    children: t.jsx(Te, {
+                    children: t.jsx(Ee, {
                         data: h,
                         style: {
                             padding: 10
                         },
                         onSelect: f => document.location.href = U(f.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(X, {
+                    children: t.jsx(K, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: T(e.data.navbar.user),
+                        dataLabel: M(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: S.colors.primary
+                                backgroundColor: k.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
 
-    function i() {
+    function l() {
         return window.application.menu && window.application.menu.items.length > 0 && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
-            children: t.jsx(Tt, {})
+            children: t.jsx(Ut, {})
         })
     }
 
-    function l() {
-        const d = {
+    function d() {
+        const o = {
                 margin: 15
             },
             h = {
-                color: S.colors.primary
+                color: k.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
-            style: d,
-            children: [t.jsx(N, {
+            style: o,
+            children: [t.jsx(O, {
                 href: "/app/dashboard/",
                 style: {
                     marginRight: 10
                 },
-                children: t.jsx(j, {
+                children: t.jsx(S, {
                     icon: "home",
                     style: h
                 })
             }), "Área Administrativa"]
         })
     }
 
-    function s() {
+    function c() {
         return t.jsxs("main", {
             style: {
-                flexGrow: 6,
-                minWidth: "400px"
+                flexGrow: 6
             },
-            children: [l(), t.jsx(It, {
+            children: [d(), t.jsx($t, {
                 data: e.data.content
             }), t.jsx("footer", {
-                children: c()
-            }), t.jsx(Et, {})]
+                children: s()
+            }), t.jsx(Vt, {})]
         })
     }
 
-    function c() {
+    function s() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
+                children: window.application.sponsors && window.application.sponsors.length > 0 && t.jsx("div", {
+                    children: window.application.sponsors.map(function(o) {
+                        return t.jsx("img", {
+                            src: o,
+                            style: {
+                                height: 30,
+                                padding: 5
+                            }
+                        }, Math.random())
+                    })
+                })
+            }), t.jsx("div", {
                 children: "Todos os direitos reservados"
             }), t.jsx("div", {
                 children: e.data.footer.version
             })]
         }) : null
     }
 
     function u() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
-                children: o()
+                children: i()
             }), t.jsxs("div", {
                 style: {
                     overflowX: "hide",
                     width: "100%",
                     display: "flex",
                     overflow: "hidden",
                     minHeight: window.innerHeight - 70
                 },
-                children: [i(), s()]
+                children: [l(), c()]
             })]
         })
     }
     return u()
 }
 
-function Dt(e) {
+function Yt(e) {
     var n = null,
         a = null,
         r = null,
-        o = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
-        i = {
+        i = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
+        l = {
             constraints: {
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: y => y.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: g => g.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
     I.useEffect(() => {
-        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(y) {
+        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(g) {
             document.getElementById("callerid").innerHTML = e.data.caller
-        }), n.on("call", function(y) {
-            o({
+        }), n.on("call", function(g) {
+            i({
                 video: {
                     width: {
                         exact: 320
                     },
                     height: {
                         exact: 240
                     }
                 },
                 audio: !0
-            }, function(k) {
-                a = k;
-                var x = document.getElementById("video2");
-                x.addEventListener("loadedmetadata", function(L) {
-                    x.style.width = this.videoWidth / 4 + "px", x.style.height = this.videoHeight / 4 + "px", x.style.marginLeft = -this.videoWidth / 4 + "px", x.style.visibility = "visible"
-                }, !1), x.srcObject = a, y.answer(k), y.on("stream", function(L) {
-                    r = L, document.getElementById("video1").srcObject = r
-                }), y.on("close", function() {
-                    c()
-                }), n.on("error", function(L) {
-                    c()
+            }, function(j) {
+                a = j;
+                var y = document.getElementById("video2");
+                y.addEventListener("loadedmetadata", function(D) {
+                    y.style.width = this.videoWidth / 4 + "px", y.style.height = this.videoHeight / 4 + "px", y.style.marginLeft = -this.videoWidth / 4 + "px", y.style.visibility = "visible"
+                }, !1), y.srcObject = a, g.answer(j), g.on("stream", function(D) {
+                    r = D, document.getElementById("video1").srcObject = r
+                }), g.on("close", function() {
+                    s()
+                }), n.on("error", function(D) {
+                    s()
                 })
-            }, function(k) {
-                console.log("Failed to get local stream", k)
+            }, function(j) {
+                console.log("Failed to get local stream", j)
             })
-        }), n.on("error", function(y) {
-            y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? alert("Problema na conexão do usuário.") : y.type == "peer-unavailable" && alert("Usuário indisponível.")
+        }), n.on("error", function(g) {
+            g.type == "browser-incompatible" ? alert("Navegador incompatível.") : g.type == "invalid-id" ? alert("Usuário inexistente.") : g.type == "network" ? alert("Problema na conexão do usuário.") : g.type == "peer-unavailable" && alert("Usuário indisponível.")
         })
     }, []);
 
-    function l() {
-        d(a, "audio"), d(a, "video"), d(r, "audio"), d(r, "video")
+    function d() {
+        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
     }
 
-    function s() {
+    function c() {
         h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
-    function c() {
+    function s() {
         u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
     }
 
-    function u(y, k) {
-        y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === k && x.stop()
+    function u(g, j) {
+        g != null && g.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && y.stop()
         })
     }
 
-    function d(y, k) {
-        y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === k && (x.enabled = !1)
+    function o(g, j) {
+        g != null && g.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && (y.enabled = !1)
         })
     }
 
-    function h(y, k) {
-        y != null && y.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === k && (x.enabled = !0)
+    function h(g, j) {
+        g != null && g.getTracks().forEach(y => {
+            y.readyState == "live" && y.kind === j && (y.enabled = !0)
         })
     }
 
     function f() {
-        var y = document.getElementById("video1");
-        y.style.width == "" ? y.style.width = "400px" : y.style.width = ""
+        var g = document.getElementById("video1");
+        g.style.width == "" ? g.style.width = "400px" : g.style.width = ""
     }
 
     function w() {
-        var y = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
-        y.on("stream", function(k) {
-            r = k, document.getElementById("video1").srcObject = r
-        }), y.on("close", function() {
-            c()
-        }), n.on("error", function(k) {
-            c()
+        var g = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, l);
+        g.on("stream", function(j) {
+            r = j, document.getElementById("video1").srcObject = r
+        }), g.on("close", function() {
+            s()
+        }), n.on("error", function(j) {
+            s()
         })
     }
 
-    function M() {
+    function v() {
         if (a != null && r == null) return w();
-        if (a != null && r != null) return s();
-        o({
+        if (a != null && r != null) return c();
+        i({
             video: {
                 width: {
                     exact: 320
                 },
                 height: {
                     exact: 240
                 }
@@ -3947,567 +4736,182 @@
                 echoCancellation: !1,
                 latency: 0,
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
-        }, function(y) {
-            a = y;
-            var k = document.getElementById("video2");
-            k.addEventListener("loadedmetadata", function(x) {
-                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
-            }, !1), k.srcObject = a, w()
-        }, function(y) {
+        }, function(g) {
+            a = g;
+            var j = document.getElementById("video2");
+            j.addEventListener("loadedmetadata", function(y) {
+                j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
+            }, !1), j.srcObject = a, w()
+        }, function(g) {
             alert("Failed to get local stream.")
         })
     }
 
-    function D() {
-        var y = {
+    function B() {
+        var g = {
                 width: "fit-content",
                 margin: "auto"
             },
-            k = {
+            j = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            x = {
+            y = {
                 color: "white",
                 backgroundColor: "black",
                 padding: 2
             },
-            L = {
+            D = {
                 position: "absolute",
                 marginTop: "-30px"
             },
             b = {
                 backgroundColor: "black"
             },
-            m = {
+            C = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: y,
+            style: g,
             children: [t.jsx("div", {
                 id: "callerid",
-                style: k
+                style: j
             }), t.jsx("video", {
                 id: "video1",
                 style: b,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
-                style: m,
+                style: C,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
-                style: L,
-                children: [t.jsx(j, {
-                    style: x,
-                    onClick: M,
+                style: D,
+                children: [t.jsx(S, {
+                    style: y,
+                    onClick: v,
                     icon: "play"
-                }), t.jsx(j, {
-                    style: x,
-                    onClick: l,
+                }), t.jsx(S, {
+                    style: y,
+                    onClick: d,
                     icon: "pause"
-                }), t.jsx(j, {
-                    style: x,
-                    onClick: c,
+                }), t.jsx(S, {
+                    style: y,
+                    onClick: s,
                     icon: "stop"
-                }), t.jsx(j, {
-                    style: x,
+                }), t.jsx(S, {
+                    style: y,
                     onClick: f,
                     icon: "maximize"
                 })]
             })]
         })
     }
-    return D()
+    return B()
 }
 
-function Lt(e) {
-    return t.jsx("img", {
-        src: e.data.src,
-        style: {
-            width: "100%"
-        }
-    })
-}
-
-function At(e) {
+function Qt(e) {
     const n = {
-        width: "100%",
-        textAlign: "center"
+        color: e.data.color
     };
-    return t.jsx("div", {
-        style: n,
-        children: t.jsx("img", {
-            src: e.data.src,
-            style: {
-                width: e.data.width,
-                height: e.data.height,
-                borderRadius: e.data.round ? "50%" : 0
-            }
-        })
-    })
-}
-
-function qt(e) {
-    return t.jsx("iframe", {
-        width: e.data.width || "100%",
-        height: e.data.height || "400px",
-        id: "gmap_canvas",
-        src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
-        frameBorder: "0",
-        scrolling: "no",
-        marginHeight: "0",
-        marginWidth: "0"
-    })
-}
-
-function Rt(e) {
-    function n(i) {
-        return e.data.icon ? i.done ? t.jsx(j, {
-            style: {
-                marginTop: 6
-            },
-            icon: e.data.icon
-        }) : t.jsx("span", {
-            children: " "
-        }) : t.jsx("div", {
-            style: {
-                marginTop: 6
-            },
-            children: i.number
-        })
-    }
-
-    function a(i) {
-        return {
-            border: "3px solid " + S.colors.primary,
-            borderRadius: "50%",
-            background: i.done ? S.colors.primary : "white",
-            color: i.done ? "white" : S.colors.primary,
-            textAlign: "center",
-            width: 50,
-            height: 50,
-            margin: "auto",
-            fontSize: "1.5rem"
-        }
-    }
-
-    function r(i) {
-        return {
-            listStyleType: "none",
-            display: "flex",
-            justifyContent: "center",
-            minWidth: i.length * 100
-        }
-    }
-
-    function o() {
-        const i = {
-                width: "100%",
-                margin: "auto",
-                overflowX: "auto",
-                "&::WebkitScrollbar": {
-                    width: 0
-                }
-            },
-            l = {
-                width: 100,
-                marginWidth: 100,
-                textAlign: "center"
-            },
-            s = {
-                position: "relative",
-                borderBottom: "2px solid #1151b3",
-                top: -28,
-                width: 45,
-                left: 77
-            };
-        return t.jsx("div", {
-            children: t.jsx("div", {
-                style: i,
-                children: t.jsx("ul", {
-                    style: r(e.data.steps),
-                    children: e.data.steps.map((c, u) => t.jsxs("li", {
-                        style: l,
-                        children: [t.jsx("div", {
-                            style: a(c),
-                            children: n(c)
-                        }), u < e.data.steps.length - 1 && t.jsx("div", {
-                            style: s
-                        }), t.jsx("div", {
-                            children: c.name
-                        })]
-                    }, Math.random()))
-                })
-            })
-        })
-    }
-    return o()
-}
-
-function Nt(e) {
-    function n() {
-        const a = {
-                display: "inline-block",
-                width: "100%",
-                backgroundColor: "#DDD",
-                borderRadius: 5,
-                marginTop: 5
-            },
-            r = {
-                marginLeft: 10
-            },
-            o = {
-                display: "block",
-                paddingTop: 2,
-                paddingBottom: 2,
-                color: "white",
-                borderRadius: 5,
-                width: e.data.value + "%",
-                backgroundColor: S.colors[e.data.style]
-            };
-        return t.jsx("span", {
-            style: a,
-            children: t.jsx("span", {
-                style: o,
-                children: t.jsxs("span", {
-                    style: r,
-                    children: [e.data.value, "%"]
-                })
-            })
-        })
-    }
-    return n()
-}
-
-function Ot(e) {
-    function n() {
-        return e.data.color = S.colors[e.data.style], t.jsx(Me, {
-            data: e.data
-        })
-    }
-    return n()
-}
-
-function Me(e) {
-    function n() {
-        const a = {
-            color: "white",
-            width: "fit-content",
-            borderRadius: 5,
-            textWrap: "nowrap",
-            padding: 10,
-            whiteSpace: "nowrap",
-            backgroundColor: e.data.color
-        };
-        return t.jsx("div", {
-            style: a,
-            children: e.data.label
-        })
-    }
-    return n()
-}
-
-function _t(e) {
-    function n() {
-        const a = {
-                padding: 20,
-                marginLeft: -20,
-                marginRight: -20,
-                textAlign: "center",
-                backgroundColor: "#f8f8f8"
-            },
-            r = {
-                padding: 20,
-                display: "inline-flex",
-                flexDirection: "column",
-                width: 250,
-                height: 250,
-                backgroundColor: "white",
-                boxShadow: "0px 15px 10px -15px #DDD",
-                margin: 10,
-                textDecoration: "none"
-            },
-            o = {
-                marginTop: 30,
-                fontSize: "3rem",
-                color: S.colors.auxiliary
-            },
-            i = {
-                marginTop: 40,
-                fontWeight: "bold",
-                fontSize: "1.2rem",
-                textTransform: "uppercase",
-                height: 70,
-                color: S.colors.primary
-            };
-        return e.data.items.length ? t.jsxs("div", {
-            style: a,
-            children: [t.jsx("h2", {
-                "data-label": T(e.data.title),
-                style: {
-                    color: S.colors.primary
-                },
-                children: e.data.title
-            }), t.jsx("div", {
-                children: e.data.items.map(l => t.jsxs(N, {
-                    href: l.url,
-                    style: r,
-                    dataLabel: l.label,
-                    children: [t.jsx("div", {
-                        children: t.jsx(j, {
-                            style: o,
-                            icon: l.icon
-                        })
-                    }), t.jsx("div", {
-                        style: i,
-                        children: l.label
-                    })]
-                }, Math.random()))
-            })]
-        }) : null
-    }
-    return n()
-}
-
-function Ft(e) {
-    function n() {
-        return t.jsx("div", {
-            style: {
-                backgroundColor: "black",
-                color: "white",
-                padding: "10px",
-                minHeight: "300px",
-                fontFamily: "monospace, monospace",
-                marginBottom: "30px"
-            },
-            children: e.data.output.split(`
-`).map(a => t.jsx("div", {
-                children: a
-            }, Math.random()))
-        })
-    }
-    return n()
-}
-
-function zt(e) {
-    function n() {
-        return e.data.url ? t.jsx(N, {
-            href: e.data.url,
-            imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(j, {
-                icon: e.data.icon
-            }) : e.data.url
-        }) : t.jsx("span", {
-            children: "-"
-        })
-    }
-    return n()
-}
-
-function Wt(e) {
-    function n() {
-        return t.jsx("iframe", {
-            src: e.data.url,
-            width: "100%",
-            height: 500,
-            style: {
-                border: 0
-            }
-        })
-    }
-    return n()
-}
-
-function Ht(e) {
-    const n = Math.random();
-    I.useEffect(() => {
-        new QRCode(document.getElementById(n), {
-            text: e.data.text,
-            width: 128,
-            height: 128,
-            colorDark: "#333333",
-            colorLight: "#ffffff",
-            correctLevel: QRCode.CorrectLevel.H
-        })
-    }, []);
 
     function a() {
         return t.jsx("div", {
-            id: n
+            style: n,
+            children: e.data.text
         })
     }
     return a()
 }
-
-function Pt(e) {
-    function n() {
-        const a = {
-                color: "white",
-                backgroundColor: S.colors.highlight,
-                margin: -20,
-                textAlign: "center",
-                paddingTop: 20,
-                paddingBottom: 70
-            },
-            r = {
-                fontSize: "4rem",
-                fontWeight: "bold",
-                marginTop: 25
-            },
-            o = {
-                fontSize: "1.2rem",
-                maxWidth: 200,
-                margin: "auto"
-            };
-        if (e.data) return t.jsxs("div", {
-            className: "indicators",
-            style: a,
-            children: [t.jsx("h1", {
-                "data-label": T(e.data.title),
-                children: e.data.title
-            }), t.jsx(G, {
-                width: 300,
-                children: e.data.items.map(i => t.jsxs("div", {
-                    children: [t.jsx("div", {
-                        style: r,
-                        children: W(i.value)
-                    }), t.jsx("div", {
-                        style: o,
-                        children: i.name
-                    })]
-                }, Math.random()))
-            }, Math.random()), t.jsx("div", {
-                className: "actions",
-                children: e.data.actions.map(i => t.jsx(N, {
-                    href: q(i.url),
-                    label: i.label,
-                    modal: i.modal,
-                    children: i.label
-                }, Math.random()))
-            })]
-        })
-    }
-    return n()
-}
-
-function Ut(e) {
-    function n() {
-        return t.jsx(G, {
-            width: 400,
-            children: e.data.items.map((a, r) => t.jsx("div", {
-                children: t.jsx(p, {
-                    data: a
-                })
-            }, Math.random()))
-        })
-    }
-    return n()
-}
-
-function Gt(e) {
-    function n() {
-        return t.jsxs("div", {
-            children: [t.jsx("h2", {
-                children: e.data.title
-            }), t.jsx("div", {
-                style: {
-                    fontSize: "12rem",
-                    textAlign: "center",
-                    color: "#5470c6"
-                },
-                children: e.data.value
-            })]
-        })
-    }
-    return n()
-}
-var Z, he = {};
-const Vt = "/api/application/",
-    ve = localStorage.getItem("application");
-
-function p(e) {
-    const n = he[e.data.type];
-    return n ? Be.createElement(n, {
+var ee, me = {};
+const Xt = "/api/application/",
+    be = localStorage.getItem("application");
+
+function x(e) {
+    const n = me[e.data.type];
+    return n ? Te.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-p.register = function(e, n) {
-    he[n.toLowerCase()] = e
+x.register = function(e, n) {
+    me[n.toLowerCase()] = e
 };
-p.render = function(e) {
-    Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
+x.render = function(e) {
+    ee = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-p.register(Gt, "Counter");
-p.register(ht, "Form");
-p.register(ft, "QuerySet");
-p.register(Ve, "Fieldset");
-p.register(Y, "Field");
-p.register(Ye, "Object");
-p.register(Qe, "Section");
-p.register(Ke, "Group");
-p.register(Ct, "Statistics");
-p.register(At, "Image");
-p.register(Lt, "Banner");
-p.register(qt, "Map");
-p.register(Rt, "Steps");
-p.register(Ht, "QrCode");
-p.register(Me, "Badge");
-p.register(Ot, "Status");
-p.register(Nt, "Progress");
-p.register(De, "Color");
-p.register(_t, "Boxes");
-p.register(Pt, "Indicators");
-p.register(Ft, "Shell");
-p.register(zt, "FileLink");
-p.register(Wt, "FilePreview");
-p.register(Ne, "Response");
-p.register(Bt, "Application");
-p.register(Le, "IconSet");
-p.register(Ut, "Grid");
-p.register(Ue, "Rows");
-p.register(Ge, "Timeline");
-p.register(Dt, "WebConf");
+x.register(ht, "Counter");
+x.register(Tt, "Form");
+x.register(qt, "QuerySet");
+x.register(Ge, "Fieldset");
+x.register(V, "Field");
+x.register(Je, "Object");
+x.register(Ye, "Section");
+x.register(Xe, "Group");
+x.register(Ht, "Statistics");
+x.register(et, "Image");
+x.register(Ze, "Banner");
+x.register(tt, "Map");
+x.register(nt, "Steps");
+x.register(st, "QrCode");
+x.register(Se, "Badge");
+x.register(rt, "Status");
+x.register(at, "Progress");
+x.register(De, "Color");
+x.register(it, "Boxes");
+x.register(ct, "Indicators");
+x.register(lt, "Shell");
+x.register(ot, "FileLink");
+x.register(dt, "FilePreview");
+x.register(Ne, "Response");
+x.register(Jt, "Application");
+x.register(Ie, "IconSet");
+x.register(ut, "Grid");
+x.register(Pe, "Rows");
+x.register(He, "Cards");
+x.register(Ue, "Timeline");
+x.register(Ce, "Scheduler");
+x.register(Yt, "WebConf");
+x.register(Qt, "Text");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    he[n] ? B("GET", q(e), function(a) {
-        Z.render(t.jsx(p, {
+    me[n] ? L("GET", A(e), function(a) {
+        ee.render(t.jsx(x, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), ve ? (window.application = JSON.parse(ve), B("GET", q(e), function(a) {
-        window.application.content = a, Z.render(t.jsx(p, {
+    }, "", e), be ? (window.application = JSON.parse(be), L("GET", A(e), function(a) {
+        window.application.content = a, ee.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
-    })) : B("GET", Vt, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), B("GET", q(e), function(o) {
-            window.application.content = o, Z.render(t.jsx(p, {
+    })) : L("GET", Xt, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), L("GET", A(e), function(i) {
+            window.application.content = i, ee.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), B("GET", q(e), function(n) {
+    }, "", e), L("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-p.render(F.createRoot(document.getElementById("root")));
+x.render(z.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.3.2/slth/static/js/vanilla-masker.js` & `pyslth-0.3.3/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.3/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/statistics.py` & `pyslth-0.3.3/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/templates/index.html` & `pyslth-0.3.3/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/templates/service-worker.js` & `pyslth-0.3.3/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/tests.py` & `pyslth-0.3.3/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/urls.py` & `pyslth-0.3.3/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/utils.py` & `pyslth-0.3.3/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.2/slth/views.py` & `pyslth-0.3.3/slth/views.py`

 * *Files identical despite different names*

