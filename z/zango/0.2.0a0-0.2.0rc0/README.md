# Comparing `tmp/zango-0.2.0a0.tar.gz` & `tmp/zango-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zango-0.2.0a0.tar", last modified: Tue May 14 06:15:58 2024, max compression
+gzip compressed data, was "zango-0.2.0rc0.tar", last modified: Wed May 15 11:29:27 2024, max compression
```

## Comparing `zango-0.2.0a0.tar` & `zango-0.2.0rc0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.401527 zango-0.2.0a0/
--rw-r--r--   0 harshshah   (501) staff       (20)    10878 2024-03-05 18:32:15.000000 zango-0.2.0a0/LICENSE
--rw-r--r--   0 harshshah   (501) staff       (20)     5116 2024-05-14 06:15:58.399274 zango-0.2.0a0/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     3512 2024-05-08 12:44:20.000000 zango-0.2.0a0/README.md
--rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-14 06:15:58.401841 zango-0.2.0a0/setup.cfg
--rw-r--r--   0 harshshah   (501) staff       (20)     1446 2024-05-14 06:13:46.000000 zango-0.2.0a0/setup.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.104233 zango-0.2.0a0/src/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.396363 zango-0.2.0a0/src/zango.egg-info/
--rw-r--r--   0 harshshah   (501) staff       (20)     5116 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     9014 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/SOURCES.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/dependency_links.txt
--rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/entry_points.txt
--rw-r--r--   0 harshshah   (501) staff       (20)      677 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/requires.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-14 06:15:56.000000 zango-0.2.0a0/src/zango.egg-info/top_level.txt
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.122919 zango-0.2.0a0/src/zcore/
--rw-r--r--   0 harshshah   (501) staff       (20)       41 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.123255 zango-0.2.0a0/src/zcore/api/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.123806 zango-0.2.0a0/src/zcore/api/app_auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.124235 zango-0.2.0a0/src/zcore/api/app_auth/profile/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.125764 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2753 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/app_auth/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.126313 zango-0.2.0a0/src/zcore/api/platform/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.126781 zango-0.2.0a0/src/zcore/api/platform/auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.129109 zango-0.2.0a0/src/zcore/api/platform/auth/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/auth/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/auth/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/auth/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6079 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/auth/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.129531 zango-0.2.0a0/src/zcore/api/platform/codeassist/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/codeassist/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.130635 zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)    11926 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.130895 zango-0.2.0a0/src/zcore/api/platform/packages/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/packages/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.132072 zango-0.2.0a0/src/zcore/api/platform/packages/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/packages/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/packages/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2601 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/packages/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.132478 zango-0.2.0a0/src/zcore/api/platform/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/permissions/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.136923 zango-0.2.0a0/src/zcore/api/platform/permissions/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/permissions/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/permissions/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/permissions/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6507 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/permissions/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.137597 zango-0.2.0a0/src/zcore/api/platform/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tasks/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.146552 zango-0.2.0a0/src/zcore/api/platform/tasks/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tasks/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tasks/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tasks/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4914 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/tasks/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.147379 zango-0.2.0a0/src/zcore/api/platform/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tenancy/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.148824 zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1926 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)    21220 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      291 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/api/platform/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.149483 zango-0.2.0a0/src/zcore/apps/
--rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.153947 zango-0.2.0a0/src/zcore/apps/appauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.158154 zango-0.2.0a0/src/zcore/apps/appauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0002_default_user_roles.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0004_oldpasswords.py
--rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0005_remove_appusermodel_user.py
--rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/0006_appusermodel_app_objects.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     9188 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/appauth/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.160207 zango-0.2.0a0/src/zcore/apps/appauth/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/templates/app.html
--rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/templates/app_login_signup.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/appauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.165349 zango-0.2.0a0/src/zcore/apps/dynamic_models/
--rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      950 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.165613 zango-0.2.0a0/src/zcore/apps/dynamic_models/fields/
--rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/fields/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.165926 zango-0.2.0a0/src/zcore/apps/dynamic_models/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.166377 zango-0.2.0a0/src/zcore/apps/dynamic_models/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/management/commands/reload_tenant.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.167479 zango-0.2.0a0/src/zcore/apps/dynamic_models/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    15486 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)      567 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/registry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      385 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.167671 zango-0.2.0a0/src/zcore/apps/dynamic_models/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)    29339 2024-05-08 05:13:42.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/templates/default_landing.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.168872 zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    17473 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/lifecycle.py
--rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/wtree.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.171285 zango-0.2.0a0/src/zcore/apps/object_store/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.172071 zango-0.2.0a0/src/zcore/apps/object_store/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/object_store/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.178816 zango-0.2.0a0/src/zcore/apps/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.183214 zango-0.2.0a0/src/zcore/apps/permissions/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/migrations/0003_default_policy.py
--rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5050 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/mixin.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3748 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/permissions/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.183837 zango-0.2.0a0/src/zcore/apps/shared/
--rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.190122 zango-0.2.0a0/src/zcore/apps/shared/platformauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2578 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/abstract_model.py
--rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.192246 zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7168 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/models.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.113937 zango-0.2.0a0/src/zcore/apps/shared/platformauth/templates/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.193193 zango-0.2.0a0/src/zcore/apps/shared/platformauth/templates/app_panel/
--rw-r--r--   0 harshshah   (501) staff       (20)     4939 2024-05-08 05:13:42.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      664 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1115 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/shared/platformauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.200394 zango-0.2.0a0/src/zcore/apps/shared/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.201168 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.204767 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/sync_static.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.210484 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5728 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/tasks.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.211991 zango-0.2.0a0/src/zcore/apps/shared/tenancy/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      676 2024-05-08 05:13:42.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/templates/app_panel.html
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.213629 zango-0.2.0a0/src/zcore/apps/shared/tenancy/templatetags/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/templatetags/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/templatetags/zstatic.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      147 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1546 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      383 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.215193 zango-0.2.0a0/src/zcore/apps/shared/tenancy/workspace_folder_template/
--rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.220137 zango-0.2.0a0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
--rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
--rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.225811 zango-0.2.0a0/src/zcore/apps/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/tasks/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/tasks/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.229965 zango-0.2.0a0/src/zcore/apps/tasks/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/tasks/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/tasks/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2647 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/apps/tasks/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/apps/tasks/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.117488 zango-0.2.0a0/src/zcore/assets/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.116509 zango-0.2.0a0/src/zcore/assets/app_landing/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.231169 zango-0.2.0a0/src/zcore/assets/app_landing/css/
--rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_landing/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.117264 zango-0.2.0a0/src/zcore/assets/app_panel/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.232312 zango-0.2.0a0/src/zcore/assets/app_panel/css/
--rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.235703 zango-0.2.0a0/src/zcore/assets/app_panel/images/
--rw-r--r--   0 harshshah   (501) staff       (20)     3499 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogo.svg
--rw-r--r--   0 harshshah   (501) staff       (20)     3906 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg
--rw-r--r--   0 harshshah   (501) staff       (20)     3913 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.276280 zango-0.2.0a0/src/zcore/assets/app_panel/js/
--rw-r--r--   0 harshshah   (501) staff       (20)  6158509 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.42.min.js
--rw-r--r--   0 harshshah   (501) staff       (20)  6158490 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.43.min.js
--rw-r--r--   0 harshshah   (501) staff       (20)  6158320 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.44.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.117605 zango-0.2.0a0/src/zcore/assets/js/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.117717 zango-0.2.0a0/src/zcore/assets/js/jquery/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.306974 zango-0.2.0a0/src/zcore/assets/js/jquery/3.7.1/
--rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/assets/js/jquery/3.7.1/jquery.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.320541 zango-0.2.0a0/src/zcore/cli/
--rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/install_package.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/package_info.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.346190 zango-0.2.0a0/src/zcore/cli/project_template/
--rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/manage.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.351598 zango-0.2.0a0/src/zcore/cli/project_template/project_name/
--rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/asgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3713 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/settings.py
--rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/urls_tenants.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/project_template/project_name/wsgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7084 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/start_project.py
--rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/cli/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.358379 zango-0.2.0a0/src/zcore/config/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/config/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-08 05:13:42.000000 zango-0.2.0a0/src/zcore/config/celery.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.363138 zango-0.2.0a0/src/zcore/config/settings/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/config/settings/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4940 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/config/settings/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      856 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/config/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/config/urls_tenants.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.382037 zango-0.2.0a0/src/zcore/core/
--rw-r--r--   0 harshshah   (501) staff       (20)       39 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.387566 zango-0.2.0a0/src/zcore/core/api/
--rw-r--r--   0 harshshah   (501) staff       (20)      200 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/api/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2104 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/api/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      846 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/api/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/common_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/custom_pluginbase.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.390071 zango-0.2.0a0/src/zcore/core/generic_views/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/generic_views/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1538 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/generic_views/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/internal_requests.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/model_mixins.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6624 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/package_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/storage_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1237 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/core/tasks.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/template_loader.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/core/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-14 06:15:58.393775 zango-0.2.0a0/src/zcore/middleware/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/middleware/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-06 09:37:40.000000 zango-0.2.0a0/src/zcore/middleware/request.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5455 2024-05-08 12:42:23.000000 zango-0.2.0a0/src/zcore/middleware/tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.578914 zango-0.2.0rc0/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10878 2024-03-05 18:32:15.000000 zango-0.2.0rc0/LICENSE
+-rw-r--r--   0 harshshah   (501) staff       (20)     5952 2024-05-15 11:29:27.577121 zango-0.2.0rc0/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     4346 2024-05-15 11:27:55.000000 zango-0.2.0rc0/README.md
+-rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-15 11:29:27.579453 zango-0.2.0rc0/setup.cfg
+-rw-r--r--   0 harshshah   (501) staff       (20)     1443 2024-05-15 11:28:20.000000 zango-0.2.0rc0/setup.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.060138 zango-0.2.0rc0/src/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.189432 zango-0.2.0rc0/src/zango/
+-rw-r--r--   0 harshshah   (501) staff       (20)       41 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.207608 zango-0.2.0rc0/src/zango/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.209414 zango-0.2.0rc0/src/zango/api/app_auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.210192 zango-0.2.0rc0/src/zango/api/app_auth/profile/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.217864 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2753 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/app_auth/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.220686 zango-0.2.0rc0/src/zango/api/platform/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.221680 zango-0.2.0rc0/src/zango/api/platform/auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.227607 zango-0.2.0rc0/src/zango/api/platform/auth/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/auth/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/auth/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/auth/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6079 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/auth/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.229094 zango-0.2.0rc0/src/zango/api/platform/codeassist/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/codeassist/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.239971 zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    11926 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.242280 zango-0.2.0rc0/src/zango/api/platform/packages/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/packages/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.245335 zango-0.2.0rc0/src/zango/api/platform/packages/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/packages/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/packages/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2601 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/packages/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.246986 zango-0.2.0rc0/src/zango/api/platform/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/permissions/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.251657 zango-0.2.0rc0/src/zango/api/platform/permissions/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/permissions/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/permissions/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/permissions/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6507 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/permissions/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.252743 zango-0.2.0rc0/src/zango/api/platform/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tasks/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.256077 zango-0.2.0rc0/src/zango/api/platform/tasks/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tasks/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tasks/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tasks/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4914 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tasks/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.257325 zango-0.2.0rc0/src/zango/api/platform/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tenancy/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.261083 zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1926 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    21220 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      291 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/api/platform/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.263019 zango-0.2.0rc0/src/zango/apps/
+-rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.277445 zango-0.2.0rc0/src/zango/apps/appauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.285092 zango-0.2.0rc0/src/zango/apps/appauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0002_default_user_roles.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0004_oldpasswords.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0005_remove_appusermodel_user.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/0006_appusermodel_app_objects.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     9188 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.286308 zango-0.2.0rc0/src/zango/apps/appauth/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/templates/app.html
+-rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/templates/app_login_signup.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/appauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.296560 zango-0.2.0rc0/src/zango/apps/dynamic_models/
+-rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      950 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.297896 zango-0.2.0rc0/src/zango/apps/dynamic_models/fields/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/fields/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.302273 zango-0.2.0rc0/src/zango/apps/dynamic_models/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.304543 zango-0.2.0rc0/src/zango/apps/dynamic_models/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/management/commands/reload_tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.305456 zango-0.2.0rc0/src/zango/apps/dynamic_models/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    15486 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      567 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/registry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      385 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.306403 zango-0.2.0rc0/src/zango/apps/dynamic_models/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)    29339 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/templates/default_landing.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.310997 zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    17473 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/lifecycle.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/wtree.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.320914 zango-0.2.0rc0/src/zango/apps/object_store/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.323583 zango-0.2.0rc0/src/zango/apps/object_store/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/object_store/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.334932 zango-0.2.0rc0/src/zango/apps/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.343251 zango-0.2.0rc0/src/zango/apps/permissions/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/migrations/0003_default_policy.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5050 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/mixin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3748 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/permissions/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.344324 zango-0.2.0rc0/src/zango/apps/shared/
+-rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.359223 zango-0.2.0rc0/src/zango/apps/shared/platformauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2578 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/abstract_model.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.364801 zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7168 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/models.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.104341 zango-0.2.0rc0/src/zango/apps/shared/platformauth/templates/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.366586 zango-0.2.0rc0/src/zango/apps/shared/platformauth/templates/app_panel/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4939 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      664 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1115 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/platformauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.381998 zango-0.2.0rc0/src/zango/apps/shared/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.383945 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.390326 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/sync_static.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.401176 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5728 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/tasks.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.403276 zango-0.2.0rc0/src/zango/apps/shared/tenancy/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      676 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/templates/app_panel.html
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.406201 zango-0.2.0rc0/src/zango/apps/shared/tenancy/templatetags/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/templatetags/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/templatetags/zstatic.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      147 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1546 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      383 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.407677 zango-0.2.0rc0/src/zango/apps/shared/tenancy/workspace_folder_template/
+-rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.410772 zango-0.2.0rc0/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
+-rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
+-rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.417342 zango-0.2.0rc0/src/zango/apps/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.420910 zango-0.2.0rc0/src/zango/apps/tasks/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2647 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/apps/tasks/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.131786 zango-0.2.0rc0/src/zango/assets/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.127643 zango-0.2.0rc0/src/zango/assets/app_landing/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.422280 zango-0.2.0rc0/src/zango/assets/app_landing/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_landing/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.130783 zango-0.2.0rc0/src/zango/assets/app_panel/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.423927 zango-0.2.0rc0/src/zango/assets/app_panel/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.427961 zango-0.2.0rc0/src/zango/assets/app_panel/images/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3499 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogo.svg
+-rw-r--r--   0 harshshah   (501) staff       (20)     3906 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogoIpad.svg
+-rw-r--r--   0 harshshah   (501) staff       (20)     3913 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogoIphone.svg
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.485592 zango-0.2.0rc0/src/zango/assets/app_panel/js/
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158509 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.42.min.js
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158490 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.43.min.js
+-rw-r--r--   0 harshshah   (501) staff       (20)  6158320 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.44.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.134986 zango-0.2.0rc0/src/zango/assets/js/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.145072 zango-0.2.0rc0/src/zango/assets/js/jquery/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.503910 zango-0.2.0rc0/src/zango/assets/js/jquery/3.7.1/
+-rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/assets/js/jquery/3.7.1/jquery.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.513110 zango-0.2.0rc0/src/zango/cli/
+-rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/install_package.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/package_info.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.515602 zango-0.2.0rc0/src/zango/cli/project_template/
+-rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/manage.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.527720 zango-0.2.0rc0/src/zango/cli/project_template/project_name/
+-rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/asgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3713 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/settings.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/urls_tenants.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/project_template/project_name/wsgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7084 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/start_project.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/cli/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.536652 zango-0.2.0rc0/src/zango/config/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/celery.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.540789 zango-0.2.0rc0/src/zango/config/settings/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/settings/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4940 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/settings/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      856 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/config/urls_tenants.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.559746 zango-0.2.0rc0/src/zango/core/
+-rw-r--r--   0 harshshah   (501) staff       (20)       39 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.563791 zango-0.2.0rc0/src/zango/core/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)      211 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/api/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2104 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/api/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      846 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/api/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/common_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/custom_pluginbase.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.567457 zango-0.2.0rc0/src/zango/core/generic_views/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/generic_views/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1539 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/generic_views/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/internal_requests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/model_mixins.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6624 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/package_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/storage_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1237 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/tasks.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/template_loader.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/core/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.572330 zango-0.2.0rc0/src/zango/middleware/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/middleware/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/middleware/request.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5455 2024-05-15 11:27:55.000000 zango-0.2.0rc0/src/zango/middleware/tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-15 11:29:27.574455 zango-0.2.0rc0/src/zango.egg-info/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5952 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     9014 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/SOURCES.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/dependency_links.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/entry_points.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)      677 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/requires.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-15 11:29:24.000000 zango-0.2.0rc0/src/zango.egg-info/top_level.txt
```

### Comparing `zango-0.2.0a0/LICENSE` & `zango-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/setup.py` & `zango-0.2.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PROJECT_DIR = os.path.dirname(__file__)
 REQUIREMENTS_DIR = os.path.join(PROJECT_DIR, "requirements")
 
 README = os.path.join(PROJECT_DIR, "README.md")
 
