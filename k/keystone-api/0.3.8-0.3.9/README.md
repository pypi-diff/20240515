# Comparing `tmp/keystone_api-0.3.8.tar.gz` & `tmp/keystone_api-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.8.tar", max compression
+gzip compressed data, was "keystone_api-0.3.9.tar", max compression
```

## Comparing `keystone_api-0.3.8.tar` & `keystone_api-0.3.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0    13578 2024-05-07 15:51:21.888062 keystone_api-0.3.8/README.md
--rw-r--r--   0        0        0      428 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.888062 keystone_api-0.3.8/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3618 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     5191 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     5590 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      572 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/tasks.py
--rw-r--r--   0        0        0      444 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/__init__.py
--rw-r--r--   0        0        0     1213 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckJsonView.py
--rw-r--r--   0        0        0      978 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckPrometheusView.py
--rw-r--r--   0        0        0     1094 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckView.py
--rw-r--r--   0        0        0      667 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/tests/views/utils.py
--rw-r--r--   0        0        0      345 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     3569 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     2496 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/admin.py
--rw-r--r--   0        0        0     1101 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1828 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0      644 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
--rw-r--r--   0        0        0      638 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/0003_taskresult.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0     1112 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      733 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/__init__.py
--rw-r--r--   0        0        0     2560 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2390 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1791 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
--rw-r--r--   0        0        0      322 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0     1284 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/openapi/__init__.py
--rw-r--r--   0        0        0      326 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/openapi/urls.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1705 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1261 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/managers.py
--rw-r--r--   0        0        0     1677 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0      437 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1776 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0     2862 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/permissions.py
--rw-r--r--   0        0        0      928 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      338 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0     1554 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0      834 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0      654 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/apps.py
--rw-r--r--   0        0        0     1649 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0      875 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/scheduler/checks.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0      402 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/0003_alter_researchgroup_name.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2383 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2095 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.892062 keystone_api-0.3.8/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     8125 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1058 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3921 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     2626 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0     2908 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test_json.py
--rw-r--r--   0        0        0     2908 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/health/test_prom.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0     2873 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/logging/test_tasks.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/test_json.py
--rw-r--r--   0        0        0     2867 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/openapi/test_yaml.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/__init__.py
--rw-r--r--   0        0        0     5611 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_grants.py
--rw-r--r--   0        0        0     4524 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_grants_pk.py
--rw-r--r--   0        0        0     5782 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_publications.py
--rw-r--r--   0        0        0     4438 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/research/test_publications_pk.py
--rw-r--r--   0        0        0        0 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2022 2024-05-07 15:51:21.896062 keystone_api-0.3.8/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      957 2024-05-07 15:51:34.851966 keystone_api-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    13785 2024-05-07 19:12:02.428153 keystone_api-0.3.9/README.md
+-rw-r--r--   0        0        0      428 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3618 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     5191 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     5590 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/views/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckJsonView.py
+-rw-r--r--   0        0        0      978 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckPrometheusView.py
+-rw-r--r--   0        0        0     1094 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckView.py
+-rw-r--r--   0        0        0      667 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/tests/views/utils.py
+-rw-r--r--   0        0        0      345 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     3569 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     2496 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/admin.py
+-rw-r--r--   0        0        0     1101 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1828 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0      644 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
+-rw-r--r--   0        0        0      638 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/migrations/0003_taskresult.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1645 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0     1112 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      733 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/handlers/__init__.py
+-rw-r--r--   0        0        0     2560 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2390 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1791 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
+-rw-r--r--   0        0        0      322 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0     1284 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/openapi/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/openapi/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1261 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/managers.py
+-rw-r--r--   0        0        0     1677 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0      437 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1776 2024-05-07 19:12:02.428153 keystone_api-0.3.9/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0     2862 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/research_products/permissions.py
+-rw-r--r--   0        0        0      928 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      338 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0     1554 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0      654 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/scheduler/apps.py
+-rw-r--r--   0        0        0     1649 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0      875 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/scheduler/checks.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0      402 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/migrations/0003_alter_researchgroup_name.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2383 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     8344 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1058 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3921 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0     2908 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/health/test_json.py
+-rw-r--r--   0        0        0     2908 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/health/test_prom.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0     2873 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/logging/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/openapi/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/openapi/test_json.py
+-rw-r--r--   0        0        0     2867 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/openapi/test_yaml.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/research/__init__.py
+-rw-r--r--   0        0        0     5611 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/research/test_grants.py
+-rw-r--r--   0        0        0     4524 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/research/test_grants_pk.py
+-rw-r--r--   0        0        0     5782 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/research/test_publications.py
+-rw-r--r--   0        0        0     4438 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/research/test_publications_pk.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2022 2024-05-07 19:12:02.432153 keystone_api-0.3.9/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-05-07 19:12:15.444170 keystone_api-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    14980 1970-01-01 00:00:00.000000 keystone_api-0.3.9/PKG-INFO
```

### Comparing `keystone_api-0.3.8/README.md` & `keystone_api-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,27 @@
 - Avoid issuing session/CSRF tokens over unsecured connections by enabling `SECURE_SESSION_TOKENS`
 - Always use a secure `SECURE_SECRET_KEY` value to ensure proper request signing across application instances/restarts
 - Consider using HTTP Strict Transport Security (HSTS) to enforce the use of HTTPS
 
 The `SECURE_SECRET_KEY` value may be changed at any given time. However, doing so may invalidate any active user
 sessions and require users to reauthenticate.
 
