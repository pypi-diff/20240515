# Comparing `tmp/bigcode-1.0.8.tar.gz` & `tmp/bigcode-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigcode-1.0.8.tar", last modified: Tue May 14 15:05:09 2024, max compression
+gzip compressed data, was "bigcode-1.0.9.tar", last modified: Wed May 15 19:03:17 2024, max compression
```

## Comparing `bigcode-1.0.8.tar` & `bigcode-1.0.9.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.642442 bigcode-1.0.8/
--rw-r--r--   0 ayhan      (501) staff       (20)      173 2024-05-12 15:17:21.000000 bigcode-1.0.8/MANIFEST.in
--rw-r--r--   0 ayhan      (501) staff       (20)      745 2024-05-14 15:05:09.642536 bigcode-1.0.8/PKG-INFO
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.586053 bigcode-1.0.8/bigcode/
--rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-14 15:05:02.000000 bigcode-1.0.8/bigcode/__init__.py
--rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.8/bigcode/apps.py
--rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/compat.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.586881 bigcode-1.0.8/bigcode/locale/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578454 bigcode-1.0.8/bigcode/locale/bg/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.587321 bigcode-1.0.8/bigcode/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     9666 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)    17953 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578561 bigcode-1.0.8/bigcode/locale/de/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.587695 bigcode-1.0.8/bigcode/locale/de/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     1536 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     2486 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578663 bigcode-1.0.8/bigcode/locale/es/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.587989 bigcode-1.0.8/bigcode/locale/es/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     1572 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     2518 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578770 bigcode-1.0.8/bigcode/locale/fr/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.588273 bigcode-1.0.8/bigcode/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     3080 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     3379 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578871 bigcode-1.0.8/bigcode/locale/hu/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.588602 bigcode-1.0.8/bigcode/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     2967 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     5327 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.578973 bigcode-1.0.8/bigcode/locale/ru/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.588974 bigcode-1.0.8/bigcode/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     2862 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     4142 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.589132 bigcode-1.0.8/bigcode/locale/tk/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/tk/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.589739 bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/.DS_Store
--rw-r--r--   0 ayhan      (501) staff       (20)    16705 2024-05-12 12:28:14.000000 bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)    15752 2024-05-12 12:28:12.000000 bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.579205 bigcode-1.0.8/bigcode/locale/uz/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.590149 bigcode-1.0.8/bigcode/locale/uz/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     3213 2024-05-14 14:55:55.000000 bigcode-1.0.8/bigcode/locale/uz/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     4415 2024-05-14 14:55:52.000000 bigcode-1.0.8/bigcode/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.579312 bigcode-1.0.8/bigcode/locale/zh_Hans/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.590544 bigcode-1.0.8/bigcode/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     1282 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     2085 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.579421 bigcode-1.0.8/bigcode/locale/zh_Hant/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.590854 bigcode-1.0.8/bigcode/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 ayhan      (501) staff       (20)     1284 2024-05-12 11:58:05.000000 bigcode-1.0.8/bigcode/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 ayhan      (501) staff       (20)     2088 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.8/bigcode/settings.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.591002 bigcode-1.0.8/bigcode/static/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 13:17:42.000000 bigcode-1.0.8/bigcode/static/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.591522 bigcode-1.0.8/bigcode/static/admin/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 14:16:10.000000 bigcode-1.0.8/bigcode/static/admin/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.591829 bigcode-1.0.8/bigcode/static/admin/js/
--rw-r--r--   0 ayhan      (501) staff       (20)      564 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/admin/js/cancel.js
--rw-r--r--   0 ayhan      (501) staff       (20)     1946 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/admin/js/popup_response.js
--rw-r--r--   0 ayhan      (501) staff       (20)    75842 2024-05-01 18:35:35.000000 bigcode-1.0.8/bigcode/static/admin/logo.png
--rw-r--r--   0 ayhan      (501) staff       (20)      206 2024-05-10 14:15:38.000000 bigcode-1.0.8/bigcode/static/admin/plus.svg
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.579967 bigcode-1.0.8/bigcode/static/jazzmin/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.591981 bigcode-1.0.8/bigcode/static/jazzmin/css/
--rw-r--r--   0 ayhan      (501) staff       (20)    16969 2024-05-11 10:58:51.000000 bigcode-1.0.8/bigcode/static/jazzmin/css/main.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.593261 bigcode-1.0.8/bigcode/static/jazzmin/img/
--rw-r--r--   0 ayhan      (501) staff       (20)     1094 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/calendar-icons.svg
--rw-r--r--   0 ayhan      (501) staff       (20)   223437 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/default-log.svg
--rw-r--r--   0 ayhan      (501) staff       (20)     7070 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/default.jpg
--rw-r--r--   0 ayhan      (501) staff       (20)     1086 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/icon-calendar.svg
--rw-r--r--   0 ayhan      (501) staff       (20)      380 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/icon-changelink.svg
--rw-r--r--   0 ayhan      (501) staff       (20)     3291 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/img/selector-icons.svg
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.594007 bigcode-1.0.8/bigcode/static/jazzmin/js/
--rw-r--r--   0 ayhan      (501) staff       (20)     6052 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/js/change_form.js
--rw-r--r--   0 ayhan      (501) staff       (20)     2252 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/js/change_list.js
--rw-r--r--   0 ayhan      (501) staff       (20)     2391 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/js/main.js
--rw-r--r--   0 ayhan      (501) staff       (20)     6258 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/js/related-modal.js
--rw-r--r--   0 ayhan      (501) staff       (20)    13873 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/js/ui-builder.js
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.580012 bigcode-1.0.8/bigcode/static/jazzmin/plugins/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.594169 bigcode-1.0.8/bigcode/static/jazzmin/plugins/bootstrap-show-modal/
--rw-r--r--   0 ayhan      (501) staff       (20)     2756 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.594326 bigcode-1.0.8/bigcode/static/vendor/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 13:17:31.000000 bigcode-1.0.8/bigcode/static/vendor/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.594513 bigcode-1.0.8/bigcode/static/vendor/adminlte/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 11:55:19.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.596805 bigcode-1.0.8/bigcode/static/vendor/adminlte/css/
--rw-r--r--   0 ayhan      (501) staff       (20)  1382975 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/css/adminlte.min.css
--rw-r--r--   0 ayhan      (501) staff       (20)  3783107 2024-05-12 11:44:51.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/css/adminlte.min.css.map
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.602304 bigcode-1.0.8/bigcode/static/vendor/adminlte/img/
--rw-r--r--   0 ayhan      (501) staff       (20)     2637 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/img/AdminLTELogo.png
--rw-r--r--   0 ayhan      (501) staff       (20)     1139 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/img/icons.png
--rw-r--r--   0 ayhan      (501) staff       (20)     5357 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/img/user2-160x160.jpg
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.602711 bigcode-1.0.8/bigcode/static/vendor/adminlte/js/
--rw-r--r--   0 ayhan      (501) staff       (20)    44244 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/js/adminlte.min.js
--rw-r--r--   0 ayhan      (501) staff       (20)   129651 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/adminlte/js/adminlte.min.js.map
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.580525 bigcode-1.0.8/bigcode/static/vendor/bootstrap/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.604723 bigcode-1.0.8/bigcode/static/vendor/bootstrap/js/
--rw-r--r--   0 ayhan      (501) staff       (20)    62440 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 ayhan      (501) staff       (20)   187646 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.582626 bigcode-1.0.8/bigcode/static/vendor/bootswatch/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.605078 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cerulean/
--rw-r--r--   0 ayhan      (501) staff       (20)   163350 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cerulean/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.605956 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cosmo/
--rw-r--r--   0 ayhan      (501) staff       (20)   154456 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cosmo/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.606619 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cyborg/
--rw-r--r--   0 ayhan      (501) staff       (20)   164597 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/cyborg/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.607056 bigcode-1.0.8/bigcode/static/vendor/bootswatch/darkly/
--rw-r--r--   0 ayhan      (501) staff       (20)   164202 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/darkly/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.607647 bigcode-1.0.8/bigcode/static/vendor/bootswatch/default/
--rw-r--r--   0 ayhan      (501) staff       (20)   161972 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/default/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.608431 bigcode-1.0.8/bigcode/static/vendor/bootswatch/flatly/
--rw-r--r--   0 ayhan      (501) staff       (20)   164819 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/flatly/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.609204 bigcode-1.0.8/bigcode/static/vendor/bootswatch/journal/
--rw-r--r--   0 ayhan      (501) staff       (20)   161735 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/journal/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.610745 bigcode-1.0.8/bigcode/static/vendor/bootswatch/litera/
--rw-r--r--   0 ayhan      (501) staff       (20)   165148 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/litera/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.611788 bigcode-1.0.8/bigcode/static/vendor/bootswatch/lumen/
--rw-r--r--   0 ayhan      (501) staff       (20)   167943 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/lumen/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.612162 bigcode-1.0.8/bigcode/static/vendor/bootswatch/lux/
--rw-r--r--   0 ayhan      (501) staff       (20)   155932 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/lux/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.612996 bigcode-1.0.8/bigcode/static/vendor/bootswatch/materia/
--rw-r--r--   0 ayhan      (501) staff       (20)   194473 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/materia/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.613842 bigcode-1.0.8/bigcode/static/vendor/bootswatch/minty/
--rw-r--r--   0 ayhan      (501) staff       (20)   165946 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/minty/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.614164 bigcode-1.0.8/bigcode/static/vendor/bootswatch/pulse/
--rw-r--r--   0 ayhan      (501) staff       (20)   155889 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/pulse/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.614481 bigcode-1.0.8/bigcode/static/vendor/bootswatch/sandstone/
--rw-r--r--   0 ayhan      (501) staff       (20)   163543 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/sandstone/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.615061 bigcode-1.0.8/bigcode/static/vendor/bootswatch/simplex/
--rw-r--r--   0 ayhan      (501) staff       (20)   163234 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/simplex/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.616229 bigcode-1.0.8/bigcode/static/vendor/bootswatch/sketchy/
--rw-r--r--   0 ayhan      (501) staff       (20)   167043 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/sketchy/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.616905 bigcode-1.0.8/bigcode/static/vendor/bootswatch/slate/
--rw-r--r--   0 ayhan      (501) staff       (20)   171632 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/slate/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.617248 bigcode-1.0.8/bigcode/static/vendor/bootswatch/solar/
--rw-r--r--   0 ayhan      (501) staff       (20)   169219 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/solar/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.617941 bigcode-1.0.8/bigcode/static/vendor/bootswatch/spacelab/
--rw-r--r--   0 ayhan      (501) staff       (20)   164894 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/spacelab/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.618729 bigcode-1.0.8/bigcode/static/vendor/bootswatch/superhero/
--rw-r--r--   0 ayhan      (501) staff       (20)   164559 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/superhero/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.619406 bigcode-1.0.8/bigcode/static/vendor/bootswatch/united/
--rw-r--r--   0 ayhan      (501) staff       (20)   161367 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/united/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.619704 bigcode-1.0.8/bigcode/static/vendor/bootswatch/yeti/
--rw-r--r--   0 ayhan      (501) staff       (20)   168497 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/bootswatch/yeti/bootstrap.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.582879 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.620423 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/css/
--rw-r--r--   0 ayhan      (501) staff       (20)    59344 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/css/all.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.630048 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/
--rw-r--r--   0 ayhan      (501) staff       (20)   134346 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
--rw-r--r--   0 ayhan      (501) staff       (20)   747545 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
--rw-r--r--   0 ayhan      (501) staff       (20)   134040 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0 ayhan      (501) staff       (20)    90060 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
--rw-r--r--   0 ayhan      (501) staff       (20)    76764 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0 ayhan      (501) staff       (20)    34034 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
--rw-r--r--   0 ayhan      (501) staff       (20)   144714 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
--rw-r--r--   0 ayhan      (501) staff       (20)    33736 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0 ayhan      (501) staff       (20)    16276 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
--rw-r--r--   0 ayhan      (501) staff       (20)    13276 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0 ayhan      (501) staff       (20)   203030 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
--rw-r--r--   0 ayhan      (501) staff       (20)   918991 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
--rw-r--r--   0 ayhan      (501) staff       (20)   202744 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0 ayhan      (501) staff       (20)   101652 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
--rw-r--r--   0 ayhan      (501) staff       (20)    78196 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.583121 bigcode-1.0.8/bigcode/static/vendor/select2/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.630305 bigcode-1.0.8/bigcode/static/vendor/select2/css/
--rw-r--r--   0 ayhan      (501) staff       (20)    16264 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/select2/css/select2.min.css
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.630684 bigcode-1.0.8/bigcode/static/vendor/select2/js/
--rw-r--r--   0 ayhan      (501) staff       (20)    73170 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/static/vendor/select2/js/select2.min.js
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.631230 bigcode-1.0.8/bigcode/templates/
--rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-12 14:21:10.000000 bigcode-1.0.8/bigcode/templates/.DS_Store
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.635015 bigcode-1.0.8/bigcode/templates/admin/
--rw-r--r--   0 ayhan      (501) staff       (20)     1551 2024-05-11 12:33:43.000000 bigcode-1.0.8/bigcode/templates/admin/actions.html
--rw-r--r--   0 ayhan      (501) staff       (20)      517 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/app_index.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.583404 bigcode-1.0.8/bigcode/templates/admin/auth/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.635387 bigcode-1.0.8/bigcode/templates/admin/auth/user/
--rw-r--r--   0 ayhan      (501) staff       (20)      365 2024-05-12 11:30:21.000000 bigcode-1.0.8/bigcode/templates/admin/auth/user/add_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)     5541 2024-05-12 11:30:38.000000 bigcode-1.0.8/bigcode/templates/admin/auth/user/change_password.html
--rw-r--r--   0 ayhan      (501) staff       (20)    22276 2024-05-12 11:38:53.000000 bigcode-1.0.8/bigcode/templates/admin/base.html
--rw-r--r--   0 ayhan      (501) staff       (20)       31 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/base_site.html
--rw-r--r--   0 ayhan      (501) staff       (20)     5658 2024-05-12 11:41:05.000000 bigcode-1.0.8/bigcode/templates/admin/change_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)      545 2024-05-11 14:21:40.000000 bigcode-1.0.8/bigcode/templates/admin/change_form_object_tools.html
--rw-r--r--   0 ayhan      (501) staff       (20)     5033 2024-05-11 14:36:21.000000 bigcode-1.0.8/bigcode/templates/admin/change_list.html
--rw-r--r--   0 ayhan      (501) staff       (20)      516 2024-05-11 14:21:24.000000 bigcode-1.0.8/bigcode/templates/admin/change_list_object_tools.html
--rw-r--r--   0 ayhan      (501) staff       (20)     2780 2024-05-11 12:53:10.000000 bigcode-1.0.8/bigcode/templates/admin/change_list_results.html
--rw-r--r--   0 ayhan      (501) staff       (20)      956 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/date_hierarchy.html
--rw-r--r--   0 ayhan      (501) staff       (20)     4117 2024-05-11 14:26:43.000000 bigcode-1.0.8/bigcode/templates/admin/delete_confirmation.html
--rw-r--r--   0 ayhan      (501) staff       (20)     4180 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/delete_selected_confirmation.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.635706 bigcode-1.0.8/bigcode/templates/admin/edit_inline/
--rw-r--r--   0 ayhan      (501) staff       (20)     4360 2024-05-11 10:16:37.000000 bigcode-1.0.8/bigcode/templates/admin/edit_inline/stacked.html
--rw-r--r--   0 ayhan      (501) staff       (20)     6519 2024-05-11 10:16:40.000000 bigcode-1.0.8/bigcode/templates/admin/edit_inline/tabular.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.636175 bigcode-1.0.8/bigcode/templates/admin/filer/
--rw-r--r--   0 ayhan      (501) staff       (20)     1875 2024-05-11 10:17:12.000000 bigcode-1.0.8/bigcode/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1037 2024-05-11 10:17:23.000000 bigcode-1.0.8/bigcode/templates/admin/filer/change_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)     4197 2024-05-11 10:17:26.000000 bigcode-1.0.8/bigcode/templates/admin/filer/delete_selected_files_confirmation.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.636330 bigcode-1.0.8/bigcode/templates/admin/filer/file/
--rw-r--r--   0 ayhan      (501) staff       (20)     1555 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/filer/file/change_form.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.636707 bigcode-1.0.8/bigcode/templates/admin/filer/folder/
--rw-r--r--   0 ayhan      (501) staff       (20)     1871 2024-05-11 10:16:56.000000 bigcode-1.0.8/bigcode/templates/admin/filer/folder/change_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)    14731 2024-05-11 10:16:59.000000 bigcode-1.0.8/bigcode/templates/admin/filer/folder/directory_listing.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.636868 bigcode-1.0.8/bigcode/templates/admin/filer/image/
--rw-r--r--   0 ayhan      (501) staff       (20)     1539 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/filer/image/change_form.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.637017 bigcode-1.0.8/bigcode/templates/admin/filer/tools/
--rw-r--r--   0 ayhan      (501) staff       (20)     2743 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0 ayhan      (501) staff       (20)      592 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/filter.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.638281 bigcode-1.0.8/bigcode/templates/admin/import_export/
--rw-r--r--   0 ayhan      (501) staff       (20)      970 2024-05-11 10:17:53.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/base.html
--rw-r--r--   0 ayhan      (501) staff       (20)      391 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list.html
--rw-r--r--   0 ayhan      (501) staff       (20)      187 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 ayhan      (501) staff       (20)      344 2024-05-11 10:19:55.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 ayhan      (501) staff       (20)      187 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 ayhan      (501) staff       (20)      323 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 ayhan      (501) staff       (20)      301 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 ayhan      (501) staff       (20)     3191 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/export.html
--rw-r--r--   0 ayhan      (501) staff       (20)    13270 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/import_export/import.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.638594 bigcode-1.0.8/bigcode/templates/admin/includes/
--rw-r--r--   0 ayhan      (501) staff       (20)     2725 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/includes/fieldset.html
--rw-r--r--   0 ayhan      (501) staff       (20)      302 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0 ayhan      (501) staff       (20)    11669 2024-05-12 12:24:58.000000 bigcode-1.0.8/bigcode/templates/admin/index.html
--rw-r--r--   0 ayhan      (501) staff       (20)     3455 2024-05-10 14:32:27.000000 bigcode-1.0.8/bigcode/templates/admin/login.html
--rw-r--r--   0 ayhan      (501) staff       (20)      699 2024-05-11 10:24:42.000000 bigcode-1.0.8/bigcode/templates/admin/mptt_filter.html
--rw-r--r--   0 ayhan      (501) staff       (20)     3486 2024-05-12 11:36:24.000000 bigcode-1.0.8/bigcode/templates/admin/object_history.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1037 2024-05-11 14:32:17.000000 bigcode-1.0.8/bigcode/templates/admin/pagination.html
--rw-r--r--   0 ayhan      (501) staff       (20)      610 2024-05-11 10:24:22.000000 bigcode-1.0.8/bigcode/templates/admin/popup_response.html
--rw-r--r--   0 ayhan      (501) staff       (20)     2303 2024-05-11 12:35:50.000000 bigcode-1.0.8/bigcode/templates/admin/search_form.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.638923 bigcode-1.0.8/bigcode/templates/admin/solo/
--rw-r--r--   0 ayhan      (501) staff       (20)      937 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/solo/change_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)      572 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templates/admin/solo/object_history.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1826 2024-05-11 10:24:06.000000 bigcode-1.0.8/bigcode/templates/admin/submit_line.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.584384 bigcode-1.0.8/bigcode/templates/bigcode/
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.640219 bigcode-1.0.8/bigcode/templates/bigcode/includes/
--rw-r--r--   0 ayhan      (501) staff       (20)     1803 2024-05-11 10:23:54.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/carousel.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1153 2024-05-11 10:23:40.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/collapsible.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1321 2024-05-11 10:23:31.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/horizontal_tabs.html
--rw-r--r--   0 ayhan      (501) staff       (20)      611 2024-05-11 10:23:23.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/related_modal.html
--rw-r--r--   0 ayhan      (501) staff       (20)      925 2024-05-11 10:23:13.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/single.html
--rw-r--r--   0 ayhan      (501) staff       (20)    15066 2024-05-11 10:22:45.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/ui_builder_panel.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1449 2024-05-11 10:22:42.000000 bigcode-1.0.8/bigcode/templates/bigcode/includes/vertical_tabs.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.640374 bigcode-1.0.8/bigcode/templates/bigcode/widgets/
--rw-r--r--   0 ayhan      (501) staff       (20)      522 2024-05-11 10:26:27.000000 bigcode-1.0.8/bigcode/templates/bigcode/widgets/select.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.641744 bigcode-1.0.8/bigcode/templates/registration/
--rw-r--r--   0 ayhan      (501) staff       (20)     2943 2024-05-11 10:22:23.000000 bigcode-1.0.8/bigcode/templates/registration/base.html
--rw-r--r--   0 ayhan      (501) staff       (20)      358 2024-05-10 14:43:04.000000 bigcode-1.0.8/bigcode/templates/registration/logged_out.html
--rw-r--r--   0 ayhan      (501) staff       (20)      880 2024-05-10 14:47:21.000000 bigcode-1.0.8/bigcode/templates/registration/password_change_done.html
--rw-r--r--   0 ayhan      (501) staff       (20)     5940 2024-05-11 10:21:48.000000 bigcode-1.0.8/bigcode/templates/registration/password_change_form.html
--rw-r--r--   0 ayhan      (501) staff       (20)      451 2024-05-11 10:21:37.000000 bigcode-1.0.8/bigcode/templates/registration/password_reset_complete.html
--rw-r--r--   0 ayhan      (501) staff       (20)     2641 2024-05-11 10:21:27.000000 bigcode-1.0.8/bigcode/templates/registration/password_reset_confirm.html
--rw-r--r--   0 ayhan      (501) staff       (20)      590 2024-05-11 10:21:17.000000 bigcode-1.0.8/bigcode/templates/registration/password_reset_done.html
--rw-r--r--   0 ayhan      (501) staff       (20)     1635 2024-05-11 10:21:11.000000 bigcode-1.0.8/bigcode/templates/registration/password_reset_form.html
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.642048 bigcode-1.0.8/bigcode/templatetags/
--rw-r--r--   0 ayhan      (501) staff       (20)        0 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templatetags/__init__.py
--rw-r--r--   0 ayhan      (501) staff       (20)    17332 2024-05-10 12:20:38.000000 bigcode-1.0.8/bigcode/templatetags/jazzmin.py
--rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.8/bigcode/utils.py
--rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.8/bigcode/widgets.py
-drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-14 15:05:09.586739 bigcode-1.0.8/bigcode.egg-info/
--rw-r--r--   0 ayhan      (501) staff       (20)      745 2024-05-14 15:05:09.000000 bigcode-1.0.8/bigcode.egg-info/PKG-INFO
--rw-r--r--   0 ayhan      (501) staff       (20)     8161 2024-05-14 15:05:09.000000 bigcode-1.0.8/bigcode.egg-info/SOURCES.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-14 15:05:09.000000 bigcode-1.0.8/bigcode.egg-info/dependency_links.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-14 15:05:09.000000 bigcode-1.0.8/bigcode.egg-info/requires.txt
--rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-14 15:05:09.000000 bigcode-1.0.8/bigcode.egg-info/top_level.txt
--rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-14 15:05:09.642760 bigcode-1.0.8/setup.cfg
--rw-r--r--   0 ayhan      (501) staff       (20)     1052 2024-05-14 15:04:45.000000 bigcode-1.0.8/setup.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.155754 bigcode-1.0.9/
+-rw-r--r--   0 ayhan      (501) staff       (20)      173 2024-05-12 15:17:21.000000 bigcode-1.0.9/MANIFEST.in
+-rw-r--r--   0 ayhan      (501) staff       (20)      745 2024-05-15 19:03:17.155814 bigcode-1.0.9/PKG-INFO
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.121629 bigcode-1.0.9/bigcode/
+-rw-r--r--   0 ayhan      (501) staff       (20)      135 2024-05-15 19:02:35.000000 bigcode-1.0.9/bigcode/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      210 2024-05-11 14:38:15.000000 bigcode-1.0.9/bigcode/apps.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      176 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/compat.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.122404 bigcode-1.0.9/bigcode/locale/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114266 bigcode-1.0.9/bigcode/locale/bg/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.122829 bigcode-1.0.9/bigcode/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     9666 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)    17953 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114370 bigcode-1.0.9/bigcode/locale/de/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.123135 bigcode-1.0.9/bigcode/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1536 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     2486 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114473 bigcode-1.0.9/bigcode/locale/es/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.123370 bigcode-1.0.9/bigcode/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1572 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     2518 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114580 bigcode-1.0.9/bigcode/locale/fr/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.123581 bigcode-1.0.9/bigcode/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     3080 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     3379 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114681 bigcode-1.0.9/bigcode/locale/hu/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.123798 bigcode-1.0.9/bigcode/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2967 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     5327 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.114785 bigcode-1.0.9/bigcode/locale/ru/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.124031 bigcode-1.0.9/bigcode/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2862 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     4142 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.124162 bigcode-1.0.9/bigcode/locale/tk/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/tk/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.126379 bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/.DS_Store
+-rw-r--r--   0 ayhan      (501) staff       (20)    16777 2024-05-15 18:51:29.000000 bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)    15802 2024-05-15 18:51:24.000000 bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.115013 bigcode-1.0.9/bigcode/locale/uz/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.126764 bigcode-1.0.9/bigcode/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     3278 2024-05-15 18:32:16.000000 bigcode-1.0.9/bigcode/locale/uz/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     4458 2024-05-15 18:32:14.000000 bigcode-1.0.9/bigcode/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.115117 bigcode-1.0.9/bigcode/locale/zh_Hans/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.127030 bigcode-1.0.9/bigcode/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1282 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     2085 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.115230 bigcode-1.0.9/bigcode/locale/zh_Hant/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.127277 bigcode-1.0.9/bigcode/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1284 2024-05-12 11:58:05.000000 bigcode-1.0.9/bigcode/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 ayhan      (501) staff       (20)     2088 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 ayhan      (501) staff       (20)    13753 2024-05-11 14:38:45.000000 bigcode-1.0.9/bigcode/settings.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.127403 bigcode-1.0.9/bigcode/static/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 13:17:42.000000 bigcode-1.0.9/bigcode/static/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.128266 bigcode-1.0.9/bigcode/static/admin/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-10 14:16:10.000000 bigcode-1.0.9/bigcode/static/admin/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.128512 bigcode-1.0.9/bigcode/static/admin/js/
+-rw-r--r--   0 ayhan      (501) staff       (20)      564 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/admin/js/cancel.js
+-rw-r--r--   0 ayhan      (501) staff       (20)     1946 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/admin/js/popup_response.js
+-rw-r--r--   0 ayhan      (501) staff       (20)    75842 2024-05-01 18:35:35.000000 bigcode-1.0.9/bigcode/static/admin/logo.png
+-rw-r--r--   0 ayhan      (501) staff       (20)      206 2024-05-10 14:15:38.000000 bigcode-1.0.9/bigcode/static/admin/plus.svg
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.115790 bigcode-1.0.9/bigcode/static/jazzmin/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.128650 bigcode-1.0.9/bigcode/static/jazzmin/css/
+-rw-r--r--   0 ayhan      (501) staff       (20)    16969 2024-05-11 10:58:51.000000 bigcode-1.0.9/bigcode/static/jazzmin/css/main.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.129584 bigcode-1.0.9/bigcode/static/jazzmin/img/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1094 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/calendar-icons.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)   223437 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/default-log.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)     7070 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/default.jpg
+-rw-r--r--   0 ayhan      (501) staff       (20)     1086 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/icon-calendar.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)      380 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/icon-changelink.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)     3291 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/img/selector-icons.svg
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.130216 bigcode-1.0.9/bigcode/static/jazzmin/js/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6052 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/js/change_form.js
+-rw-r--r--   0 ayhan      (501) staff       (20)     2252 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/js/change_list.js
+-rw-r--r--   0 ayhan      (501) staff       (20)     2391 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/js/main.js
+-rw-r--r--   0 ayhan      (501) staff       (20)     6258 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/js/related-modal.js
+-rw-r--r--   0 ayhan      (501) staff       (20)    13873 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/js/ui-builder.js
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.115833 bigcode-1.0.9/bigcode/static/jazzmin/plugins/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.130393 bigcode-1.0.9/bigcode/static/jazzmin/plugins/bootstrap-show-modal/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2756 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.130522 bigcode-1.0.9/bigcode/static/vendor/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 13:17:31.000000 bigcode-1.0.9/bigcode/static/vendor/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.130787 bigcode-1.0.9/bigcode/static/vendor/adminlte/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-11 11:55:19.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.131861 bigcode-1.0.9/bigcode/static/vendor/adminlte/css/
+-rw-r--r--   0 ayhan      (501) staff       (20)  1382975 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/css/adminlte.min.css
+-rw-r--r--   0 ayhan      (501) staff       (20)  3783107 2024-05-12 11:44:51.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/css/adminlte.min.css.map
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.137899 bigcode-1.0.9/bigcode/static/vendor/adminlte/img/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2637 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/img/AdminLTELogo.png
+-rw-r--r--   0 ayhan      (501) staff       (20)     1139 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/img/icons.png
+-rw-r--r--   0 ayhan      (501) staff       (20)     5357 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/img/user2-160x160.jpg
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.138373 bigcode-1.0.9/bigcode/static/vendor/adminlte/js/
+-rw-r--r--   0 ayhan      (501) staff       (20)    44244 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/js/adminlte.min.js
+-rw-r--r--   0 ayhan      (501) staff       (20)   129651 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/adminlte/js/adminlte.min.js.map
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.116276 bigcode-1.0.9/bigcode/static/vendor/bootstrap/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.138709 bigcode-1.0.9/bigcode/static/vendor/bootstrap/js/
+-rw-r--r--   0 ayhan      (501) staff       (20)    62440 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 ayhan      (501) staff       (20)   187646 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.118604 bigcode-1.0.9/bigcode/static/vendor/bootswatch/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.138957 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cerulean/
+-rw-r--r--   0 ayhan      (501) staff       (20)   163350 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cerulean/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.139167 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cosmo/
+-rw-r--r--   0 ayhan      (501) staff       (20)   154456 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cosmo/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.139364 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cyborg/
+-rw-r--r--   0 ayhan      (501) staff       (20)   164597 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/cyborg/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.139567 bigcode-1.0.9/bigcode/static/vendor/bootswatch/darkly/
+-rw-r--r--   0 ayhan      (501) staff       (20)   164202 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/darkly/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.139777 bigcode-1.0.9/bigcode/static/vendor/bootswatch/default/
+-rw-r--r--   0 ayhan      (501) staff       (20)   161972 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/default/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.139968 bigcode-1.0.9/bigcode/static/vendor/bootswatch/flatly/
+-rw-r--r--   0 ayhan      (501) staff       (20)   164819 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/flatly/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.140181 bigcode-1.0.9/bigcode/static/vendor/bootswatch/journal/
+-rw-r--r--   0 ayhan      (501) staff       (20)   161735 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/journal/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.140375 bigcode-1.0.9/bigcode/static/vendor/bootswatch/litera/
+-rw-r--r--   0 ayhan      (501) staff       (20)   165148 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/litera/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.140570 bigcode-1.0.9/bigcode/static/vendor/bootswatch/lumen/
+-rw-r--r--   0 ayhan      (501) staff       (20)   167943 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/lumen/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.140771 bigcode-1.0.9/bigcode/static/vendor/bootswatch/lux/
+-rw-r--r--   0 ayhan      (501) staff       (20)   155932 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/lux/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.140991 bigcode-1.0.9/bigcode/static/vendor/bootswatch/materia/
+-rw-r--r--   0 ayhan      (501) staff       (20)   194473 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/materia/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.141224 bigcode-1.0.9/bigcode/static/vendor/bootswatch/minty/
+-rw-r--r--   0 ayhan      (501) staff       (20)   165946 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/minty/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.141425 bigcode-1.0.9/bigcode/static/vendor/bootswatch/pulse/
+-rw-r--r--   0 ayhan      (501) staff       (20)   155889 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/pulse/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.141613 bigcode-1.0.9/bigcode/static/vendor/bootswatch/sandstone/
+-rw-r--r--   0 ayhan      (501) staff       (20)   163543 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/sandstone/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.141800 bigcode-1.0.9/bigcode/static/vendor/bootswatch/simplex/
+-rw-r--r--   0 ayhan      (501) staff       (20)   163234 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/simplex/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.142014 bigcode-1.0.9/bigcode/static/vendor/bootswatch/sketchy/
+-rw-r--r--   0 ayhan      (501) staff       (20)   167043 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/sketchy/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.142238 bigcode-1.0.9/bigcode/static/vendor/bootswatch/slate/
+-rw-r--r--   0 ayhan      (501) staff       (20)   171632 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/slate/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.142435 bigcode-1.0.9/bigcode/static/vendor/bootswatch/solar/
+-rw-r--r--   0 ayhan      (501) staff       (20)   169219 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/solar/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.142630 bigcode-1.0.9/bigcode/static/vendor/bootswatch/spacelab/
+-rw-r--r--   0 ayhan      (501) staff       (20)   164894 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/spacelab/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.142826 bigcode-1.0.9/bigcode/static/vendor/bootswatch/superhero/
+-rw-r--r--   0 ayhan      (501) staff       (20)   164559 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/superhero/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.143031 bigcode-1.0.9/bigcode/static/vendor/bootswatch/united/
+-rw-r--r--   0 ayhan      (501) staff       (20)   161367 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/united/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.143263 bigcode-1.0.9/bigcode/static/vendor/bootswatch/yeti/
+-rw-r--r--   0 ayhan      (501) staff       (20)   168497 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/bootswatch/yeti/bootstrap.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.118845 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.143473 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/css/
+-rw-r--r--   0 ayhan      (501) staff       (20)    59344 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/css/all.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.146604 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/
+-rw-r--r--   0 ayhan      (501) staff       (20)   134346 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
+-rw-r--r--   0 ayhan      (501) staff       (20)   747545 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)   134040 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 ayhan      (501) staff       (20)    90060 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
+-rw-r--r--   0 ayhan      (501) staff       (20)    76764 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 ayhan      (501) staff       (20)    34034 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
+-rw-r--r--   0 ayhan      (501) staff       (20)   144714 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)    33736 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 ayhan      (501) staff       (20)    16276 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
+-rw-r--r--   0 ayhan      (501) staff       (20)    13276 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 ayhan      (501) staff       (20)   203030 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
+-rw-r--r--   0 ayhan      (501) staff       (20)   918991 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
+-rw-r--r--   0 ayhan      (501) staff       (20)   202744 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 ayhan      (501) staff       (20)   101652 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
+-rw-r--r--   0 ayhan      (501) staff       (20)    78196 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.119112 bigcode-1.0.9/bigcode/static/vendor/select2/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.146757 bigcode-1.0.9/bigcode/static/vendor/select2/css/
+-rw-r--r--   0 ayhan      (501) staff       (20)    16264 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/select2/css/select2.min.css
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.146875 bigcode-1.0.9/bigcode/static/vendor/select2/js/
+-rw-r--r--   0 ayhan      (501) staff       (20)    73170 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/static/vendor/select2/js/select2.min.js
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.147016 bigcode-1.0.9/bigcode/templates/
+-rw-r--r--   0 ayhan      (501) staff       (20)     6148 2024-05-12 14:21:10.000000 bigcode-1.0.9/bigcode/templates/.DS_Store
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.149897 bigcode-1.0.9/bigcode/templates/admin/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1551 2024-05-11 12:33:43.000000 bigcode-1.0.9/bigcode/templates/admin/actions.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      517 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/app_index.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.119428 bigcode-1.0.9/bigcode/templates/admin/auth/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.150129 bigcode-1.0.9/bigcode/templates/admin/auth/user/
+-rw-r--r--   0 ayhan      (501) staff       (20)      365 2024-05-12 11:30:21.000000 bigcode-1.0.9/bigcode/templates/admin/auth/user/add_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     5541 2024-05-12 11:30:38.000000 bigcode-1.0.9/bigcode/templates/admin/auth/user/change_password.html
+-rw-r--r--   0 ayhan      (501) staff       (20)    22867 2024-05-15 18:29:36.000000 bigcode-1.0.9/bigcode/templates/admin/base.html
+-rw-r--r--   0 ayhan      (501) staff       (20)       31 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/base_site.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     5658 2024-05-12 11:41:05.000000 bigcode-1.0.9/bigcode/templates/admin/change_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      545 2024-05-11 14:21:40.000000 bigcode-1.0.9/bigcode/templates/admin/change_form_object_tools.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     5033 2024-05-11 14:36:21.000000 bigcode-1.0.9/bigcode/templates/admin/change_list.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      516 2024-05-11 14:21:24.000000 bigcode-1.0.9/bigcode/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     2780 2024-05-11 12:53:10.000000 bigcode-1.0.9/bigcode/templates/admin/change_list_results.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      956 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/date_hierarchy.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     4117 2024-05-11 14:26:43.000000 bigcode-1.0.9/bigcode/templates/admin/delete_confirmation.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     4180 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/delete_selected_confirmation.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.150358 bigcode-1.0.9/bigcode/templates/admin/edit_inline/
+-rw-r--r--   0 ayhan      (501) staff       (20)     4360 2024-05-11 10:16:37.000000 bigcode-1.0.9/bigcode/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     6519 2024-05-11 10:16:40.000000 bigcode-1.0.9/bigcode/templates/admin/edit_inline/tabular.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.150723 bigcode-1.0.9/bigcode/templates/admin/filer/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1875 2024-05-11 10:17:12.000000 bigcode-1.0.9/bigcode/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1037 2024-05-11 10:17:23.000000 bigcode-1.0.9/bigcode/templates/admin/filer/change_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     4197 2024-05-11 10:17:26.000000 bigcode-1.0.9/bigcode/templates/admin/filer/delete_selected_files_confirmation.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.150858 bigcode-1.0.9/bigcode/templates/admin/filer/file/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1555 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/filer/file/change_form.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.151089 bigcode-1.0.9/bigcode/templates/admin/filer/folder/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1871 2024-05-11 10:16:56.000000 bigcode-1.0.9/bigcode/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)    14731 2024-05-11 10:16:59.000000 bigcode-1.0.9/bigcode/templates/admin/filer/folder/directory_listing.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.151199 bigcode-1.0.9/bigcode/templates/admin/filer/image/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1539 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/filer/image/change_form.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.151307 bigcode-1.0.9/bigcode/templates/admin/filer/tools/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2743 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      592 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/filter.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.152582 bigcode-1.0.9/bigcode/templates/admin/import_export/
+-rw-r--r--   0 ayhan      (501) staff       (20)      970 2024-05-11 10:17:53.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/base.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      391 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      187 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      344 2024-05-11 10:19:55.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      187 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      323 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      301 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     3191 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/export.html
+-rw-r--r--   0 ayhan      (501) staff       (20)    13270 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/import_export/import.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.152875 bigcode-1.0.9/bigcode/templates/admin/includes/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2725 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/includes/fieldset.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      302 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0 ayhan      (501) staff       (20)    11669 2024-05-12 12:24:58.000000 bigcode-1.0.9/bigcode/templates/admin/index.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     3455 2024-05-10 14:32:27.000000 bigcode-1.0.9/bigcode/templates/admin/login.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      699 2024-05-11 10:24:42.000000 bigcode-1.0.9/bigcode/templates/admin/mptt_filter.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     3486 2024-05-12 11:36:24.000000 bigcode-1.0.9/bigcode/templates/admin/object_history.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1037 2024-05-11 14:32:17.000000 bigcode-1.0.9/bigcode/templates/admin/pagination.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      610 2024-05-11 10:24:22.000000 bigcode-1.0.9/bigcode/templates/admin/popup_response.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     2303 2024-05-11 12:35:50.000000 bigcode-1.0.9/bigcode/templates/admin/search_form.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.153135 bigcode-1.0.9/bigcode/templates/admin/solo/
+-rw-r--r--   0 ayhan      (501) staff       (20)      937 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/solo/change_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      572 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templates/admin/solo/object_history.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1826 2024-05-11 10:24:06.000000 bigcode-1.0.9/bigcode/templates/admin/submit_line.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.120362 bigcode-1.0.9/bigcode/templates/bigcode/
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.154112 bigcode-1.0.9/bigcode/templates/bigcode/includes/
+-rw-r--r--   0 ayhan      (501) staff       (20)     1803 2024-05-11 10:23:54.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/carousel.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1153 2024-05-11 10:23:40.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/collapsible.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1321 2024-05-11 10:23:31.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/horizontal_tabs.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      611 2024-05-11 10:23:23.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/related_modal.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      925 2024-05-11 10:23:13.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/single.html
+-rw-r--r--   0 ayhan      (501) staff       (20)    15066 2024-05-11 10:22:45.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/ui_builder_panel.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1449 2024-05-11 10:22:42.000000 bigcode-1.0.9/bigcode/templates/bigcode/includes/vertical_tabs.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.154255 bigcode-1.0.9/bigcode/templates/bigcode/widgets/
+-rw-r--r--   0 ayhan      (501) staff       (20)      522 2024-05-11 10:26:27.000000 bigcode-1.0.9/bigcode/templates/bigcode/widgets/select.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.155363 bigcode-1.0.9/bigcode/templates/registration/
+-rw-r--r--   0 ayhan      (501) staff       (20)     2943 2024-05-11 10:22:23.000000 bigcode-1.0.9/bigcode/templates/registration/base.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      358 2024-05-10 14:43:04.000000 bigcode-1.0.9/bigcode/templates/registration/logged_out.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      880 2024-05-10 14:47:21.000000 bigcode-1.0.9/bigcode/templates/registration/password_change_done.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     5940 2024-05-11 10:21:48.000000 bigcode-1.0.9/bigcode/templates/registration/password_change_form.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      451 2024-05-11 10:21:37.000000 bigcode-1.0.9/bigcode/templates/registration/password_reset_complete.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     2641 2024-05-11 10:21:27.000000 bigcode-1.0.9/bigcode/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 ayhan      (501) staff       (20)      590 2024-05-11 10:21:17.000000 bigcode-1.0.9/bigcode/templates/registration/password_reset_done.html
+-rw-r--r--   0 ayhan      (501) staff       (20)     1635 2024-05-11 10:21:11.000000 bigcode-1.0.9/bigcode/templates/registration/password_reset_form.html
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.155608 bigcode-1.0.9/bigcode/templatetags/
+-rw-r--r--   0 ayhan      (501) staff       (20)        0 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templatetags/__init__.py
+-rw-r--r--   0 ayhan      (501) staff       (20)    17332 2024-05-10 12:20:38.000000 bigcode-1.0.9/bigcode/templatetags/jazzmin.py
+-rw-r--r--   0 ayhan      (501) staff       (20)     7813 2024-05-11 14:39:24.000000 bigcode-1.0.9/bigcode/utils.py
+-rw-r--r--   0 ayhan      (501) staff       (20)      803 2024-05-11 14:39:40.000000 bigcode-1.0.9/bigcode/widgets.py
+drwxr-xr-x   0 ayhan      (501) staff       (20)        0 2024-05-15 19:03:17.122281 bigcode-1.0.9/bigcode.egg-info/
+-rw-r--r--   0 ayhan      (501) staff       (20)      745 2024-05-15 19:03:17.000000 bigcode-1.0.9/bigcode.egg-info/PKG-INFO
+-rw-r--r--   0 ayhan      (501) staff       (20)     8161 2024-05-15 19:03:17.000000 bigcode-1.0.9/bigcode.egg-info/SOURCES.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        1 2024-05-15 19:03:17.000000 bigcode-1.0.9/bigcode.egg-info/dependency_links.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       12 2024-05-15 19:03:17.000000 bigcode-1.0.9/bigcode.egg-info/requires.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)        8 2024-05-15 19:03:17.000000 bigcode-1.0.9/bigcode.egg-info/top_level.txt
+-rw-r--r--   0 ayhan      (501) staff       (20)       38 2024-05-15 19:03:17.155994 bigcode-1.0.9/setup.cfg
+-rw-r--r--   0 ayhan      (501) staff       (20)     1052 2024-05-15 19:02:52.000000 bigcode-1.0.9/setup.py
```

### Comparing `bigcode-1.0.8/PKG-INFO` & `bigcode-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigcode
-Version: 1.0.8
+Version: 1.0.9
 Summary: A custom admin interface for Django inspired by the Django Jazzmin.
 Home-page: https://github.com/ayhandev/bigcode_adminstration
 Download-URL: https://github.com/ayhandev/bigcode_adminstration.git
 Author: ayhan
 Author-email: jumanyyazowayhan32@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigcode-1.0.8/bigcode/locale/.DS_Store` & `bigcode-1.0.9/bigcode/locale/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/bg/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/bg/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/de/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/de/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/es/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/es/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/fr/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/fr/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/hu/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/hu/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/ru/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/ru/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/tk/.DS_Store` & `bigcode-1.0.9/bigcode/locale/tk/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/.DS_Store` & `bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -968,14 +968,17 @@
 
 msgid "Upload Files"
 msgstr "Faýllary Ýüklemek"
 
 msgid "Users"
 msgstr "Ulanyjylar"
 