-PLATFORM_VERSION = "0.2.0-alpha"
+PLATFORM_VERSION = "0.2.0-rc"
 
 
 def get_requirements(env):
     with open(os.path.join(REQUIREMENTS_DIR, f"{env}.txt")) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
@@ -28,26 +28,26 @@
     long_description_content_type="text/markdown",
     author='Zelthy ("Healthlane Technologies")',
     author_email="maintainers@zelthy.com",
     url="https://github.com/Healthlane-Technologies/zelthy3",
     package_dir={"": "src"},
     packages=find_packages("src"),
     package_data={
-        "zcore": [
+        "zango": [
             "cli/project_template/**/*",
             "assets/**",
             "**/templates/**",
             "**/workspace_folder_template/**",
         ],
     },
     install_requires=install_requires,
     classifiers=[
         "Framework :: Django",
         "Programming Language :: Python",
     ],
     entry_points={
         "console_scripts": [
-            "zcore=zcore.cli:cli",
+            "zango=zango.cli:cli",
         ],
     },
     license_files=["LICENSE"],
 )
```

### Comparing `zango-0.2.0a0/src/zango.egg-info/SOURCES.txt` & `zango-0.2.0rc0/src/zango.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,202 +1,202 @@
 LICENSE
 README.md
 setup.py
+src/zango/__init__.py
 src/zango.egg-info/PKG-INFO
 src/zango.egg-info/SOURCES.txt
 src/zango.egg-info/dependency_links.txt
 src/zango.egg-info/entry_points.txt
 src/zango.egg-info/requires.txt
 src/zango.egg-info/top_level.txt