-| Setting Name              | Default Value            | Description                                                   |
-|---------------------------|--------------------------|---------------------------------------------------------------|
-| `SECURE_SECRET_KEY`       | Randomly generated       | Secret key used to enforce cryptographic signing.             |
-| `SECURE_ALLOWED_HOSTS`    | `localhost,127.0.0.1`    | Comma-separated list of accepted host/domain names.           |
-| `SECURE_SSL_REDIRECT`     | `False`                  | Automatically redirect all HTTP traffic to HTTPS.             |
-| `SECURE_SESSION_TOKENS`   | `False`                  | Only issue session/CSRF tokens over secure connections.       |
-| `SECURE_CSRF_ORIGINS`     | `[]`                     | Domains (with protocol) to accept CSRF headers from.          |
-| `SECURE_HSTS_SECONDS`     | `0` (Disabled)           | HSTS cache duration in seconds.                               |
-| `SECURE_HSTS_SUBDOMAINS`  | `False`                  | Enable HSTS for subdomains.                                   |
-| `SECURE_HSTS_PRELOAD`     | `False`                  | Enable HSTS preload functionality.                            |
+| Setting Name                    | Default Value         | Description                                             |
+|---------------------------------|-----------------------|---------------------------------------------------------|
+| `SECURE_SECRET_KEY`             | Randomly generated    | Secret key used to enforce cryptographic signing.       |
+| `SECURE_ALLOWED_HOSTS`          | `localhost,127.0.0.1` | Comma-separated list of accepted host/domain names.     |
+| `SECURE_SSL_REDIRECT`           | `False`               | Automatically redirect all HTTP traffic to HTTPS.       |
+| `SECURE_SESSION_TOKENS`         | `False`               | Only issue session/CSRF tokens over secure connections. |
+| `SECURE_CSRF_ORIGINS`           | `[]`                  | Domains (with protocol) to accept CSRF headers from.    |
+| `SECURE_HSTS_SECONDS`           | `0` (Disabled)        | HSTS cache duration in seconds.                         |
+| `SECURE_HSTS_SUBDOMAINS`        | `False`               | Enable HSTS for subdomains.                             |
+| `SECURE_HSTS_PRELOAD`           | `False`               | Enable HSTS preload functionality.                      |
+| `SECURE_ACCESS_TOKEN_LIFETIME`  | `300` (5 Minutes)     | JWT Access token lifetime in seconds.                   |
+| `SECURE_REFRESH_TOKEN_LIFETIME` | `86400` (1 Day)       | JWT Refresh token lifetime in seconds.                  |
+
 
 ### General Configuration
 
 The following settings configure varius aspects of Keystone's backend behavior.
 
 Keystone uses various static files to facilitate operation and support user requests.
 By default, these files are stored in subdirectories of the installed application directory (`<app>`).