+msgid "VIEW SITE"
+msgstr "SAÝTA BARYP GÖRÜÑ"
+
 msgid "Vagabonds"
 msgstr "Aýlanyp ýörenler"
 
 msgid "Vendors"
 msgstr "Söwdagärler"
 
 msgid "Version"
```

### Comparing `bigcode-1.0.8/bigcode/locale/tk/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/tk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1026,8 +1026,11 @@
 msgid "Changed Name."
 msgstr "Üýtgedilen at."
 
 msgid "Django Administration"
 msgstr "Django administrasiýasy"
 
 msgid "Version"
-msgstr "wersiýa"
+msgstr "wersiýa"
+
+msgid "VIEW SITE"
+msgstr "SAÝTA BARYP GÖRÜÑ"
```

### Comparing `bigcode-1.0.8/bigcode/locale/uz/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/uz/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -103,14 +103,17 @@
 msgstr ""
 "Ushbu ob'ektda o'zgarishlar tarixi yo'q. Bu administrator paneli orqali "
 "qo'shilmagan bo'lishi mumkin."
 
 msgid "UI Configuration"
 msgstr "UI sozlamalari"
 
+msgid "VIEW SITE"
+msgstr "SAYTNI KO'RISH"
+
 msgid ""
 "View function: <code>%(full_name)s</code>. Name: <code>%(url_name)s</code>."
 msgstr ""
 "Taqdimot funktsiyasi: <code>%(full_name)s</code>. Nomi: <code>%(url_name)s</"
 "code>."
 
 msgid "Views by empty namespace"