-src/zcore/__init__.py
-src/zcore/api/__init__.py
-src/zcore/api/app_auth/__init__.py
-src/zcore/api/app_auth/urls.py
-src/zcore/api/app_auth/profile/__init__.py
-src/zcore/api/app_auth/profile/v1/__init__.py
-src/zcore/api/app_auth/profile/v1/serializers.py
-src/zcore/api/app_auth/profile/v1/urls.py
-src/zcore/api/app_auth/profile/v1/utils.py
-src/zcore/api/app_auth/profile/v1/views.py
-src/zcore/api/platform/__init__.py
-src/zcore/api/platform/urls.py
-src/zcore/api/platform/auth/__init__.py
-src/zcore/api/platform/auth/v1/__init__.py
-src/zcore/api/platform/auth/v1/serializers.py
-src/zcore/api/platform/auth/v1/urls.py
-src/zcore/api/platform/auth/v1/views.py
-src/zcore/api/platform/codeassist/__init__.py
-src/zcore/api/platform/codeassist/v1/__init__.py
-src/zcore/api/platform/codeassist/v1/urls.py
-src/zcore/api/platform/codeassist/v1/utils.py
-src/zcore/api/platform/codeassist/v1/views.py
-src/zcore/api/platform/packages/__init__.py
-src/zcore/api/platform/packages/v1/__init__.py
-src/zcore/api/platform/packages/v1/urls.py
-src/zcore/api/platform/packages/v1/views.py
-src/zcore/api/platform/permissions/__init__.py
-src/zcore/api/platform/permissions/v1/__init__.py
-src/zcore/api/platform/permissions/v1/serializers.py
-src/zcore/api/platform/permissions/v1/urls.py
-src/zcore/api/platform/permissions/v1/views.py
-src/zcore/api/platform/tasks/__init__.py
-src/zcore/api/platform/tasks/v1/__init__.py
-src/zcore/api/platform/tasks/v1/serializers.py
-src/zcore/api/platform/tasks/v1/urls.py
-src/zcore/api/platform/tasks/v1/views.py
-src/zcore/api/platform/tenancy/__init__.py
-src/zcore/api/platform/tenancy/v1/__init__.py
-src/zcore/api/platform/tenancy/v1/serializers.py
-src/zcore/api/platform/tenancy/v1/urls.py
-src/zcore/api/platform/tenancy/v1/views.py
-src/zcore/apps/__init__.py
-src/zcore/apps/appauth/__init__.py
-src/zcore/apps/appauth/admin.py
-src/zcore/apps/appauth/apps.py
-src/zcore/apps/appauth/auth_backend.py
-src/zcore/apps/appauth/models.py
-src/zcore/apps/appauth/serializers.py
-src/zcore/apps/appauth/signals.py
-src/zcore/apps/appauth/tests.py
-src/zcore/apps/appauth/urls.py
-src/zcore/apps/appauth/views.py
-src/zcore/apps/appauth/migrations/0001_initial.py
-src/zcore/apps/appauth/migrations/0002_default_user_roles.py
-src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
-src/zcore/apps/appauth/migrations/0004_oldpasswords.py
-src/zcore/apps/appauth/migrations/0005_remove_appusermodel_user.py
-src/zcore/apps/appauth/migrations/0006_appusermodel_app_objects.py
-src/zcore/apps/appauth/migrations/__init__.py
-src/zcore/apps/appauth/templates/app.html
-src/zcore/apps/appauth/templates/app_login_signup.html
-src/zcore/apps/dynamic_models/__init__.py
-src/zcore/apps/dynamic_models/admin.py
-src/zcore/apps/dynamic_models/apps.py
-src/zcore/apps/dynamic_models/models.py
-src/zcore/apps/dynamic_models/permissions.py
-src/zcore/apps/dynamic_models/registry.py
-src/zcore/apps/dynamic_models/signals.py
-src/zcore/apps/dynamic_models/tests.py
-src/zcore/apps/dynamic_models/urls.py
-src/zcore/apps/dynamic_models/views.py
-src/zcore/apps/dynamic_models/fields/__init__.py
-src/zcore/apps/dynamic_models/management/__init__.py
-src/zcore/apps/dynamic_models/management/commands/__init__.py
-src/zcore/apps/dynamic_models/management/commands/reload_tenant.py
-src/zcore/apps/dynamic_models/migrations/__init__.py
-src/zcore/apps/dynamic_models/templates/default_landing.html
-src/zcore/apps/dynamic_models/workspace/__init__.py
-src/zcore/apps/dynamic_models/workspace/base.py
-src/zcore/apps/dynamic_models/workspace/lifecycle.py
-src/zcore/apps/dynamic_models/workspace/wtree.py
-src/zcore/apps/object_store/__init__.py
-src/zcore/apps/object_store/admin.py
-src/zcore/apps/object_store/apps.py
-src/zcore/apps/object_store/models.py
-src/zcore/apps/object_store/tests.py
-src/zcore/apps/object_store/views.py
-src/zcore/apps/object_store/migrations/0001_initial.py
-src/zcore/apps/object_store/migrations/__init__.py
-src/zcore/apps/permissions/__init__.py
-src/zcore/apps/permissions/admin.py
-src/zcore/apps/permissions/apps.py
-src/zcore/apps/permissions/mixin.py
-src/zcore/apps/permissions/models.py
-src/zcore/apps/permissions/tests.py
-src/zcore/apps/permissions/views.py
-src/zcore/apps/permissions/migrations/0001_initial.py
-src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
-src/zcore/apps/permissions/migrations/0003_default_policy.py
-src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
-src/zcore/apps/permissions/migrations/__init__.py
-src/zcore/apps/shared/__init__.py
-src/zcore/apps/shared/platformauth/__init__.py
-src/zcore/apps/shared/platformauth/abstract_model.py
-src/zcore/apps/shared/platformauth/admin.py
-src/zcore/apps/shared/platformauth/apps.py
-src/zcore/apps/shared/platformauth/auth_backend.py
-src/zcore/apps/shared/platformauth/models.py
-src/zcore/apps/shared/platformauth/tests.py
-src/zcore/apps/shared/platformauth/urls.py
-src/zcore/apps/shared/platformauth/views.py
-src/zcore/apps/shared/platformauth/migrations/0001_initial.py
-src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
-src/zcore/apps/shared/platformauth/migrations/__init__.py
-src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html
-src/zcore/apps/shared/tenancy/__init__.py
-src/zcore/apps/shared/tenancy/admin.py
-src/zcore/apps/shared/tenancy/apps.py
-src/zcore/apps/shared/tenancy/models.py
-src/zcore/apps/shared/tenancy/tasks.py
-src/zcore/apps/shared/tenancy/tests.py
-src/zcore/apps/shared/tenancy/urls.py
-src/zcore/apps/shared/tenancy/utils.py
-src/zcore/apps/shared/tenancy/views.py
-src/zcore/apps/shared/tenancy/management/__init__.py
-src/zcore/apps/shared/tenancy/management/commands/__init__.py
-src/zcore/apps/shared/tenancy/management/commands/sync_static.py
-src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py
-src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py
-src/zcore/apps/shared/tenancy/migrations/0001_initial.py
-src/zcore/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
-src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
-src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
-src/zcore/apps/shared/tenancy/migrations/__init__.py
-src/zcore/apps/shared/tenancy/templates/app_panel.html
-src/zcore/apps/shared/tenancy/templatetags/__init__.py
-src/zcore/apps/shared/tenancy/templatetags/zstatic.py
-src/zcore/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
-src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
-src/zcore/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
-src/zcore/apps/tasks/__init__.py
-src/zcore/apps/tasks/apps.py
-src/zcore/apps/tasks/models.py
-src/zcore/apps/tasks/utils.py
-src/zcore/apps/tasks/migrations/0001_initial.py
-src/zcore/apps/tasks/migrations/__init__.py
-src/zcore/assets/app_landing/css/styles.css
-src/zcore/assets/app_panel/css/styles.css
-src/zcore/assets/app_panel/images/zelthyLogo.svg
-src/zcore/assets/app_panel/images/zelthyLogoIpad.svg
-src/zcore/assets/app_panel/images/zelthyLogoIphone.svg
-src/zcore/assets/app_panel/js/build.v1.0.42.min.js
-src/zcore/assets/app_panel/js/build.v1.0.43.min.js
-src/zcore/assets/app_panel/js/build.v1.0.44.min.js
-src/zcore/assets/js/jquery/3.7.1/jquery.min.js
-src/zcore/cli/__init__.py
-src/zcore/cli/install_package.py
-src/zcore/cli/package_info.py
-src/zcore/cli/start_project.py
-src/zcore/cli/utils.py
-src/zcore/cli/project_template/manage.py
-src/zcore/cli/project_template/project_name/__init__.py
-src/zcore/cli/project_template/project_name/asgi.py
-src/zcore/cli/project_template/project_name/settings.py
-src/zcore/cli/project_template/project_name/urls.py
-src/zcore/cli/project_template/project_name/urls_public.py
-src/zcore/cli/project_template/project_name/urls_tenants.py
-src/zcore/cli/project_template/project_name/wsgi.py
-src/zcore/config/__init__.py
-src/zcore/config/celery.py
-src/zcore/config/urls_public.py
-src/zcore/config/urls_tenants.py
-src/zcore/config/settings/__init__.py
-src/zcore/config/settings/base.py
-src/zcore/core/__init__.py
-src/zcore/core/common_utils.py
-src/zcore/core/custom_pluginbase.py
-src/zcore/core/internal_requests.py
-src/zcore/core/model_mixins.py
-src/zcore/core/package_utils.py
-src/zcore/core/permissions.py
-src/zcore/core/storage_utils.py
-src/zcore/core/tasks.py
-src/zcore/core/template_loader.py
-src/zcore/core/utils.py
-src/zcore/core/api/__init__.py
-src/zcore/core/api/base.py
-src/zcore/core/api/utils.py
-src/zcore/core/generic_views/__init__.py
-src/zcore/core/generic_views/base.py
-src/zcore/middleware/__init__.py
-src/zcore/middleware/request.py
-src/zcore/middleware/tenant.py
+src/zango/api/__init__.py
+src/zango/api/app_auth/__init__.py
+src/zango/api/app_auth/urls.py
+src/zango/api/app_auth/profile/__init__.py
+src/zango/api/app_auth/profile/v1/__init__.py
+src/zango/api/app_auth/profile/v1/serializers.py
+src/zango/api/app_auth/profile/v1/urls.py
+src/zango/api/app_auth/profile/v1/utils.py
+src/zango/api/app_auth/profile/v1/views.py
+src/zango/api/platform/__init__.py
+src/zango/api/platform/urls.py
+src/zango/api/platform/auth/__init__.py
+src/zango/api/platform/auth/v1/__init__.py
+src/zango/api/platform/auth/v1/serializers.py
+src/zango/api/platform/auth/v1/urls.py
+src/zango/api/platform/auth/v1/views.py
+src/zango/api/platform/codeassist/__init__.py
+src/zango/api/platform/codeassist/v1/__init__.py
+src/zango/api/platform/codeassist/v1/urls.py
+src/zango/api/platform/codeassist/v1/utils.py
+src/zango/api/platform/codeassist/v1/views.py
+src/zango/api/platform/packages/__init__.py
+src/zango/api/platform/packages/v1/__init__.py
+src/zango/api/platform/packages/v1/urls.py
+src/zango/api/platform/packages/v1/views.py
+src/zango/api/platform/permissions/__init__.py
+src/zango/api/platform/permissions/v1/__init__.py
+src/zango/api/platform/permissions/v1/serializers.py
+src/zango/api/platform/permissions/v1/urls.py
+src/zango/api/platform/permissions/v1/views.py
+src/zango/api/platform/tasks/__init__.py
+src/zango/api/platform/tasks/v1/__init__.py
+src/zango/api/platform/tasks/v1/serializers.py
+src/zango/api/platform/tasks/v1/urls.py
+src/zango/api/platform/tasks/v1/views.py
+src/zango/api/platform/tenancy/__init__.py
+src/zango/api/platform/tenancy/v1/__init__.py
+src/zango/api/platform/tenancy/v1/serializers.py
+src/zango/api/platform/tenancy/v1/urls.py
+src/zango/api/platform/tenancy/v1/views.py
+src/zango/apps/__init__.py
+src/zango/apps/appauth/__init__.py
+src/zango/apps/appauth/admin.py
+src/zango/apps/appauth/apps.py
+src/zango/apps/appauth/auth_backend.py
+src/zango/apps/appauth/models.py
+src/zango/apps/appauth/serializers.py
+src/zango/apps/appauth/signals.py
+src/zango/apps/appauth/tests.py
+src/zango/apps/appauth/urls.py
+src/zango/apps/appauth/views.py
+src/zango/apps/appauth/migrations/0001_initial.py
+src/zango/apps/appauth/migrations/0002_default_user_roles.py
+src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
+src/zango/apps/appauth/migrations/0004_oldpasswords.py
+src/zango/apps/appauth/migrations/0005_remove_appusermodel_user.py
+src/zango/apps/appauth/migrations/0006_appusermodel_app_objects.py
+src/zango/apps/appauth/migrations/__init__.py
+src/zango/apps/appauth/templates/app.html
+src/zango/apps/appauth/templates/app_login_signup.html
+src/zango/apps/dynamic_models/__init__.py
+src/zango/apps/dynamic_models/admin.py
+src/zango/apps/dynamic_models/apps.py
+src/zango/apps/dynamic_models/models.py
+src/zango/apps/dynamic_models/permissions.py
+src/zango/apps/dynamic_models/registry.py
+src/zango/apps/dynamic_models/signals.py
+src/zango/apps/dynamic_models/tests.py
+src/zango/apps/dynamic_models/urls.py
+src/zango/apps/dynamic_models/views.py
+src/zango/apps/dynamic_models/fields/__init__.py
+src/zango/apps/dynamic_models/management/__init__.py
+src/zango/apps/dynamic_models/management/commands/__init__.py
+src/zango/apps/dynamic_models/management/commands/reload_tenant.py
+src/zango/apps/dynamic_models/migrations/__init__.py
+src/zango/apps/dynamic_models/templates/default_landing.html
+src/zango/apps/dynamic_models/workspace/__init__.py
+src/zango/apps/dynamic_models/workspace/base.py
+src/zango/apps/dynamic_models/workspace/lifecycle.py
+src/zango/apps/dynamic_models/workspace/wtree.py
+src/zango/apps/object_store/__init__.py
+src/zango/apps/object_store/admin.py
+src/zango/apps/object_store/apps.py
+src/zango/apps/object_store/models.py
+src/zango/apps/object_store/tests.py
+src/zango/apps/object_store/views.py
+src/zango/apps/object_store/migrations/0001_initial.py
+src/zango/apps/object_store/migrations/__init__.py
+src/zango/apps/permissions/__init__.py
+src/zango/apps/permissions/admin.py
+src/zango/apps/permissions/apps.py
+src/zango/apps/permissions/mixin.py
+src/zango/apps/permissions/models.py
+src/zango/apps/permissions/tests.py
+src/zango/apps/permissions/views.py
+src/zango/apps/permissions/migrations/0001_initial.py
+src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
+src/zango/apps/permissions/migrations/0003_default_policy.py
+src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
+src/zango/apps/permissions/migrations/__init__.py
+src/zango/apps/shared/__init__.py
+src/zango/apps/shared/platformauth/__init__.py
+src/zango/apps/shared/platformauth/abstract_model.py
+src/zango/apps/shared/platformauth/admin.py
+src/zango/apps/shared/platformauth/apps.py
+src/zango/apps/shared/platformauth/auth_backend.py
+src/zango/apps/shared/platformauth/models.py
+src/zango/apps/shared/platformauth/tests.py
+src/zango/apps/shared/platformauth/urls.py
+src/zango/apps/shared/platformauth/views.py
+src/zango/apps/shared/platformauth/migrations/0001_initial.py
+src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
+src/zango/apps/shared/platformauth/migrations/__init__.py
+src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html
+src/zango/apps/shared/tenancy/__init__.py
+src/zango/apps/shared/tenancy/admin.py
+src/zango/apps/shared/tenancy/apps.py
+src/zango/apps/shared/tenancy/models.py
+src/zango/apps/shared/tenancy/tasks.py
+src/zango/apps/shared/tenancy/tests.py
+src/zango/apps/shared/tenancy/urls.py
+src/zango/apps/shared/tenancy/utils.py
+src/zango/apps/shared/tenancy/views.py
+src/zango/apps/shared/tenancy/management/__init__.py
+src/zango/apps/shared/tenancy/management/commands/__init__.py
+src/zango/apps/shared/tenancy/management/commands/sync_static.py
+src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py
+src/zango/apps/shared/tenancy/management/commands/ws_migrate.py
+src/zango/apps/shared/tenancy/migrations/0001_initial.py
+src/zango/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
+src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
+src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
+src/zango/apps/shared/tenancy/migrations/__init__.py
+src/zango/apps/shared/tenancy/templates/app_panel.html
+src/zango/apps/shared/tenancy/templatetags/__init__.py
+src/zango/apps/shared/tenancy/templatetags/zstatic.py
+src/zango/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
+src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
+src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
+src/zango/apps/tasks/__init__.py
+src/zango/apps/tasks/apps.py
+src/zango/apps/tasks/models.py
+src/zango/apps/tasks/utils.py
+src/zango/apps/tasks/migrations/0001_initial.py
+src/zango/apps/tasks/migrations/__init__.py
+src/zango/assets/app_landing/css/styles.css
+src/zango/assets/app_panel/css/styles.css
+src/zango/assets/app_panel/images/zelthyLogo.svg
+src/zango/assets/app_panel/images/zelthyLogoIpad.svg
+src/zango/assets/app_panel/images/zelthyLogoIphone.svg
+src/zango/assets/app_panel/js/build.v1.0.42.min.js
+src/zango/assets/app_panel/js/build.v1.0.43.min.js
+src/zango/assets/app_panel/js/build.v1.0.44.min.js
+src/zango/assets/js/jquery/3.7.1/jquery.min.js
+src/zango/cli/__init__.py
+src/zango/cli/install_package.py
+src/zango/cli/package_info.py
+src/zango/cli/start_project.py
+src/zango/cli/utils.py
+src/zango/cli/project_template/manage.py
+src/zango/cli/project_template/project_name/__init__.py
+src/zango/cli/project_template/project_name/asgi.py
+src/zango/cli/project_template/project_name/settings.py
+src/zango/cli/project_template/project_name/urls.py
+src/zango/cli/project_template/project_name/urls_public.py
+src/zango/cli/project_template/project_name/urls_tenants.py
+src/zango/cli/project_template/project_name/wsgi.py
+src/zango/config/__init__.py
+src/zango/config/celery.py
+src/zango/config/urls_public.py
+src/zango/config/urls_tenants.py
+src/zango/config/settings/__init__.py
+src/zango/config/settings/base.py
+src/zango/core/__init__.py
+src/zango/core/common_utils.py
+src/zango/core/custom_pluginbase.py
+src/zango/core/internal_requests.py
+src/zango/core/model_mixins.py
+src/zango/core/package_utils.py
+src/zango/core/permissions.py
+src/zango/core/storage_utils.py
+src/zango/core/tasks.py
+src/zango/core/template_loader.py
+src/zango/core/utils.py
+src/zango/core/api/__init__.py
+src/zango/core/api/base.py
+src/zango/core/api/utils.py
+src/zango/core/generic_views/__init__.py
+src/zango/core/generic_views/base.py
+src/zango/middleware/__init__.py
+src/zango/middleware/request.py
+src/zango/middleware/tenant.py
```

### Comparing `zango-0.2.0a0/src/zango.egg-info/requires.txt` & `zango-0.2.0rc0/src/zango.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/utils.py` & `zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/api/app_auth/profile/v1/views.py` & `zango-0.2.0rc0/src/zango/api/app_auth/profile/v1/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django.contrib.auth import authenticate
 from django.core.exceptions import ValidationError
 