```

### Comparing `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.9/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.9/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/authentication/tasks.py` & `keystone_api-0.3.9/keystone_api/apps/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckJsonView.py` & `keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckJsonView.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckPrometheusView.py` & `keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckPrometheusView.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/health/tests/views/test_HealthCheckView.py` & `keystone_api-0.3.9/keystone_api/apps/health/tests/views/test_HealthCheckView.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/health/tests/views/utils.py` & `keystone_api-0.3.9/keystone_api/apps/health/tests/views/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/health/views.py` & `keystone_api-0.3.9/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/admin.py` & `keystone_api-0.3.9/keystone_api/apps/logging/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.9/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.9/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.9/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py` & `keystone_api-0.3.9/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/migrations/0003_taskresult.py` & `keystone_api-0.3.9/keystone_api/apps/logging/migrations/0003_taskresult.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/models.py` & `keystone_api-0.3.9/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.9/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.9/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/tests/handlers/test_DBHandler.py` & `keystone_api-0.3.9/keystone_api/apps/logging/tests/handlers/test_DBHandler.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py` & `keystone_api-0.3.9/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py` & `keystone_api-0.3.9/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/logging/views.py` & `keystone_api-0.3.9/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/managers.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/permissions.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.9/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.9/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/scheduler/apps.py` & `keystone_api-0.3.9/keystone_api/apps/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.9/keystone_api/apps/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/scheduler/checks.py` & `keystone_api-0.3.9/keystone_api/apps/scheduler/checks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/admin.py` & `keystone_api-0.3.9/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.9/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/managers.py` & `keystone_api-0.3.9/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.9/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/models.py` & `keystone_api-0.3.9/keystone_api/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.9/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.9/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.9/keystone_api/apps/users/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.9/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.9/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.9/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.9/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/apps/users/views.py` & `keystone_api-0.3.9/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/main/settings.py` & `keystone_api-0.3.9/keystone_api/main/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -225,14 +225,19 @@
 AUTH_PASSWORD_VALIDATORS = [
     {'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator'},
     {'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator'},
     {'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator'},
     {'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator'},
 ]
 
+SIMPLE_JWT = {
+    'ACCESS_TOKEN_LIFETIME': timedelta(seconds=env.int('SECURE_ACCESS_TOKEN_LIFETIME', 5 * 60)),
+    'REFRESH_TOKEN_LIFETIME': timedelta(seconds=env.int('SECURE_REFRESH_TOKEN_LIFETIME', 24 * 60 * 60))
+}
+
 # Static file handling (CSS, JavaScript, Images)
 
 STATIC_URL = 'static/'
 STATIC_ROOT = Path(env.path('CONFIG_STATIC_DIR', BASE_DIR / 'static_files'))
 STATIC_ROOT.mkdir(parents=True, exist_ok=True)
 
 MEDIA_URL = 'uploads/'