```

### Comparing `bigcode-1.0.8/bigcode/locale/uz/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/uz/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -162,8 +162,11 @@
 msgid "staff status"
 msgstr "xodimlar holati"
 
 msgid "Last name"
 msgstr "Familiya"
 
 msgid "Old password"
-msgstr "Eski parol"
+msgstr "Eski parol"
+
+msgid "VIEW SITE"
+msgstr "SAYTNI KO'RISH"
```

### Comparing `bigcode-1.0.8/bigcode/locale/zh_Hans/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/zh_Hans/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/zh_Hant/LC_MESSAGES/django.mo` & `bigcode-1.0.9/bigcode/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/locale/zh_Hant/LC_MESSAGES/django.po` & `bigcode-1.0.9/bigcode/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/settings.py` & `bigcode-1.0.9/bigcode/settings.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/.DS_Store` & `bigcode-1.0.9/bigcode/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/admin/.DS_Store` & `bigcode-1.0.9/bigcode/static/admin/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/admin/js/cancel.js` & `bigcode-1.0.9/bigcode/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/admin/js/popup_response.js` & `bigcode-1.0.9/bigcode/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/admin/logo.png` & `bigcode-1.0.9/bigcode/static/admin/logo.png`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/css/main.css` & `bigcode-1.0.9/bigcode/static/jazzmin/css/main.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/img/calendar-icons.svg` & `bigcode-1.0.9/bigcode/static/jazzmin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/img/default-log.svg` & `bigcode-1.0.9/bigcode/static/jazzmin/img/default-log.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/img/default.jpg` & `bigcode-1.0.9/bigcode/static/jazzmin/img/default.jpg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/img/icon-calendar.svg` & `bigcode-1.0.9/bigcode/static/jazzmin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/img/selector-icons.svg` & `bigcode-1.0.9/bigcode/static/jazzmin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/js/change_form.js` & `bigcode-1.0.9/bigcode/static/jazzmin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/js/change_list.js` & `bigcode-1.0.9/bigcode/static/jazzmin/js/change_list.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/js/main.js` & `bigcode-1.0.9/bigcode/static/jazzmin/js/main.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/js/related-modal.js` & `bigcode-1.0.9/bigcode/static/jazzmin/js/related-modal.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/js/ui-builder.js` & `bigcode-1.0.9/bigcode/static/jazzmin/js/ui-builder.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js` & `bigcode-1.0.9/bigcode/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/.DS_Store` & `bigcode-1.0.9/bigcode/static/vendor/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/.DS_Store` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/css/adminlte.min.css` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/css/adminlte.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/css/adminlte.min.css.map` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/css/adminlte.min.css.map`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/img/AdminLTELogo.png` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/img/AdminLTELogo.png`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/img/icons.png` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/img/icons.png`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/img/user2-160x160.jpg` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/img/user2-160x160.jpg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/js/adminlte.min.js` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/adminlte/js/adminlte.min.js.map` & `bigcode-1.0.9/bigcode/static/vendor/adminlte/js/adminlte.min.js.map`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootstrap/js/bootstrap.min.js` & `bigcode-1.0.9/bigcode/static/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootstrap/js/bootstrap.min.js.map` & `bigcode-1.0.9/bigcode/static/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/cerulean/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/cerulean/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/cosmo/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/cosmo/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/cyborg/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/cyborg/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/darkly/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/default/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/default/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/flatly/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/journal/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/journal/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/litera/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/litera/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/lumen/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/lumen/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/lux/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/lux/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/materia/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/minty/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/minty/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/pulse/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/pulse/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/sandstone/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/sandstone/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/simplex/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/simplex/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/sketchy/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/sketchy/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/slate/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/solar/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/solar/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/spacelab/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/spacelab/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/superhero/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/superhero/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/united/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/united/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/bootswatch/yeti/bootstrap.min.css` & `bigcode-1.0.9/bigcode/static/vendor/bootswatch/yeti/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/css/all.min.css` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `bigcode-1.0.9/bigcode/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/select2/css/select2.min.css` & `bigcode-1.0.9/bigcode/static/vendor/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/static/vendor/select2/js/select2.min.js` & `bigcode-1.0.9/bigcode/static/vendor/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/.DS_Store` & `bigcode-1.0.9/bigcode/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/actions.html` & `bigcode-1.0.9/bigcode/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/app_index.html` & `bigcode-1.0.9/bigcode/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/auth/user/change_password.html` & `bigcode-1.0.9/bigcode/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/base.html` & `bigcode-1.0.9/bigcode/templates/admin/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 <body  class="hold-transition{% if not jazzmin_settings.show_sidebar %} no-sidebar{% else %} sidebar-mini{% endif %} {% sidebar_status request %} {% if is_popup %}popup {% endif %}{% block bodyclass %}{% endblock %} {{ jazzmin_ui.body_classes }} {% if jazzmin_ui.dark_mode_theme %}theme-dark{% endif %}" data-admin-utc-offset="{% now "Z" %}">
 
 <div class="wrapper amon">
 
     {% if not is_popup %}
         <nav class="main-header navbar navbar-expand {{ jazzmin_ui.navbar_classes }}" id="jazzy-navbar" >
             <ul class="navbar-nav">