-from zcore.core.api import (
+from zango.core.api import (
     get_api_response,
-    ZCoreGenericAppAPIView,
-    ZCoreSessionAppAPIView,
+    ZangoGenericAppAPIView,
+    ZangoSessionAppAPIView,
 )
-from zcore.api.app_auth.profile.v1.utils import PasswordValidationMixin
-from zcore.apps.appauth.models import OldPasswords
+from zango.api.app_auth.profile.v1.utils import PasswordValidationMixin
+from zango.apps.appauth.models import OldPasswords
 
 from .serializers import ProfileSerializer
 
 
-class ProfileViewAPIV1(ZCoreGenericAppAPIView):
+class ProfileViewAPIV1(ZangoGenericAppAPIView):
     def get(self, request, *args, **kwargs):
         serializer = ProfileSerializer(request.user)
         success = True
         response = {"message": "success", "profile_data": serializer.data}
         status = 200
         return get_api_response(success, response, status)
 
@@ -26,15 +26,15 @@
         if success:
             status = 200
         else:
             status = 400
         return get_api_response(success, response, status)
 
 
-class PasswordChangeViewAPIV1(ZCoreSessionAppAPIView, PasswordValidationMixin):
+class PasswordChangeViewAPIV1(ZangoSessionAppAPIView, PasswordValidationMixin):
     def clean_password(self, email, password):
         """
         Validates that the email is not already in use.
         """
         try:
             user = authenticate(username=email, password=password)
         except:
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/auth/v1/serializers.py` & `zango-0.2.0rc0/src/zango/api/platform/auth/v1/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rest_framework import serializers
-from zcore.apps.shared.platformauth.models import PlatformUserModel
-from zcore.api.platform.tenancy.v1.serializers import TenantSerializerModel
+from zango.apps.shared.platformauth.models import PlatformUserModel
+from zango.api.platform.tenancy.v1.serializers import TenantSerializerModel
 
 
 class PlatformUserSerializerModel(serializers.ModelSerializer):
     apps = TenantSerializerModel(many=True)
 
     class Meta:
         model = PlatformUserModel
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/auth/v1/urls.py` & `zango-0.2.0rc0/src/zango/api/platform/auth/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/api/platform/auth/v1/views.py` & `zango-0.2.0rc0/src/zango/api/platform/auth/v1/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.db.models import Q
 from django.conf import settings
 
-from zcore.core.api import (
+from zango.core.api import (
     get_api_response,
-    ZCoreGenericPlatformAPIView,
+    ZangoGenericPlatformAPIView,
 )
-from zcore.core.api.utils import ZCoreAPIPagination
-from zcore.apps.shared.platformauth.models import PlatformUserModel
-from zcore.apps.shared.tenancy.models import TenantModel
-from zcore.core.permissions import IsSuperAdminPlatformUser
-from zcore.core.utils import get_search_columns
+from zango.core.api.utils import ZangoAPIPagination
+from zango.apps.shared.platformauth.models import PlatformUserModel
+from zango.apps.shared.tenancy.models import TenantModel
+from zango.core.permissions import IsSuperAdminPlatformUser
+from zango.core.utils import get_search_columns
 
 from .serializers import PlatformUserSerializerModel
 
 
-class PlatformUserViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
+class PlatformUserViewAPIV1(ZangoGenericPlatformAPIView, ZangoAPIPagination):
     permission_classes = (IsSuperAdminPlatformUser,)
-    pagination_class = ZCoreAPIPagination
+    pagination_class = ZangoAPIPagination
 
     def get_dropdown_options(self):
         options = {}
         options["apps"] = [
             {"id": str(t.uuid), "label": t.name}
             for t in TenantModel.objects.all().exclude(schema_name="public")
         ]
@@ -100,15 +100,15 @@
         except Exception as e:
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
-class PlatformUserDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class PlatformUserDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsSuperAdminPlatformUser,)
 
     def get_obj(self, **kwargs):
         obj = PlatformUserModel.objects.get(id=kwargs.get("user_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -140,15 +140,15 @@
             success = False
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
-class AppPanelDetailsView(ZCoreGenericPlatformAPIView):
+class AppPanelDetailsView(ZangoGenericPlatformAPIView):
     def get_obj(self, request, **kwargs):
         obj = PlatformUserModel.objects.get(id=request.user.id)
         return obj
 
     def get(self, request, *args, **kwargs):
         try:
             obj = self.get_obj(request, **kwargs)
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/codeassist/v1/views.py` & `zango-0.2.0rc0/src/zango/api/platform/codeassist/v1/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import os
 import importlib
 
 from django.utils.decorators import method_decorator
 from django.conf import settings
 
-from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api import get_api_response, ZCoreGenericPlatformAPIView
+from zango.core.common_utils import set_app_schema_path
+from zango.core.api import get_api_response, ZangoGenericPlatformAPIView
 
-from zcore.apps.permissions.models import PolicyModel
-from zcore.apps.appauth.models import AppUserModel, UserRoleModel
-from zcore.apps.shared.tenancy.models import TenantModel
+from zango.apps.permissions.models import PolicyModel
+from zango.apps.appauth.models import AppUserModel, UserRoleModel
+from zango.apps.shared.tenancy.models import TenantModel
 
 from .utils import lambda_invocation
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class ConversationViewAPIV1(ZCoreGenericPlatformAPIView):
+class ConversationViewAPIV1(ZangoGenericPlatformAPIView):
     def get_app_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_settings_path(self, **kwargs):
         obj = self.get_app_obj(**kwargs)
         path = str(settings.BASE_DIR) + f"/workspaces/{obj.name}/settings.json"
@@ -53,15 +53,15 @@
 
         response_data = lambda_invocation(data)
         response = response_data["response"]
         return get_api_response(True, response, 200)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class ExecutionViewAPIV1(ZCoreGenericPlatformAPIView):
+class ExecutionViewAPIV1(ZangoGenericPlatformAPIView):
     def get_app_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_settings_path(self, **kwargs):
         obj = self.get_app_obj(**kwargs)
         path = str(settings.BASE_DIR) + f"/workspaces/{obj.name}/settings.json"
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/permissions/v1/serializers.py` & `zango-0.2.0rc0/src/zango/api/platform/permissions/v1/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 from rest_framework import serializers
-from zcore.apps.shared.tenancy.models import TenantModel, Domain
-from zcore.apps.permissions.models import PolicyModel
-from zcore.apps.appauth.models import UserRoleModel
+from zango.apps.shared.tenancy.models import TenantModel, Domain
+from zango.apps.permissions.models import PolicyModel
+from zango.apps.appauth.models import UserRoleModel
 
 
 class PolicySerializer(serializers.ModelSerializer):
     roles = serializers.SerializerMethodField()
 
     class Meta:
         model = PolicyModel
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/permissions/v1/urls.py` & `zango-0.2.0rc0/src/zango/api/platform/permissions/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/api/platform/permissions/v1/views.py` & `zango-0.2.0rc0/src/zango/api/platform/permissions/v1/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import traceback
 
 from django.utils.decorators import method_decorator
 from django.db.models import Q
 from django.db import connection
 
-from zcore.core.api import (
+from zango.core.api import (
     get_api_response,
-    ZCoreGenericPlatformAPIView,
+    ZangoGenericPlatformAPIView,
 )
-from zcore.core.utils import get_search_columns
-from zcore.apps.shared.tenancy.models import TenantModel
-from zcore.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT
-from zcore.apps.permissions.models import PolicyModel, PermissionsModel
-from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api.utils import ZCoreAPIPagination
-from zcore.core.permissions import IsPlatformUserAllowedApp
-from zcore.apps.appauth.models import UserRoleModel
-from zcore.apps.dynamic_models.workspace.base import Workspace
+from zango.core.utils import get_search_columns
+from zango.apps.shared.tenancy.models import TenantModel
+from zango.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT
+from zango.apps.permissions.models import PolicyModel, PermissionsModel
+from zango.core.common_utils import set_app_schema_path
+from zango.core.api.utils import ZangoAPIPagination
+from zango.core.permissions import IsPlatformUserAllowedApp
+from zango.apps.appauth.models import UserRoleModel
+from zango.apps.dynamic_models.workspace.base import Workspace
 
 
 from .serializers import PolicySerializer
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class PolicyViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
-    pagination_class = ZCoreAPIPagination
+class PolicyViewAPIV1(ZangoGenericPlatformAPIView, ZangoAPIPagination):
+    pagination_class = ZangoAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_queryset(self, search, columns={}):
         field_name_query_mapping = {
             "policy_name": "name__icontains",
             "description": "description__icontains",
             "policy_id": "id__icontains",
@@ -116,15 +116,15 @@
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class PolicyDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class PolicyDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = PolicyModel.objects.get(id=kwargs.get("policy_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/tasks/v1/serializers.py` & `zango-0.2.0rc0/src/zango/api/platform/tasks/v1/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from django_celery_beat.models import CrontabSchedule
 from rest_framework import serializers
 
-from zcore.apps.tasks.models import AppTask
-from zcore.api.platform.permissions.v1.serializers import PolicySerializer
-from zcore.apps.tasks.utils import get_crontab_obj
+from zango.apps.tasks.models import AppTask
+from zango.api.platform.permissions.v1.serializers import PolicySerializer
+from zango.apps.tasks.utils import get_crontab_obj
 
 
 class CronTabSerializer(serializers.ModelSerializer):
     class Meta:
         model = CrontabSchedule
         fields = [
             "minute",
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/tasks/v1/views.py` & `zango-0.2.0rc0/src/zango/api/platform/tasks/v1/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import traceback
 
 from django.utils.decorators import method_decorator
 from django.db import connection
 from django.db.models import Q
 
-from zcore.core.api import get_api_response, ZCoreGenericPlatformAPIView
-from zcore.apps.tasks.models import AppTask
-from zcore.core.api.utils import ZCoreAPIPagination
-from zcore.core.common_utils import set_app_schema_path
-from zcore.apps.dynamic_models.workspace.base import Workspace
-from zcore.apps.shared.tenancy.models import TenantModel
-from zcore.core.utils import get_search_columns
+from zango.core.api import get_api_response, ZangoGenericPlatformAPIView
+from zango.apps.tasks.models import AppTask
+from zango.core.api.utils import ZangoAPIPagination
+from zango.core.common_utils import set_app_schema_path
+from zango.apps.dynamic_models.workspace.base import Workspace
+from zango.apps.shared.tenancy.models import TenantModel
+from zango.core.utils import get_search_columns
 
 
 from .serializers import TaskSerializer
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class AppTaskView(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
-    pagination_class = ZCoreAPIPagination
+class AppTaskView(ZangoGenericPlatformAPIView, ZangoAPIPagination):
+    pagination_class = ZangoAPIPagination
 
     def get_queryset(self, search, columns={}):
         name_field_query_mappping = {
             "name": "name__icontains",
             "id": "id__icontains",
             "attached_policies": "attached_policies__name__icontains",
             "is_enabled": "is_enabled",
@@ -81,15 +81,15 @@
             response = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, response, status)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class AppTaskDetailView(ZCoreGenericPlatformAPIView):
+class AppTaskDetailView(ZangoGenericPlatformAPIView):
     def get(self, request, app_uuid, task_uuid, *args, **kwargs):
         try:
             app_task = AppTask.objects.get(id=task_uuid)
             serializer = TaskSerializer(instance=app_task)
             response = {"task": serializer.data}
             status = 200
             success = True
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/serializers.py` & `zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 from rest_framework import serializers
-from zcore.apps.shared.tenancy.models import TenantModel, Domain, ThemesModel
-from zcore.apps.appauth.models import UserRoleModel, AppUserModel
+from zango.apps.shared.tenancy.models import TenantModel, Domain, ThemesModel
+from zango.apps.appauth.models import UserRoleModel, AppUserModel
 
-from zcore.api.platform.permissions.v1.serializers import PolicySerializer
+from zango.api.platform.permissions.v1.serializers import PolicySerializer
 
 
 class DomainSerializerModel(serializers.ModelSerializer):
     class Meta:
         model = Domain
         fields = ["domain", "is_primary"]
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/urls.py` & `zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     UserRoleDetailViewAPIV1,
     UserViewAPIV1,
     UserDetailViewAPIV1,
     ThemeViewAPIV1,
     ThemeDetailViewAPIV1,
 )
 
-from zcore.api.platform.permissions.v1 import urls as permissions_v1_urls
-from zcore.api.platform.packages.v1 import urls as packages_v1_urls
-from zcore.api.platform.tasks.v1 import urls as tasks_v1_urls
-from zcore.api.platform.codeassist.v1 import urls as codeassist_v1_urls
+from zango.api.platform.permissions.v1 import urls as permissions_v1_urls
+from zango.api.platform.packages.v1 import urls as packages_v1_urls
+from zango.api.platform.tasks.v1 import urls as tasks_v1_urls
+from zango.api.platform.codeassist.v1 import urls as codeassist_v1_urls
 
 
 urlpatterns = [
     re_path(r"$", AppViewAPIV1.as_view(), name="apps-apiv1-appview"),
     re_path(
         r"^(?P<app_uuid>[\w-]+)/$",
         AppDetailViewAPIV1.as_view(),
```

### Comparing `zango-0.2.0a0/src/zcore/api/platform/tenancy/v1/views.py` & `zango-0.2.0rc0/src/zango/api/platform/tenancy/v1/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 from django_celery_results.models import TaskResult
 
 from django.conf import settings
 from django.utils.decorators import method_decorator
 from django.db.models import Q
 
-from zcore.core.api import (
+from zango.core.api import (
     get_api_response,
-    ZCoreGenericPlatformAPIView,
+    ZangoGenericPlatformAPIView,
 )
-from zcore.apps.shared.tenancy.models import TenantModel, ThemesModel
-from zcore.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT, DATEFORMAT
-from zcore.apps.appauth.models import UserRoleModel, AppUserModel
-from zcore.apps.permissions.models import PolicyModel
-from zcore.core.common_utils import set_app_schema_path
-from zcore.core.api.utils import ZCoreAPIPagination
-from zcore.core.permissions import IsPlatformUserAllowedApp
-from zcore.core.utils import get_search_columns
+from zango.apps.shared.tenancy.models import TenantModel, ThemesModel
+from zango.apps.shared.tenancy.utils import TIMEZONES, DATETIMEFORMAT, DATEFORMAT
+from zango.apps.appauth.models import UserRoleModel, AppUserModel
+from zango.apps.permissions.models import PolicyModel
+from zango.core.common_utils import set_app_schema_path
+from zango.core.api.utils import ZangoAPIPagination
+from zango.core.permissions import IsPlatformUserAllowedApp
+from zango.core.utils import get_search_columns
 
 from .serializers import (
     TenantSerializerModel,
     UserRoleSerializerModel,
     AppUserModelSerializerModel,
     ThemeModelSerializer,
 )
 
 
-class AppViewAPIV1(ZCoreGenericPlatformAPIView):
+class AppViewAPIV1(ZangoGenericPlatformAPIView):
     def get(self, request, *args, **kwargs):
         try:
             action = request.GET.get("action")
             if action == "get_app_creation_status":
                 task_id = request.GET.get("task_id")
                 try:
                     task = TaskResult.objects.get(task_id=task_id)
@@ -112,15 +112,15 @@
             # logger.error(traceback.format_exc())
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
-class AppDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class AppDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = TenantModel.objects.get(uuid=kwargs.get("app_uuid"))
         return obj
 
     def get_dropdown_options(self):
@@ -185,16 +185,16 @@
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserRoleViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
-    pagination_class = ZCoreAPIPagination
+class UserRoleViewAPIV1(ZangoGenericPlatformAPIView, ZangoAPIPagination):
+    pagination_class = ZangoAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_dropdown_options(self):
         options = {}
         options["policies"] = [
             {"id": t.id, "label": t.name}
             for t in PolicyModel.objects.all().order_by("-modified_at")
@@ -274,15 +274,15 @@
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserRoleDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class UserRoleDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = UserRoleModel.objects.get(id=kwargs.get("role_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -333,16 +333,16 @@
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserViewAPIV1(ZCoreGenericPlatformAPIView, ZCoreAPIPagination):
-    pagination_class = ZCoreAPIPagination
+class UserViewAPIV1(ZangoGenericPlatformAPIView, ZangoAPIPagination):
+    pagination_class = ZangoAPIPagination
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_dropdown_options(self):
         options = {}
         options["roles"] = [
             {"id": t.id, "label": t.name}
             for t in UserRoleModel.objects.all().exclude(
@@ -422,15 +422,15 @@
             result = {"message": str(e)}
             status = 500
             success = False
         return get_api_response(success, result, status)
 
 
 @method_decorator(set_app_schema_path, name="dispatch")
-class UserDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class UserDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = AppUserModel.objects.get(id=kwargs.get("user_id"))
         return obj
 
     def get(self, request, *args, **kwargs):
@@ -462,15 +462,15 @@
             success = False
             result = {"message": str(e)}
             status_code = 500
 
         return get_api_response(success, result, status_code)
 
 
-class ThemeViewAPIV1(ZCoreGenericPlatformAPIView):
+class ThemeViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_app_tenant(self):
         tenant_obj = TenantModel.objects.get(uuid=self.kwargs["app_uuid"])
         return tenant_obj
 
     def get(self, request, *args, **kwargs):
@@ -522,15 +522,15 @@
                 error_message = "Invalid data"
 
             result = {"message": error_message}
 
         return get_api_response(success, result, status_code)
 
 
-class ThemeDetailViewAPIV1(ZCoreGenericPlatformAPIView):
+class ThemeDetailViewAPIV1(ZangoGenericPlatformAPIView):
     permission_classes = (IsPlatformUserAllowedApp,)
 
     def get_obj(self, **kwargs):
         obj = ThemesModel.objects.get(
             tenant__uuid=kwargs.get("app_uuid"), id=kwargs.get("theme_id")
         )
         return obj
```

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/auth_backend.py` & `zango-0.2.0rc0/src/zango/apps/appauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/appauth/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by Django 4.2.2 on 2023-08-13 04:09
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
-import zcore.apps.appauth.models
-import zcore.core.storage_utils
+import zango.apps.appauth.models
+import zango.core.storage_utils
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
@@ -66,15 +66,15 @@
                         to="permissions.policygroupmodel",
                     ),
                 ),
             ],
             options={
                 "abstract": False,
             },
-            bases=(models.Model, zcore.apps.permissions.mixin.PermissionMixin),
+            bases=(models.Model, zango.apps.permissions.mixin.PermissionMixin),
         ),
         migrations.CreateModel(
             name="AppUserModel",
             fields=[
                 (
                     "id",
                     models.BigAutoField(
@@ -165,15 +165,15 @@
                     models.CharField(max_length=200, null=True, verbose_name="country"),
                 ),
                 (
                     "profile_pic",
                     models.FileField(
                         blank=True,
                         null=True,
-                        upload_to=zcore.core.storage_utils.RandomUniqueFileName,
+                        upload_to=zango.core.storage_utils.RandomUniqueFileName,
                         verbose_name="user profile pic",
                     ),
                 ),
                 ("extra_data", models.JSONField(null=True)),
                 (
                     "policies",
                     models.ManyToManyField(
@@ -196,10 +196,10 @@
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "abstract": False,
             },
-            bases=(models.Model, zcore.apps.permissions.mixin.PermissionMixin),
+            bases=(models.Model, zango.apps.permissions.mixin.PermissionMixin),
         ),
     ]
```

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/migrations/0002_default_user_roles.py` & `zango-0.2.0rc0/src/zango/apps/appauth/migrations/0002_default_user_roles.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py` & `zango-0.2.0rc0/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/migrations/0004_oldpasswords.py` & `zango-0.2.0rc0/src/zango/apps/appauth/migrations/0004_oldpasswords.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/models.py` & `zango-0.2.0rc0/src/zango/apps/appauth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import date, timedelta
 
 from django.db import models
 from django.db.models import Q
 from django.conf import settings
 from django.contrib.auth.hashers import check_password
 
-from zcore.core.model_mixins import FullAuditMixin
+from zango.core.model_mixins import FullAuditMixin
 
-from zcore.apps.object_store.models import ObjectStore
-from zcore.apps.shared.platformauth.abstract_model import AbstractZCoreUserModel
+from zango.apps.object_store.models import ObjectStore
+from zango.apps.shared.platformauth.abstract_model import AbstractZangoUserModel
 
 
-from zcore.core.model_mixins import FullAuditMixin
-from zcore.apps.shared.platformauth.abstract_model import (
-    AbstractZCoreUserModel,
+from zango.core.model_mixins import FullAuditMixin
+from zango.apps.shared.platformauth.abstract_model import (
+    AbstractZangoUserModel,
     AbstractOldPasswords,
 )
 
 from ..permissions.models import PolicyModel, PolicyGroupModel
 
 # from .perm_mixin import PolicyQsMixin
 from ..permissions.mixin import PermissionMixin
@@ -52,15 +52,15 @@
     def delete(self, *args, **kwargs):
         if self.is_default:
             # Prevent deletion of the default object
             raise ValueError("Cannot delete the default object.")
         super().delete(*args, **kwargs)
 
 
-class AppUserModel(AbstractZCoreUserModel, PermissionMixin):
+class AppUserModel(AbstractZangoUserModel, PermissionMixin):
     roles = models.ManyToManyField(UserRoleModel, related_name="users")
     policies = models.ManyToManyField(PolicyModel, related_name="user_policies")
     policy_groups = models.ManyToManyField(
         PolicyGroupModel, related_name="user_policy_groups"
     )
     app_objects = models.JSONField(null=True)
```

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/templates/app.html` & `zango-0.2.0rc0/src/zango/apps/appauth/templates/app.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/templates/app_login_signup.html` & `zango-0.2.0rc0/src/zango/apps/appauth/templates/app_login_signup.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/appauth/views.py` & `zango-0.2.0rc0/src/zango/apps/appauth/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/apps.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from django.conf import settings
 from django.db.models.signals import pre_save
 from .signals import set_created_modified_by
 
 
 class DynamicModelsConfig(AppConfig):
     default_auto_field = "django.db.models.BigAutoField"
-    name = "zcore.apps.dynamic_models"
+    name = "zango.apps.dynamic_models"
 
     def ready(self):
         # thanks to Baserow for this hack
-        import zcore.apps.dynamic_models.signals
+        import zango.apps.dynamic_models.signals
 
         original_register_model = self.apps.register_model
 
         def register_model(app_label, model):
             if "ws_makemigration" in sys.argv or getattr(
                 settings, "TEST_MIGRATION_RUNNING", False
             ):
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/fields/__init__.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/models.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from django.db import models, connection
 from django.db.models import Q
 from django.apps import apps
 from django.core.exceptions import PermissionDenied
 from django.contrib.contenttypes.models import ContentType
 
-from zcore.apps.appauth.models import AppUserModel
-from zcore.core.utils import get_current_request, get_current_role
-from zcore.apps.shared.platformauth.models import PlatformUserModel
-from zcore.apps.dynamic_models.permissions import is_platform_user
+from zango.apps.appauth.models import AppUserModel
+from zango.core.utils import get_current_request, get_current_role
+from zango.apps.shared.platformauth.models import PlatformUserModel
+from zango.apps.dynamic_models.permissions import is_platform_user
 
-from zcore.apps.object_store.models import ObjectStore
+from zango.apps.object_store.models import ObjectStore
 
 
 class RegisterOnceModeMeta(type(models.Model)):
     pass
 
     def __new__(mcs, name, bases, attrs):
         if apps.ready:
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/permissions.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core import signing
 
-from zcore.apps.shared.platformauth.models import PlatformUserModel
+from zango.apps.shared.platformauth.models import PlatformUserModel
 
 
 def is_platform_user(request):
     try:
         token = request.GET.get("token", None)
         user_id = signing.loads(token, max_age=1800)
         user = PlatformUserModel.objects.get(id=user_id)
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/templates/default_landing.html` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/templates/default_landing.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="initial-scale=1.0,maximum-scale=1.0,user-scalable=no" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
     <!-- Remove Tap Highlight on Windows Phone IE -->
     <meta name="msapplication-tap-highlight" content="no" />
 
-    <title>ZCore App Landing Page</title>
+    <title>Zango App Landing Page</title>
 
     <link rel="stylesheet" href="{% static 'app_landing/css/styles.css' %}" />
 </head>
 
 <body>
     
 
@@ -100,15 +100,15 @@
                                         fill="#E1D6AE" />
                                 </g>
                             </svg>
                         </div>
 
                         <div class="card-title">Docs</div>
                         <div class="slide-in-text">
-                            Explore the ZCore Docs
+                            Explore the Zango Docs
                             <a href="https://docs.zelthy.com/" target="_blank" style="text-decoration: none; color: white;">
                                 <button class="card-button">
                                     learn about Docs
                                 </button>
                             </a>
                         </div>
                     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 [https://cdn.builder.io/api/v1/image/assets/TEMP/
 4dbbe9d05256abc545ca036748f8c130cab52148d61d9b8b71adc3b55ebab7c4?]
 Edit your app codebase at {{project_name}}/workspaces/{{app_name}}/
 hello world
 tutorial
 learn how to setup a basic hello world App. _H_e_l_l_o_ _W_o_r_l_d_ _T_u_t_o_r_i_a_l
 Docs
-Explore the ZCore Docs _l_e_a_r_n_ _a_b_o_u_t_ _D_o_c_s
+Explore the Zango Docs _l_e_a_r_n_ _a_b_o_u_t_ _D_o_c_s
 learn about
 packages
 learn about packages _l_e_a_r_n_ _a_b_o_u_t_ _p_a_c_k_a_g_e_s
 permissions
 and policies
 learn how to setup permissions and policies _l_e_a_r_n_ _a_b_o_u_t_ _p_e_r_m_i_s_s_i_o_n_s_ _a_n_d
 _p_o_l_i_c_i_e_s
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/views.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from django.views.decorators.csrf import csrf_exempt, csrf_protect
 from django.utils.decorators import method_decorator
 from django.conf import settings
 
 from django.views.generic import View
 from django.http import Http404
 
-from zcore.core.utils import get_current_role
-from zcore.apps.dynamic_models.permissions import is_platform_user
+from zango.core.utils import get_current_role
+from zango.apps.dynamic_models.permissions import is_platform_user
 
 from .workspace.base import Workspace
 
 
 class PermMixin:
     def has_user_access_perm(self, request, *args, **kwargs):
         if is_platform_user(request):
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/base.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 import os
 import re
 
 from django.conf import settings
 from django.db import connection
 
-from zcore.apps.permissions.models import PolicyModel
-from zcore.apps.appauth.models import UserRoleModel
-from zcore.core.custom_pluginbase import get_plugin_source
+from zango.apps.permissions.models import PolicyModel
+from zango.apps.appauth.models import UserRoleModel
+from zango.core.custom_pluginbase import get_plugin_source
 
 from .lifecycle import Lifecycle
 from .wtree import WorkspaceTreeNode
 
 
 class Workspace:
     """
@@ -80,15 +80,15 @@
             pass
         if request:
             user = request.user
             if user.is_anonymous:
                 role = UserRoleModel.objects.get(name="AnonymousUsers")
                 return role.has_perm(request, "userAccess")
             else:
-                from zcore.core.utils import get_current_role
+                from zango.core.utils import get_current_role
 
                 role = get_current_role()
                 return role.has_perm(request, "userAccess")
         elif as_systemuser:
             # role = UserRoleModel.objects.get(name='SystemUser')
             return True
 
@@ -258,19 +258,19 @@
         return
 
     def sync_tasks(self, tenant_name) -> None:
         """
         get topologically sorted list of tasks from packages and modules and
         import tasks.py files in that order
         """
-        from zcore.config.celery import app
+        from zango.config.celery import app
         from celery import Task
         import inspect
-        from zcore.apps.tasks.models import AppTask
-        from zcore.apps.tasks.utils import get_crontab_obj
+        from zango.apps.tasks.models import AppTask
+        from zango.apps.tasks.utils import get_crontab_obj
 
         task_ids_synced = []
 
         for m in self.get_tasks():
             mod_path = m.split(".")[2:]
             mod_path_str = ".".join(mod_path)
             _plugin = self.plugin_source.load_plugin(mod_path_str)
```

### Comparing `zango-0.2.0a0/src/zcore/apps/dynamic_models/workspace/wtree.py` & `zango-0.2.0rc0/src/zango/apps/dynamic_models/workspace/wtree.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/object_store/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/object_store/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/object_store/models.py` & `zango-0.2.0rc0/src/zango/apps/object_store/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         try:
             # Retrieve the object store instance by UUID
             obj_store_instance = cls.objects.get(object_uuid=object_uuid)
 
             # Check if the object belongs to "dynamic_models" app
             if obj_store_instance.content_type.app_label == "dynamic_models":
-                from zcore.apps.dynamic_models.workspace.base import Workspace
+                from zango.apps.dynamic_models.workspace.base import Workspace
                 from django.db import connection
 
                 model_name = obj_store_instance.content_type.model
                 wobj = Workspace(connection.tenant, as_systemuser=True)
 
                 content_model = []
                 for mod in wobj.get_models():
```

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py` & `zango-0.2.0rc0/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/migrations/0003_default_policy.py` & `zango-0.2.0rc0/src/zango/apps/permissions/migrations/0003_default_policy.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py` & `zango-0.2.0rc0/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/mixin.py` & `zango-0.2.0rc0/src/zango/apps/permissions/mixin.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/permissions/models.py` & `zango-0.2.0rc0/src/zango/apps/permissions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 from django.db.models import Q
 from django.db import models
 from django.db.models import JSONField
 from django.db.models.query import QuerySet
-from zcore.core.model_mixins import FullAuditMixin
+from zango.core.model_mixins import FullAuditMixin
 
 
 class PermissionsModel(FullAuditMixin):
     name = models.CharField("Name of the permission", max_length=100, unique=True)
     type = models.CharField(
         "Type of the permission",
         max_length=50,
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/abstract_model.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/abstract_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from django.utils import timezone
 from django.contrib.auth.models import User
 
 from phonenumber_field.modelfields import PhoneNumberField
 
 
 # from backend.core.storage_utils import S3PrivateFileField, RandomUniqueFileName
-from zcore.core.storage_utils import RandomUniqueFileName
-from zcore.core.model_mixins import FullAuditMixin
+from zango.core.storage_utils import RandomUniqueFileName
+from zango.core.model_mixins import FullAuditMixin
 from phonenumber_field.modelfields import PhoneNumberField
 
 
-class AbstractZCoreUserModel(AbstractBaseUser, FullAuditMixin):
+class AbstractZangoUserModel(AbstractBaseUser, FullAuditMixin):
     name = models.CharField("full name of user", max_length=75)
     email = models.EmailField("email address", null=True, blank=True)
     mobile = PhoneNumberField("mobile number", null=True, blank=True)
     is_active = models.BooleanField(
         "active",
         default=True,
         help_text=(
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/auth_backend.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by Django 4.2.2 on 2023-08-13 04:09
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
-import zcore.core.storage_utils
+import zango.core.storage_utils
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
@@ -109,15 +109,15 @@
                     models.CharField(max_length=200, null=True, verbose_name="country"),
                 ),
                 (
                     "profile_pic",
                     models.FileField(
                         blank=True,
                         null=True,
-                        upload_to=zcore.core.storage_utils.RandomUniqueFileName,
+                        upload_to=zango.core.storage_utils.RandomUniqueFileName,
                         verbose_name="user profile pic",
                     ),
                 ),
                 ("extra_data", models.JSONField(null=True)),
                 (
                     "is_staff",
                     models.BooleanField(
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/models.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 # from phonenumber_field.modelfields import PhoneNumberField
 from django.utils.translation import gettext_lazy as _
 from django.utils import timezone
 
 from django.contrib.auth.models import User
 
-from zcore.apps.shared.tenancy.models import TenantModel
+from zango.apps.shared.tenancy.models import TenantModel
 
-from .abstract_model import AbstractZCoreUserModel
+from .abstract_model import AbstractZangoUserModel
 
-from zcore.core.model_mixins import FullAuditMixin
+from zango.core.model_mixins import FullAuditMixin
 
 
-class PlatformUserModel(AbstractZCoreUserModel):
+class PlatformUserModel(AbstractZangoUserModel):
     is_staff = models.BooleanField(
         _("staff status"),
         default=False,
         help_text="For Django Admin Access. Can be deprecated later",
     )
     is_superadmin = models.BooleanField(
         _("Super Admin"),
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/templates/app_panel/app_panel_login.html` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
   <meta name="viewport" content="initial-scale=1.0,maximum-scale=1.0,user-scalable=no" />
 
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />
   <!-- Remove Tap Highlight on Windows Phone IE -->
   <meta name="msapplication-tap-highlight" content="no" />
 
   <!-- Primary Meta Tags -->
-  <title>ZCore</title>
-  <meta name="title" content="ZCore" />
+  <title>Zango</title>
+  <meta name="title" content="Zango" />
 
   <link rel="preconnect" href="https://fonts.googleapis.com">
   <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
   <link
     href="https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap"
     rel="stylesheet">
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/urls.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/platformauth/views.py` & `zango-0.2.0rc0/src/zango/apps/shared/platformauth/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib.auth.views import LoginView
 from django.shortcuts import redirect
 from rest_framework.views import APIView
-from zcore.core.api import ZCoreSessionPlatformAPIView, get_api_response
+from zango.core.api import ZangoSessionPlatformAPIView, get_api_response
 
 
 # Create your views here.
 class PlatformUserLoginView(LoginView):
     """
     View to render the login page html.
     """
@@ -17,15 +17,15 @@
         return redirect("/platform")
 
 
 class PlatformUserLoginAPIV1(APIView):
     pass
 
 
-class PlatformUserProfileAPIV1(ZCoreSessionPlatformAPIView):
+class PlatformUserProfileAPIV1(ZangoSessionPlatformAPIView):
     """ """
 
     def get_profile_data(self, request):
         data = {}
         data["name"] = request.user.platform_user.name
         data["email"] = request.user.platform_user.email
         data["mobile"] = request.user.platform_user.mobile
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/sync_static.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/sync_static.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.core.management.base import BaseCommand, CommandError
 import os
 import shutil
 from django.conf import settings
 from django.db import connection
-from zcore.apps.shared.tenancy.models import TenantModel
-from zcore.apps.dynamic_models.workspace.base import Workspace
+from zango.apps.shared.tenancy.models import TenantModel
+from zango.apps.dynamic_models.workspace.base import Workspace
 
 
 class Command(BaseCommand):
     help = "Collects assets from the specified app, including packages and copies into \
             the main django asset folder"
 
     def add_arguments(self, parser):
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/ws_makemigration.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from django.conf import settings
 from django.db import connection
 
 from django.core.management.commands.makemigrations import (
     Command as MakeMigrationsCommand,
 )
-from zcore.apps.shared.tenancy.models import TenantModel
-from zcore.apps.dynamic_models.workspace.base import Workspace
+from zango.apps.shared.tenancy.models import TenantModel
+from zango.apps.dynamic_models.workspace.base import Workspace
 
 
 class Command(MakeMigrationsCommand):
     """
     Custom makemigration to generate migration files for dynamic_models. The
     workspace name is a mandatory argument with this command. The workspace is
     initialized and the models are loaded after which the migrations are
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/management/commands/ws_migrate.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from django_tenants.management.commands.migrate_schemas import MigrateSchemasCommand
 from django.conf import settings
 from django.db import connection
-from zcore.apps.shared.tenancy.models import TenantModel
+from zango.apps.shared.tenancy.models import TenantModel
 
 
 class Command(MigrateSchemasCommand):
     # TODO: Handle package migration
 
     def add_arguments(self, parser):
         super().add_arguments(parser)
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by Django 4.2.2 on 2023-08-13 04:09
 
 from django.db import migrations, models
 import django.db.models.deletion
 import django_tenants.postgresql_backend.base
 import uuid
-import zcore.core.storage_utils
+import zango.core.storage_utils
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = []
 
@@ -888,15 +888,15 @@
                     ),
                 ),
                 (
                     "logo",
                     models.FileField(
                         blank=True,
                         null=True,
-                        upload_to=zcore.core.storage_utils.RandomUniqueFileName,
+                        upload_to=zango.core.storage_utils.RandomUniqueFileName,
                         verbose_name="Logo",
                     ),
                 ),
                 ("extra_config", models.JSONField(blank=True, null=True)),
             ],
             options={
                 "abstract": False,
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Generated by Django 4.2.5 on 2023-09-21 16:07
 
 from django.db import migrations
-import zcore.core.storage_utils
+import zango.core.storage_utils
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("tenancy", "0003_themesmodel_created_at_themesmodel_created_by_and_more"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="tenantmodel",
             name="fav_icon",
-            field=zcore.core.storage_utils.ZFileField(
+            field=zango.core.storage_utils.ZFileField(
                 blank=True,
                 null=True,
-                upload_to=zcore.core.storage_utils.RandomUniqueFileName,
-                validators=[zcore.core.storage_utils.validate_file_extension],
+                upload_to=zango.core.storage_utils.RandomUniqueFileName,
+                validators=[zango.core.storage_utils.validate_file_extension],
                 verbose_name="Fav Icon",
             ),
         ),
         migrations.AlterField(
             model_name="tenantmodel",
             name="logo",
-            field=zcore.core.storage_utils.ZFileField(
+            field=zango.core.storage_utils.ZFileField(
                 blank=True,
                 null=True,
-                upload_to=zcore.core.storage_utils.RandomUniqueFileName,
-                validators=[zcore.core.storage_utils.validate_file_extension],
+                upload_to=zango.core.storage_utils.RandomUniqueFileName,
+                validators=[zango.core.storage_utils.validate_file_extension],
                 verbose_name="Logo",
             ),
         ),
     ]
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/models.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from django.db import models
 from django.utils import timezone
 from django.conf import settings
 from django_tenants.models import TenantMixin, DomainMixin
 from django.core.exceptions import ValidationError
 
-from zcore.core.model_mixins import FullAuditMixin
-from zcore.core.storage_utils import RandomUniqueFileName, ZFileField
-from zcore.apps.permissions.models import PolicyModel
-from zcore.apps.appauth.models import UserRoleModel
+from zango.core.model_mixins import FullAuditMixin
+from zango.core.storage_utils import RandomUniqueFileName, ZFileField
+from zango.apps.permissions.models import PolicyModel
+from zango.apps.appauth.models import UserRoleModel
 
 
 from .tasks import initialize_workspace
 
 
 from .utils import (
     TIMEZONES,
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/tasks.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from .utils import assign_policies_to_anonymous_user, DEFAULT_THEME_CONFIG
 
 
 @shared_task
 def initialize_workspace(tenant_uuid):
     try:
-        from zcore.apps.shared.tenancy.models import TenantModel, ThemesModel
+        from zango.apps.shared.tenancy.models import TenantModel, ThemesModel
 
         tenant = TenantModel.objects.get(uuid=tenant_uuid)
 
         # Creating schema
         tenant.create_schema(check_if_exists=True)
 
         # migrating schema
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/templates/app_panel.html` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/templates/app_panel.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width,initial-scale=1" />
   <meta name="theme-color" content="#000000" />
-  <meta name="description" content="ZCore App Panel" />
-  <title>ZCore App Panel</title>
+  <meta name="description" content="Zango App Panel" />
+  <title>Zango App Panel</title>
 </head>
 
 <body>
   <noscript>You need to enable JavaScript to run this app.</noscript>
   <div id="root"></div>
   <script>
     var csrf_token = "{{ csrf_token }}";
```

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/templatetags/zstatic.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/templatetags/zstatic.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/shared/tenancy/utils.py` & `zango-0.2.0rc0/src/zango/apps/shared/tenancy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytz
 
 from django_tenants.utils import schema_context
 
-from zcore.apps.permissions.models import PolicyModel
-from zcore.apps.appauth.models import UserRoleModel
+from zango.apps.permissions.models import PolicyModel
+from zango.apps.appauth.models import UserRoleModel
 
 __all__ = [
     "TIMEZONES",
     "DATEFORMAT",
     "DATETIMEFORMAT",
 ]
```

### Comparing `zango-0.2.0a0/src/zcore/apps/tasks/migrations/0001_initial.py` & `zango-0.2.0rc0/src/zango/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/apps/tasks/models.py` & `zango-0.2.0rc0/src/zango/apps/tasks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 
 from django.db import models
 from django_celery_beat.models import CrontabSchedule, IntervalSchedule
 from django_celery_beat.models import PeriodicTask
 
-from zcore.core.model_mixins import FullAuditMixin
-from zcore.apps.permissions.models import PolicyModel
+from zango.core.model_mixins import FullAuditMixin
+from zango.apps.permissions.models import PolicyModel
 
 
 class AppTask(FullAuditMixin):
     name = models.CharField(max_length=255, unique=True)
     is_enabled = models.BooleanField(default=False)
     is_deleted = models.BooleanField(default=False)
-    task = "zcore.core.tasks.zcore_task_executor"
+    task = "zango.core.tasks.zango_task_executor"
     interval = models.ForeignKey(
         IntervalSchedule,
         on_delete=models.CASCADE,
         null=True,
         blank=True,
         verbose_name="interval",
     )
```

### Comparing `zango-0.2.0a0/src/zcore/apps/tasks/utils.py` & `zango-0.2.0rc0/src/zango/apps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_landing/css/styles.css` & `zango-0.2.0rc0/src/zango/assets/app_landing/css/styles.css`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/css/styles.css` & `zango-0.2.0rc0/src/zango/assets/app_panel/css/styles.css`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogo.svg` & `zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogo.svg`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogoIpad.svg` & `zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogoIpad.svg`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/images/zelthyLogoIphone.svg` & `zango-0.2.0rc0/src/zango/assets/app_panel/images/zelthyLogoIphone.svg`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.42.min.js` & `zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.42.min.js`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.43.min.js` & `zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.43.min.js`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/app_panel/js/build.v1.0.44.min.js` & `zango-0.2.0rc0/src/zango/assets/app_panel/js/build.v1.0.44.min.js`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/assets/js/jquery/3.7.1/jquery.min.js` & `zango-0.2.0rc0/src/zango/assets/js/jquery/3.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/cli/install_package.py` & `zango-0.2.0rc0/src/zango/cli/install_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from zcore.core.package_utils import install_package as install_pkg
+from zango.core.package_utils import install_package as install_pkg
 
 
 @click.command("install-package")
 @click.argument("package_name")
 @click.option("--version", prompt=True, help="Version", default="latest")
 @click.option("--tenants", prompt=True, help="Tenants")
 @click.option("--skip-static", is_flag=True, help="Skip Static")
```

### Comparing `zango-0.2.0a0/src/zcore/cli/package_info.py` & `zango-0.2.0rc0/src/zango/cli/package_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import click
 import json
 
-from zcore.core.package_utils import get_all_packages
+from zango.core.package_utils import get_all_packages
 
 
 @click.command("list-packages")
 @click.option("--tenant", help="Tenant", default=None)
 def list_packages(tenant):
     available_packages = get_all_packages()
     tenants = []
```

### Comparing `zango-0.2.0a0/src/zcore/cli/project_template/manage.py` & `zango-0.2.0rc0/src/zango/cli/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/cli/project_template/project_name/settings.py` & `zango-0.2.0rc0/src/zango/cli/project_template/project_name/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 import environ
 
-from zcore.config.settings.base import *
+from zango.config.settings.base import *
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 env = environ.Env(
     DEBUG=(bool, True),
     REDIS_HOST=(str, "127.0.0.1"),
     REDIS_PORT=(str, "6379"),
@@ -82,15 +82,15 @@
 # ROOT_URLCONF = '{{project_name}}.urls'
 
 import os
 
 TEMPLATES[0]["DIRS"] = [os.path.join(BASE_DIR, "templates")]
 
 SHOW_PUBLIC_IF_NO_TENANT_FOUND = False
-PUBLIC_SCHEMA_URLCONF = "zcore.config.urls_public"
+PUBLIC_SCHEMA_URLCONF = "zango.config.urls_public"
 ROOT_URLCONF = f"{PROJECT_NAME}.urls_tenants"
 
 ENV = "dev"
 
 PHONENUMBER_DEFAULT_REGION = "IN"
 
 MEDIA_URL = "/media/"
@@ -104,16 +104,16 @@
     "default": {"BACKEND": "django.core.files.storage.FileSystemStorage"},
     "staticfiles": {"BACKEND": "django.contrib.staticfiles.storage.StaticFilesStorage"},
 }
 
 # To change the media storage to S3 you can use the BACKEND class provided by the default storage
 # To change the static storage to S3 you can use the BACKEND class provided by the staticfiles storage
 # STORAGES = {
-#     "default": {"BACKEND": "zcore.core.storage_utils.S3MediaStorage"},
-#     "staticfiles": {"BACKEND": "zcore.core.storage_utils.S3StaticStorage"},
+#     "default": {"BACKEND": "zango.core.storage_utils.S3MediaStorage"},
+#     "staticfiles": {"BACKEND": "zango.core.storage_utils.S3StaticStorage"},
 # }
 #
 AWS_MEDIA_STORAGE_BUCKET_NAME = "media"  # S3 Bucket Name
 AWS_MEDIA_STORAGE_LOCATION = "media"  # Prefix added to all the files uploaded
 AWS_STATIC_STORAGE_BUCKET_NAME = "static"  # S3 Bucket Name
 AWS_STATIC_STORAGE_LOCATION = "static"  # Prefix added to all the files uploaded
```

### Comparing `zango-0.2.0a0/src/zcore/cli/project_template/project_name/urls.py` & `zango-0.2.0rc0/src/zango/cli/project_template/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/cli/start_project.py` & `zango-0.2.0rc0/src/zango/cli/start_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import psycopg2
 import click
 
 import django
 from django.core.management import call_command
 
-import zcore
+import zango
 from .utils import replace_placeholders_in_file
 
 
 def test_db_conection(db_name, db_user, db_password, db_host, db_port):
     """
     Establishes a connection to a PostgreSQL database using the provided credentials.
 
@@ -86,15 +86,15 @@
 
     project_root = get_project_root(project_name, directory=directory)
 
     if os.path.exists(project_root):
         return False, f"Folder already exists: {project_root}"
 
     project_template_path = os.path.join(
-        os.path.dirname(zcore.cli.__file__), "project_template"
+        os.path.dirname(zango.cli.__file__), "project_template"
     )
     command = f"{command} --template {str(project_template_path)}"
 
     subprocess.run(command, shell=True, check=True)
     env_file = open(f".env", "w")
     env_file.write(
         f"POSTGRES_DB={db_name}\nPOSTGRES_USER={db_user}\nPOSTGRES_PASSWORD={db_password}\nPOSTGRES_HOST={db_host}\nPOSTGRES_PORT={db_port}\nREDIS_HOST={redis_host}\nREDIS_PORT={redis_port}\nPROJECT_NAME={project_name}\n"
@@ -104,15 +104,15 @@
     return True, "Project created successfully"
 
     # PROJECT_ROOT = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     # sys.path.insert(
 
 
 def create_public_tenant(platform_domain_url="localhost"):
-    from zcore.apps.shared.tenancy.models import TenantModel, Domain
+    from zango.apps.shared.tenancy.models import TenantModel, Domain
 
     # Creating public tenant
     if not TenantModel.objects.filter(schema_name="public").exists():
         public_tenant = TenantModel.objects.create(
             name="public",
             schema_name="public",
             description="Public Tenant",
@@ -122,15 +122,15 @@
         # Creating domain
         Domain.objects.create(
             tenant=public_tenant, domain=platform_domain_url, is_primary=True
         )
 
 
 def create_platform_user(platform_username, platform_username_password):
-    from zcore.apps.shared.platformauth.models import PlatformUserModel
+    from zango.apps.shared.platformauth.models import PlatformUserModel
 
     # Creating default SuperAdmin User
     result = PlatformUserModel.create_user(
         name="Default Super Admin",
         email=platform_username,
         mobile="",
         password=platform_username_password,
```

### Comparing `zango-0.2.0a0/src/zcore/cli/utils.py` & `zango-0.2.0rc0/src/zango/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/config/celery.py` & `zango-0.2.0rc0/src/zango/config/celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 current_project_dir = os.getcwd()
 project_name = os.path.basename(current_project_dir)
 
 # Setting the Django settings module to the current project's settings
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", f"{project_name}.settings")
 
 # Creating a Celery application instance
-app = Celery("zcore")
+app = Celery("zango")
 
 # Configuring the Celery app using the Django settings
 app.config_from_object("django.conf:settings", namespace="CELERY")
 
 # Discovering and registering task modules
 app.autodiscover_tasks()
```

### Comparing `zango-0.2.0a0/src/zcore/config/settings/base.py` & `zango-0.2.0rc0/src/zango/config/settings/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import os
 
-import zcore
+import zango
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
 
@@ -31,27 +31,27 @@
     # 'axes',
     "session_security",
     "django_celery_beat",
     "django_celery_results",
     "rest_framework",
     "knox",
     # 'nocaptcha_recaptcha',
-    "zcore.apps.shared.tenancy",
-    "zcore.apps.shared.platformauth",
+    "zango.apps.shared.tenancy",
+    "zango.apps.shared.platformauth",
 ]
 
 
 TENANT_APPS = [
     # The following Django contrib apps must be in TENANT_APPS
     "django.contrib.contenttypes",
-    "zcore.apps.appauth",
-    "zcore.apps.permissions",
-    "zcore.apps.object_store",
-    "zcore.apps.dynamic_models",
-    "zcore.apps.tasks",
+    "zango.apps.appauth",
+    "zango.apps.permissions",
+    "zango.apps.object_store",
+    "zango.apps.dynamic_models",
+    "zango.apps.tasks",
     "corsheaders",
     "crispy_forms",
     "crispy_bootstrap5",
     "debug_toolbar",
     "crispy_forms",
     "django_celery_results",
     # "cachalot",
@@ -62,38 +62,38 @@
 ]
 
 TENANT_MODEL = "tenancy.TenantModel"
 TENANT_DOMAIN_MODEL = "tenancy.Domain"
 
 
 MIDDLEWARE = [
-    "zcore.middleware.tenant.ZCoreTenantMainMiddleware",
-    # 'zcore.middleware.context_middleware.SimpleContextMiddleware',
-    # 'zcore.middleware.tenant_url_switch.url_switch_middleware',
+    "zango.middleware.tenant.ZangoTenantMainMiddleware",
+    # 'zango.middleware.context_middleware.SimpleContextMiddleware',
+    # 'zango.middleware.tenant_url_switch.url_switch_middleware',
     # 'django_tenants.middleware.main.TenantMainMiddleware',
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "session_security.middleware.SessionSecurityMiddleware",
-    "zcore.middleware.request.UserRoleAndAppObjectAssignmentMiddleware",
-    # 'zcore.middleware.middleware.SetUserRoleMiddleWare',
+    "zango.middleware.request.UserRoleAndAppObjectAssignmentMiddleware",
+    # 'zango.middleware.middleware.SetUserRoleMiddleWare',
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
     "django.middleware.common.CommonMiddleware",
     "corsheaders.middleware.CorsMiddleware",
     "debug_toolbar.middleware.DebugToolbarMiddleware",
-    "zcore.middleware.tenant.TimezoneMiddleware",
+    "zango.middleware.tenant.TimezoneMiddleware",
 ]
 
 
 AUTHENTICATION_BACKENDS = (
-    "zcore.apps.shared.platformauth.auth_backend.PlatformUserModelBackend",
-    "zcore.apps.appauth.auth_backend.AppUserModelBackend",
+    "zango.apps.shared.platformauth.auth_backend.PlatformUserModelBackend",
+    "zango.apps.appauth.auth_backend.AppUserModelBackend",
 )
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
         "DIRS": [],
         "APP_DIRS": False,
@@ -104,15 +104,15 @@
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
             ],
             # 'builtins': [
             #     'django.contrib.staticfiles',  # Add this line
             # ],
             "loaders": [
-                "zcore.core.template_loader.AppTemplateLoader",
+                "zango.core.template_loader.AppTemplateLoader",
                 "django.template.loaders.filesystem.Loader",
                 "django.template.loaders.app_directories.Loader",
             ],
         },
     },
 ]
 
@@ -129,26 +129,26 @@
 ]
 
 # DEBUG_TOOLBAR_PANELS += ['cachalot.panels.CachalotPanel',]
 
 CACHALOT_ENABLED = False
 
 STATIC_URL = "static/"
-STATICFILES_DIRS = [os.path.join(os.path.dirname(zcore.__file__), "assets")]
+STATICFILES_DIRS = [os.path.join(os.path.dirname(zango.__file__), "assets")]
 
 
 CRISPY_ALLOWED_TEMPLATE_PACKS = (
     "ukcrisp",
     "uni_form",
     "bootstrap5",
 )
 
 CRISPY_TEMPLATE_PACK = "bootstrap5"
 
-SESSION_COOKIE_NAME = "zcorecookie"
+SESSION_COOKIE_NAME = "zangocookie"
 SESSION_COOKIE_SECURE = True
 CSRF_COOKIE_SECURE = True
 
 LOGOUT_REDIRECT_URL = "/admin/login"
 
 PASSWORD_MIN_LENGTH = 8
 PASSWORD_NO_REPEAT_DAYS = 180
```

### Comparing `zango-0.2.0a0/src/zcore/config/urls_public.py` & `zango-0.2.0rc0/src/zango/config/urls_public.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from django.urls import path, include
 from django.urls import re_path
 from django.contrib import admin
 from django.conf import settings
 from django.conf.urls.static import static
 
-from zcore.apps.shared.platformauth.views import (
+from zango.apps.shared.platformauth.views import (
     PlatformUserLoginView,
 )
 
 urlpatterns = [
     re_path(
         r"^admin/login/$",
         PlatformUserLoginView.as_view(),
         name="login",
     ),
     re_path(r"^admin/", admin.site.urls),
-    re_path(r"^api/", include("zcore.api.platform.urls")),
+    re_path(r"^api/", include("zango.api.platform.urls")),
     re_path(r"api/auth/", include("knox.urls")),
     re_path(r"session_security/", include("session_security.urls")),
-    re_path(r"^", include("zcore.apps.shared.tenancy.urls")),
+    re_path(r"^", include("zango.apps.shared.tenancy.urls")),
 ]
 if settings.DEBUG:
     urlpatterns += [
         path("__debug__/", include("debug_toolbar.urls")),
     ]
     urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
```

### Comparing `zango-0.2.0a0/src/zcore/config/urls_tenants.py` & `zango-0.2.0rc0/src/zango/config/urls_tenants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django.urls import include
 from django.urls import re_path, path
 from django.conf import settings
 from django.conf.urls.static import static
 
 urlpatterns = [
-    re_path(r"^", include("zcore.apps.appauth.urls")),
+    re_path(r"^", include("zango.apps.appauth.urls")),
     re_path(r"api/auth/", include("knox.urls")),
-    re_path(r"api/", include("zcore.api.app_auth.urls")),
+    re_path(r"api/", include("zango.api.app_auth.urls")),
     re_path(r"session_security/", include("session_security.urls")),
 ]
 
 if settings.DEBUG:
     urlpatterns += [
         path("__debug__/", include("debug_toolbar.urls")),
     ]
     urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 
 # include dynamic views
 urlpatterns += [
-    re_path(r"^((?:[\w\-:.,]+/)*)$", include("zcore.apps.dynamic_models.urls")),
+    re_path(r"^((?:[\w\-:.,]+/)*)$", include("zango.apps.dynamic_models.urls")),
 ]
```

### Comparing `zango-0.2.0a0/src/zcore/core/api/base.py` & `zango-0.2.0rc0/src/zango/core/api/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from rest_framework.views import APIView
 from rest_framework.authentication import SessionAuthentication
 from knox.auth import TokenAuthentication
 
 from ..permissions import IsAuthenticatedPlatformUser, IsAuthenticatedAppUser
 
 
-class ZCoreSessionPlatformAPIView(APIView):
+class ZangoSessionPlatformAPIView(APIView):
     """
     This is the base class for developing Platform APIs that need to support only session based
     authentication. Expected use cases include APIs that must be supported only with session and NOT token
     """
 
     authentication_classes = (SessionAuthentication,)
     permission_classes = (IsAuthenticatedPlatformUser,)
 
 
-class ZCoreSessionAppAPIView(APIView):
+class ZangoSessionAppAPIView(APIView):
     """
     Base API view for developing Session Authenticated Platform APIs
     Use Case: Platform APIs accessed by the web apps on the same domain
     CSRF Not Exempted
-    This API expects zcorecookie & csrftoken as Cookies. zcorecookie should
+    This API expects zangocookie & csrftoken as Cookies. zangocookie should
     represent an active platform user.
     Additional Perms: Request should pass whitelisting setting of Platform
     """
 
     authentication_classes = (SessionAuthentication,)
     permission_classes = (IsAuthenticatedAppUser,)
 
 
-class ZCoreTokenPlatformAPIView(APIView):
+class ZangoTokenPlatformAPIView(APIView):
     """
     This is the base class for developing Platform APIs that need to support only token based
     authentication. Expected use cases include APIs that will be used by third parties only
     """
 
     authentication_classes = (TokenAuthentication,)
     permission_classes = (IsAuthenticatedPlatformUser,)
 
 
-class ZCoreGenericPlatformAPIView(APIView):
+class ZangoGenericPlatformAPIView(APIView):
     """
     This is the base auth class for developing Platform APIs that need to support both
     token based authentication as well as session cookie based authentication.
-    The ZCore platform webapp must use session based authentication and should provide csrftoken as well.
+    The Zango platform webapp must use session based authentication and should provide csrftoken as well.
     """
 
     authentication_classes = (SessionAuthentication, TokenAuthentication)
     permission_classes = (IsAuthenticatedPlatformUser,)
 
 
-class ZCoreGenericAppAPIView(APIView):
+class ZangoGenericAppAPIView(APIView):
     authentication_classes = (TokenAuthentication, SessionAuthentication)
     permission_classes = (IsAuthenticatedAppUser,)
```

### Comparing `zango-0.2.0a0/src/zcore/core/api/utils.py` & `zango-0.2.0rc0/src/zango/core/api/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from collections import OrderedDict
 
 from django.http import HttpResponse
 from rest_framework.pagination import PageNumberPagination
 
 
-class ZCoreAPIPagination(PageNumberPagination):
+class ZangoAPIPagination(PageNumberPagination):
     page_size = 10
     page_size_query_param = "page_size"
     max_page_size = 100
 
     def get_paginated_response_data(self, data):
         return OrderedDict(
             [
```

### Comparing `zango-0.2.0a0/src/zcore/core/common_utils.py` & `zango-0.2.0rc0/src/zango/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/custom_pluginbase.py` & `zango-0.2.0rc0/src/zango/core/custom_pluginbase.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/generic_views/base.py` & `zango-0.2.0rc0/src/zango/core/generic_views/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from django.views.generic import View, TemplateView
 from django.contrib.auth.decorators import login_required
 from ..permissions import IsAuthenticatedPlatformUser, IsAuthenticatedAppUser
 
 
-class ZCoreSessionPlatformView(IsAuthenticatedPlatformUser, View):
+class ZangoSessionPlatformView(IsAuthenticatedPlatformUser, View):
     """
     View only accessible to authenticated platform users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZCoreSessionPlatformView, cls).as_view(), login_url=login_url
+            super(ZangoSessionPlatformView, cls).as_view(), login_url=login_url
         )
 
 
-class ZCoreSessionPlatformTemplateView(IsAuthenticatedPlatformUser, TemplateView):
+class ZangoSessionPlatformTemplateView(IsAuthenticatedPlatformUser, TemplateView):
     """
     TemplateView only accessible to authenticated platform users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = "/admin/login/"
         return login_required(
-            super(ZCoreSessionPlatformTemplateView, cls).as_view(), login_url=login_url
+            super(ZangoSessionPlatformTemplateView, cls).as_view(), login_url=login_url
         )
 
 
-class ZCoreSessionAppView(IsAuthenticatedAppUser, View):
+class ZangoSessionAppView(IsAuthenticatedAppUser, View):
     """
     View only accessible to authenticated app users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZCoreSessionAppView, cls).as_view(), login_url=login_url
+            super(ZangoSessionAppView, cls).as_view(), login_url=login_url
         )
 
-class ZCoreSessionAppTemplateView(IsAuthenticatedAppUser, TemplateView):
+
+class ZangoSessionAppTemplateView(IsAuthenticatedAppUser, TemplateView):
     """
     TemplateView only accessible to authenticated app users.
     """
 
     @classmethod
     def as_view(cls):
         login_url = None
         return login_required(
-            super(ZCoreSessionAppTemplateView, cls).as_view(), login_url=login_url
+            super(ZangoSessionAppTemplateView, cls).as_view(), login_url=login_url
         )
```

### Comparing `zango-0.2.0a0/src/zcore/core/internal_requests.py` & `zango-0.2.0rc0/src/zango/core/internal_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return domain_obj
 
 
 def process_internal_request(fake_request, tenant, **kwargs):
     fake_request.tenant = tenant
     fake_request.internal_routing = True
     connection.set_tenant(tenant)
-    ws_module = import_module("zcore.apps.dynamic_models.workspace.base")
+    ws_module = import_module("zango.apps.dynamic_models.workspace.base")
     ws_klass = getattr(ws_module, "Workspace")
     ws = ws_klass(tenant, fake_request)
     ws.ready()
     view, resolve = ws.match_view(fake_request)
     response = view(fake_request, (), **kwargs)
     return response
```

### Comparing `zango-0.2.0a0/src/zcore/core/model_mixins.py` & `zango-0.2.0rc0/src/zango/core/model_mixins.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/package_utils.py` & `zango-0.2.0rc0/src/zango/core/package_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import boto3
 from botocore import UNSIGNED
 from botocore.config import Config
 
 from django.conf import settings
 from django.db import connection
 
-from zcore.core.utils import get_current_request_url
+from zango.core.utils import get_current_request_url
 
 
 def create_directories(dirs):
     for directory in dirs:
         if not os.path.exists(directory):
             os.makedirs(directory)
 
@@ -165,16 +165,16 @@
         subprocess.run("python manage.py collectstatic --noinput", shell=True)
         if os.path.exists(f"workspaces/{tenant}/packages/{package_name}/migrations"):
             subprocess.run(
                 f"python manage.py ws_migrate {tenant} --package {package_name}",
                 shell=True,
             )
 
-        from zcore.apps.dynamic_models.workspace.base import Workspace
-        from zcore.apps.shared.tenancy.models import TenantModel
+        from zango.apps.dynamic_models.workspace.base import Workspace
+        from zango.apps.shared.tenancy.models import TenantModel
 
         tenant_obj = TenantModel.objects.get(name=tenant)
         connection.set_tenant(tenant_obj)
         with connection.cursor() as c:
             ws = Workspace(connection.tenant, request=None, as_systemuser=True)
             ws.ready()
             ws.sync_tasks(tenant)
```

### Comparing `zango-0.2.0a0/src/zcore/core/permissions.py` & `zango-0.2.0rc0/src/zango/core/permissions.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/storage_utils.py` & `zango-0.2.0rc0/src/zango/core/storage_utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/tasks.py` & `zango-0.2.0rc0/src/zango/core/tasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import partial
 from celery import shared_task, current_task
 from django.db import connection
 
 
 @shared_task
-def zcore_task_executor(tenant_name, task_name, *args, **kwargs):
-    from zcore.apps.dynamic_models.workspace.base import Workspace
-    from zcore.apps.shared.tenancy.models import TenantModel
-    from zcore.apps.tasks.models import AppTask
+def zango_task_executor(tenant_name, task_name, *args, **kwargs):
+    from zango.apps.dynamic_models.workspace.base import Workspace
+    from zango.apps.shared.tenancy.models import TenantModel
+    from zango.apps.tasks.models import AppTask
 
     tenant = TenantModel.objects.get(name=tenant_name)
 
     connection.set_tenant(tenant)
     with connection.cursor() as c:
         task_obj = AppTask.objects.get(name=task_name)
 
@@ -21,18 +21,18 @@
         task_module = task_obj.name.rsplit(".", 1)[0]
         func_name = task_obj.name.rsplit(".", 1)[1]
         _task = ws.plugin_source.load_plugin(f"{task_module}")
         task_fun = getattr(_task, func_name)
         return task_fun(*args, **kwargs)
 
 
-def zcore_task(task_fun, *args, **kwargs):
-    def get_zcore_task_executor(**options):
-        return zcore_task_executor
+def zango_task(task_fun, *args, **kwargs):
+    def get_zango_task_executor(**options):
+        return zango_task_executor
 
     def original_function(*args, **kwargs):
         return task_fun(*args, **kwargs)
 
-    task_executor = get_zcore_task_executor()
+    task_executor = get_zango_task_executor()
     task_executor.original_function = original_function
 
     return task_executor
```

### Comparing `zango-0.2.0a0/src/zcore/core/template_loader.py` & `zango-0.2.0rc0/src/zango/core/template_loader.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/core/utils.py` & `zango-0.2.0rc0/src/zango/core/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/middleware/request.py` & `zango-0.2.0rc0/src/zango/middleware/request.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0a0/src/zcore/middleware/tenant.py` & `zango-0.2.0rc0/src/zango/middleware/tenant.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     get_public_schema_urlconf,
 )
 from django_tenants.middleware.main import TenantMainMiddleware
 from django.conf import settings
 from django.utils import timezone
 
 
-class ZCoreTenantMainMiddleware(TenantMainMiddleware):
+class ZangoTenantMainMiddleware(TenantMainMiddleware):
     TENANT_NOT_FOUND_EXCEPTION = Http404
 
     @staticmethod
     def hostname_from_request(request):
         """
         Static method to extract hostname from request.
```