```

### Comparing `keystone_api-0.3.8/keystone_api/main/urls.py` & `keystone_api-0.3.9/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/manage.py` & `keystone_api-0.3.9/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/plugins/slurm.py` & `keystone_api-0.3.9/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.9/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.9/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/health/test.py` & `keystone_api-0.3.9/keystone_api/tests/health/test.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/health/test_json.py` & `keystone_api-0.3.9/keystone_api/tests/health/test_json.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/health/test_prom.py` & `keystone_api-0.3.9/keystone_api/tests/health/test_prom.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.9/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.9/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/logging/test_tasks.py` & `keystone_api-0.3.9/keystone_api/tests/logging/test_tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/openapi/test_json.py` & `keystone_api-0.3.9/keystone_api/tests/openapi/test_json.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/openapi/test_yaml.py` & `keystone_api-0.3.9/keystone_api/tests/openapi/test_yaml.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/research/test_grants.py` & `keystone_api-0.3.9/keystone_api/tests/research/test_grants.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/research/test_grants_pk.py` & `keystone_api-0.3.9/keystone_api/tests/research/test_grants_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/research/test_publications.py` & `keystone_api-0.3.9/keystone_api/tests/research/test_publications.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/research/test_publications_pk.py` & `keystone_api-0.3.9/keystone_api/tests/research/test_publications_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.9/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.9/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.9/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.9/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/keystone_api/tests/utils.py` & `keystone_api-0.3.9/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.8/pyproject.toml` & `keystone_api-0.3.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.8"
+version = "0.3.9"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
```

### Comparing `keystone_api-0.3.8/PKG-INFO` & `keystone_api-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.8
+Version: 0.3.9
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -135,24 +135,27 @@
 - Avoid issuing session/CSRF tokens over unsecured connections by enabling `SECURE_SESSION_TOKENS`
 - Always use a secure `SECURE_SECRET_KEY` value to ensure proper request signing across application instances/restarts
 - Consider using HTTP Strict Transport Security (HSTS) to enforce the use of HTTPS
 
 The `SECURE_SECRET_KEY` value may be changed at any given time. However, doing so may invalidate any active user
 sessions and require users to reauthenticate.
 
-| Setting Name              | Default Value            | Description                                                   |
-|---------------------------|--------------------------|---------------------------------------------------------------|
-| `SECURE_SECRET_KEY`       | Randomly generated       | Secret key used to enforce cryptographic signing.             |
-| `SECURE_ALLOWED_HOSTS`    | `localhost,127.0.0.1`    | Comma-separated list of accepted host/domain names.           |
-| `SECURE_SSL_REDIRECT`     | `False`                  | Automatically redirect all HTTP traffic to HTTPS.             |
-| `SECURE_SESSION_TOKENS`   | `False`                  | Only issue session/CSRF tokens over secure connections.       |
-| `SECURE_CSRF_ORIGINS`     | `[]`                     | Domains (with protocol) to accept CSRF headers from.          |
-| `SECURE_HSTS_SECONDS`     | `0` (Disabled)           | HSTS cache duration in seconds.                               |
-| `SECURE_HSTS_SUBDOMAINS`  | `False`                  | Enable HSTS for subdomains.                                   |
-| `SECURE_HSTS_PRELOAD`     | `False`                  | Enable HSTS preload functionality.                            |
+| Setting Name                    | Default Value         | Description                                             |
+|---------------------------------|-----------------------|---------------------------------------------------------|
+| `SECURE_SECRET_KEY`             | Randomly generated    | Secret key used to enforce cryptographic signing.       |
+| `SECURE_ALLOWED_HOSTS`          | `localhost,127.0.0.1` | Comma-separated list of accepted host/domain names.     |
+| `SECURE_SSL_REDIRECT`           | `False`               | Automatically redirect all HTTP traffic to HTTPS.       |
+| `SECURE_SESSION_TOKENS`         | `False`               | Only issue session/CSRF tokens over secure connections. |
+| `SECURE_CSRF_ORIGINS`           | `[]`                  | Domains (with protocol) to accept CSRF headers from.    |
+| `SECURE_HSTS_SECONDS`           | `0` (Disabled)        | HSTS cache duration in seconds.                         |
+| `SECURE_HSTS_SUBDOMAINS`        | `False`               | Enable HSTS for subdomains.                             |
+| `SECURE_HSTS_PRELOAD`           | `False`               | Enable HSTS preload functionality.                      |
+| `SECURE_ACCESS_TOKEN_LIFETIME`  | `300` (5 Minutes)     | JWT Access token lifetime in seconds.                   |
+| `SECURE_REFRESH_TOKEN_LIFETIME` | `86400` (1 Day)       | JWT Refresh token lifetime in seconds.                  |
+
 
 ### General Configuration
 
 The following settings configure varius aspects of Keystone's backend behavior.
 
 Keystone uses various static files to facilitate operation and support user requests.
 By default, these files are stored in subdirectories of the installed application directory (`<app>`).
```