-
                 {% if jazzmin_settings.show_sidebar %}
                     <li class="nav-item">
                         <a class="nav-link" data-widget="pushmenu" href="#" role="button"><i class="fas fa-bars"></i></a>
                     </li>
                 {% else %}
                     <li class="nav-item">
                         <a href="{% url 'admin:index' %}" class="brand-link">
@@ -104,14 +103,37 @@
                         {% else %}
                             <a href="{{ link.url }}" class="nav-link" {% if link.new_window %}target="_blank"{% endif %}>{{ link.name }}</a>
                         {% endif %}
                     </li>
                 {% endfor %}
             </ul>
 
+           <style>
+    /* CSS */
+    .navbar-nav .nav-item .nav-link.return-to-site {
+        border-bottom: 2px solid transparent;
+        display: inline-block;
+        padding-bottom: 5px;
+        transition: border-bottom 0.3s, transform 0.3s;
+    }
+
+    .navbar-nav .nav-item .nav-link.return-to-site:hover {
+        border-bottom: 2px solid orange;
+        transform: scale(1.05);
+    }
+</style>
+
+<ul class="navbar-nav flex-fill justify-content-center">
+    <li class="nav-item">
+        <b class="nav-link return-to-site"><a href="/">{% trans 'VIEW SITE' %}</a></b>
+    </li>
+</ul>
+
+
+
             {% if jazzmin_settings.search_model %}
                 {% for search_model in jazzmin_settings.search_models_parsed %}
                     <form action="{{ search_model.search_url }}" method="GET" class="form-inline ml-3">
                         <div class="input-group input-group-sm">
                             <input class="form-control form-control-navbar" name="q" type="search" placeholder="{% trans 'Search' %} {{ search_model.search_name }}..." aria-label="{% trans 'Search' %} {{ search_model.search_name }}...">
                             <div class="input-group-append">
                                 <button class="btn btn-navbar" type="submit">
@@ -120,15 +142,14 @@
                             </div>
                         </div>
                     </form>
                 {% endfor %}
             {% endif %}
 
             <ul class="navbar-nav ml-auto">
-
                 {% if jazzmin_settings.show_ui_builder %}
                 <li class="nav-item">
                     <a class="nav-link" data-widget="control-sidebar" data-slide="true" href="#" role="button">
                         <i class="fas fa-th-large"></i>
                     </a>
                 </li>
                 {% endif %}
@@ -219,14 +240,15 @@
                         <div class="dropdown-divider"></div>
                         {% if perms|can_view_self %}
                             <a href="{% jazzy_admin_url request.user request.current_app|default:"admin" %}" class="dropdown-item dropdown-footer">{% trans 'See Profile' %}</a>
                         {% endif %}
                     </div>
                 </li>
             </ul>
+
         </nav>
         {% block sidebar %}
         {% if jazzmin_settings.show_sidebar %}
             {% get_side_menu as side_menu_list %}
             <style>
                 #jazzy-sidebar {
                     background-color: #0000008e;
```

#### html2text {}

```diff
@@ -22,14 +22,15 @@
       {% for child in link.children %}
       % if link.new_window %}target="_blank"{% endif %}>{{ child.name }}
  {% endfor %}
 {% else %}
 % if link.new_window %}target="_blank"{% endif %}>{{ link.name }}
  {% endif %}
 {% endfor %}
+    * _{{_%%_ _tt_rr_aa_nn_ss_ _''_VV_II_EE_WW_ _SS_II_TT_EE_''_ _%%_}}
 {% if jazzmin_settings.search_model %} {% for search_model in
 jazzmin_settings.search_models_parsed %}
 [Unknown INPUT type]
 {% endfor %} {% endif %}
     * {% if jazzmin_settings.show_ui_builder %}
     * {% endif %} {% if 'django.contrib.admindocs'|app_is_installed %}
     * {% endif %} {% if jazzmin_settings.language_chooser %} {%
```

### Comparing `bigcode-1.0.8/bigcode/templates/admin/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/change_form_object_tools.html` & `bigcode-1.0.9/bigcode/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/change_list.html` & `bigcode-1.0.9/bigcode/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/change_list_object_tools.html` & `bigcode-1.0.9/bigcode/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/change_list_results.html` & `bigcode-1.0.9/bigcode/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/date_hierarchy.html` & `bigcode-1.0.9/bigcode/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/delete_confirmation.html` & `bigcode-1.0.9/bigcode/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/delete_selected_confirmation.html` & `bigcode-1.0.9/bigcode/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/edit_inline/stacked.html` & `bigcode-1.0.9/bigcode/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/edit_inline/tabular.html` & `bigcode-1.0.9/bigcode/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/breadcrumbs.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/delete_selected_files_confirmation.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/file/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/folder/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/folder/directory_listing.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/folder/directory_listing.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/image/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filer/tools/detail_info.html` & `bigcode-1.0.9/bigcode/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/filter.html` & `bigcode-1.0.9/bigcode/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/import_export/base.html` & `bigcode-1.0.9/bigcode/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/import_export/export.html` & `bigcode-1.0.9/bigcode/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/import_export/import.html` & `bigcode-1.0.9/bigcode/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/includes/fieldset.html` & `bigcode-1.0.9/bigcode/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/index.html` & `bigcode-1.0.9/bigcode/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/login.html` & `bigcode-1.0.9/bigcode/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/mptt_filter.html` & `bigcode-1.0.9/bigcode/templates/admin/mptt_filter.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/object_history.html` & `bigcode-1.0.9/bigcode/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/pagination.html` & `bigcode-1.0.9/bigcode/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/popup_response.html` & `bigcode-1.0.9/bigcode/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/search_form.html` & `bigcode-1.0.9/bigcode/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/solo/change_form.html` & `bigcode-1.0.9/bigcode/templates/admin/solo/change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/solo/object_history.html` & `bigcode-1.0.9/bigcode/templates/admin/solo/object_history.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/admin/submit_line.html` & `bigcode-1.0.9/bigcode/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/carousel.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/carousel.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/collapsible.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/collapsible.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/horizontal_tabs.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/horizontal_tabs.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/related_modal.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/related_modal.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/single.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/single.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/ui_builder_panel.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/ui_builder_panel.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/includes/vertical_tabs.html` & `bigcode-1.0.9/bigcode/templates/bigcode/includes/vertical_tabs.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/bigcode/widgets/select.html` & `bigcode-1.0.9/bigcode/templates/bigcode/widgets/select.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/base.html` & `bigcode-1.0.9/bigcode/templates/registration/base.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/password_change_done.html` & `bigcode-1.0.9/bigcode/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/password_change_form.html` & `bigcode-1.0.9/bigcode/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/password_reset_confirm.html` & `bigcode-1.0.9/bigcode/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/password_reset_done.html` & `bigcode-1.0.9/bigcode/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templates/registration/password_reset_form.html` & `bigcode-1.0.9/bigcode/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/templatetags/jazzmin.py` & `bigcode-1.0.9/bigcode/templatetags/jazzmin.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/utils.py` & `bigcode-1.0.9/bigcode/utils.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode/widgets.py` & `bigcode-1.0.9/bigcode/widgets.py`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/bigcode.egg-info/PKG-INFO` & `bigcode-1.0.9/bigcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigcode
-Version: 1.0.8
+Version: 1.0.9
 Summary: A custom admin interface for Django inspired by the Django Jazzmin.
 Home-page: https://github.com/ayhandev/bigcode_adminstration
 Download-URL: https://github.com/ayhandev/bigcode_adminstration.git
 Author: ayhan
 Author-email: jumanyyazowayhan32@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigcode-1.0.8/bigcode.egg-info/SOURCES.txt` & `bigcode-1.0.9/bigcode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigcode-1.0.8/setup.py` & `bigcode-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.8'
+version = '1.0.9'
 
 long_description = """Python module for BIGCODE management platform (BIGCODE wrapper)"""
 
 setup(
     name='bigcode',
     version=version,
     author='ayhan',
```

