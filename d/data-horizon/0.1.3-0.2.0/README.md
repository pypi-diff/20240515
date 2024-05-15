# Comparing `tmp/data_horizon-0.1.3.tar.gz` & `tmp/data_horizon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_horizon-0.1.3.tar", max compression
+gzip compressed data, was "data_horizon-0.2.0.tar", max compression
```

## Comparing `data_horizon-0.1.3.tar` & `data_horizon-0.2.0.tar`

### file list

```diff
@@ -1,145 +1,144 @@
--rw-r--r--   0        0        0    11426 2024-05-02 10:58:16.721839 data_horizon-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2843 2024-05-02 10:58:46.689953 data_horizon-0.1.3/README.rst
--rw-r--r--   0        0        0      530 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/__init__.py
--rw-r--r--   0        0        0     2540 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/__init__.py
--rwxr-xr-x   0        0        0      815 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/__main__.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/__init__.py
--rw-r--r--   0        0        0     4168 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/handlers.py
--rw-r--r--   0        0        0      362 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/monitoring.py
--rw-r--r--   0        0        0      372 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/router.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/__init__.py
--rw-r--r--   0        0        0      997 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/__init__.py
--rw-r--r--   0        0        0     1252 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/auth.py
--rw-r--r--   0        0        0     6454 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/hwm.py
--rw-r--r--   0        0        0      975 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/hwm_history.py
--rw-r--r--   0        0        0     1029 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/namespace_history.py
--rw-r--r--   0        0        0     4226 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/namespaces.py
--rw-r--r--   0        0        0     3650 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/permission.py
--rw-r--r--   0        0        0      854 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/users.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/__init__.py
--rw-r--r--   0        0        0      669 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/factory.py
--rw-r--r--   0        0        0       58 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/README
--rwxr-xr-x   0        0        0      868 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/__main__.py
--rw-r--r--   0        0        0      673 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/alembic.ini
--rw-r--r--   0        0        0     2360 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/env.py
--rw-r--r--   0        0        0      510 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/.keep
--rw-r--r--   0        0        0     1498 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
--rw-r--r--   0        0        0     1723 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
--rw-r--r--   0        0        0     2283 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
--rw-r--r--   0        0        0     2302 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
--rw-r--r--   0        0        0     1684 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
--rw-r--r--   0        0        0     1375 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
--rw-r--r--   0        0        0     1877 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
--rw-r--r--   0        0        0      670 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
--rw-r--r--   0        0        0     2345 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
--rw-r--r--   0        0        0     1799 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
--rw-r--r--   0        0        0     2564 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
--rw-r--r--   0        0        0      599 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/__init__.py
--rw-r--r--   0        0        0     1091 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/changed_by.py
--rw-r--r--   0        0        0      634 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/timestamp.py
--rw-r--r--   0        0        0      595 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/__init__.py
--rw-r--r--   0        0        0     1044 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/base.py
--rw-r--r--   0        0        0     1112 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/credentials_cache.py
--rw-r--r--   0        0        0     1380 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/hwm.py
--rw-r--r--   0        0        0     1266 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/hwm_history.py
--rw-r--r--   0        0        0     1223 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace.py
--rw-r--r--   0        0        0     1174 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace_history.py
--rw-r--r--   0        0        0      723 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace_user.py
--rw-r--r--   0        0        0      758 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/user.py
--rw-r--r--   0        0        0      554 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/__init__.py
--rw-r--r--   0        0        0     3797 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/base.py
--rw-r--r--   0        0        0      915 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/credentials_cache.py
--rw-r--r--   0        0        0     5178 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/hwm.py
--rw-r--r--   0        0        0     1312 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/hwm_history.py
--rw-r--r--   0        0        0     6275 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/namespace.py
--rw-r--r--   0        0        0     1102 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/namespace_history.py
--rw-r--r--   0        0        0     1509 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/user.py
--rw-r--r--   0        0        0      151 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/dependencies/__init__.py
--rw-r--r--   0        0        0     1636 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/dependencies/stub.py
--rwxr-xr-x   0        0        0      482 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/export_openapi_schema.py
--rw-r--r--   0        0        0     1555 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/__init__.py
--rw-r--r--   0        0        0     1600 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/application_version.py
--rw-r--r--   0        0        0      522 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/cors.py
--rw-r--r--   0        0        0      752 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/logging.py
--rw-r--r--   0        0        0      303 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/__init__.py
--rw-r--r--   0        0        0     1337 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/metrics.py
--rw-r--r--   0        0        0     2912 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/stats.py
--rw-r--r--   0        0        0     4252 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/openapi.py
--rw-r--r--   0        0        0      629 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/request_id.py
--rw-r--r--   0        0        0      633 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/static_files.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/__init__.py
--rw-r--r--   0        0        0      160 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/__init__.py
--rw-r--r--   0        0        0     3119 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/base.py
--rw-r--r--   0        0        0     5817 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/cached_ldap.py
--rw-r--r--   0        0        0     3791 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/dummy.py
--rw-r--r--   0        0        0    10170 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/ldap.py
--rwxr-xr-x   0        0        0     3656 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/scripts/manage_admins.py
--rw-r--r--   0        0        0      215 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/services/__init__.py
--rw-r--r--   0        0        0      654 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/services/current_user.py
--rw-r--r--   0        0        0     1241 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/services/uow.py
--rw-r--r--   0        0        0     2136 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/__init__.py
--rw-r--r--   0        0        0     1078 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/__init__.py
--rw-r--r--   0        0        0     2758 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/cached_ldap.py
--rw-r--r--   0        0        0      567 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/dummy.py
--rw-r--r--   0        0        0     1166 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/jwt.py
--rw-r--r--   0        0        0     7103 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/ldap.py
--rw-r--r--   0        0        0     1133 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/database.py
--rw-r--r--   0        0        0     2678 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/__init__.py
--rw-r--r--   0        0        0      704 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/application_version.py
--rw-r--r--   0        0        0     2102 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/cors.py
--rw-r--r--   0        0        0     2862 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/__init__.py
--rw-r--r--   0        0        0      924 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/colored.yml
--rw-r--r--   0        0        0      867 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/json.yml
--rw-r--r--   0        0        0      909 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/plain.yml
--rw-r--r--   0        0        0     2203 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/monitoring.py
--rw-r--r--   0        0        0     4345 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/openapi.py
--rw-r--r--   0        0        0     1048 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/request_id.py
--rw-r--r--   0        0        0     1025 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/static_files.py
--rw-r--r--   0        0        0        0 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/static/.gitkeep
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/__init__.py
--rw-r--r--   0        0        0      827 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/jwt.py
--rw-r--r--   0        0        0      343 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/slug.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/__init__.py
--rw-r--r--   0        0        0      335 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/__init__.py
--rw-r--r--   0        0        0     1743 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/access_token.py
--rw-r--r--   0        0        0      795 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/base.py
--rw-r--r--   0        0        0     1381 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/login_password.py
--rw-r--r--   0        0        0     6593 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/base.py
--rw-r--r--   0        0        0    34597 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/sync.py
--rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/__init__.py
--rw-r--r--   0        0        0      244 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/__init__.py
--rw-r--r--   0        0        0     1003 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/pagination.py
--rw-r--r--   0        0        0      583 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/unset.py
--rw-r--r--   0        0        0      480 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/__init__.py
--rw-r--r--   0        0        0      860 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/base.py
--rw-r--r--   0        0        0     2261 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/registration.py
--rw-r--r--   0        0        0      730 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/__init__.py
--rw-r--r--   0        0        0      982 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/already_exists.py
--rw-r--r--   0        0        0      525 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/bad_request.py
--rw-r--r--   0        0        0     1200 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/invalid_request.py
--rw-r--r--   0        0        0      753 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/not_authorized.py
--rw-r--r--   0        0        0      939 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/not_found.py
--rw-r--r--   0        0        0      927 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/permission_denied.py
--rw-r--r--   0        0        0      724 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/__init__.py
--rw-r--r--   0        0        0      832 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/auth.py
--rw-r--r--   0        0        0     1016 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/bad_request.py
--rw-r--r--   0        0        0      550 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/base.py
--rw-r--r--   0        0        0     2346 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/entity.py
--rw-r--r--   0        0        0     1300 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/permission.py
--rw-r--r--   0        0        0      760 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/service.py
--rw-r--r--   0        0        0      189 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/__init__.py
--rw-r--r--   0        0        0      293 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/ping.py
--rw-r--r--   0        0        0     1929 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/__init__.py
--rw-r--r--   0        0        0      305 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/auth.py
--rw-r--r--   0        0        0     4589 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/hwm.py
--rw-r--r--   0        0        0     1700 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/hwm_history.py
--rw-r--r--   0        0        0     2358 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/namespace.py
--rw-r--r--   0        0        0     1371 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/namespace_history.py
--rw-r--r--   0        0        0     2174 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/pagination.py
--rw-r--r--   0        0        0     2209 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/permission.py
--rw-r--r--   0        0        0      770 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/user.py
--rw-r--r--   0        0        0        0 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/py.typed
--rw-r--r--   0        0        0    15137 2024-05-02 10:58:16.737839 data_horizon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7390 1970-01-01 00:00:00.000000 data_horizon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11426 2024-05-15 08:55:17.089771 data_horizon-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2843 2024-05-15 08:55:47.225989 data_horizon-0.2.0/README.rst
+-rw-r--r--   0        0        0      530 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/__init__.py
+-rw-r--r--   0        0        0     2540 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/backend/__init__.py
+-rwxr-xr-x   0        0        0      815 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/backend/__main__.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/backend/api/__init__.py
+-rw-r--r--   0        0        0     4214 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/backend/api/handlers.py
+-rw-r--r--   0        0        0      362 2024-05-15 08:55:17.093771 data_horizon-0.2.0/horizon/backend/api/monitoring.py
+-rw-r--r--   0        0        0      372 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/router.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/auth.py
+-rw-r--r--   0        0        0     6454 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/hwm.py
+-rw-r--r--   0        0        0      975 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/hwm_history.py
+-rw-r--r--   0        0        0     1029 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/namespace_history.py
+-rw-r--r--   0        0        0     7375 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/namespaces.py
+-rw-r--r--   0        0        0      854 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/api/v1/router/users.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/factory.py
+-rw-r--r--   0        0        0       58 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/README
+-rwxr-xr-x   0        0        0      868 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/__main__.py
+-rw-r--r--   0        0        0      673 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/alembic.ini
+-rw-r--r--   0        0        0     2360 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/env.py
+-rw-r--r--   0        0        0      510 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/.keep
+-rw-r--r--   0        0        0     1498 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
+-rw-r--r--   0        0        0     1723 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
+-rw-r--r--   0        0        0     2283 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
+-rw-r--r--   0        0        0     2302 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
+-rw-r--r--   0        0        0     1684 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
+-rw-r--r--   0        0        0     1375 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
+-rw-r--r--   0        0        0     1877 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
+-rw-r--r--   0        0        0      670 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
+-rw-r--r--   0        0        0     2345 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
+-rw-r--r--   0        0        0     1799 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
+-rw-r--r--   0        0        0     2564 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
+-rw-r--r--   0        0        0      599 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/mixins/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/mixins/changed_by.py
+-rw-r--r--   0        0        0      634 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/mixins/timestamp.py
+-rw-r--r--   0        0        0      595 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/__init__.py
+-rw-r--r--   0        0        0     1044 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/base.py
+-rw-r--r--   0        0        0     1112 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/credentials_cache.py
+-rw-r--r--   0        0        0     1380 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/hwm.py
+-rw-r--r--   0        0        0     1266 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/hwm_history.py
+-rw-r--r--   0        0        0     1223 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/namespace.py
+-rw-r--r--   0        0        0     1174 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/namespace_history.py
+-rw-r--r--   0        0        0      723 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/namespace_user.py
+-rw-r--r--   0        0        0      758 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/models/user.py
+-rw-r--r--   0        0        0      554 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/__init__.py
+-rw-r--r--   0        0        0     3797 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/base.py
+-rw-r--r--   0        0        0      915 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/credentials_cache.py
+-rw-r--r--   0        0        0     5178 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/hwm.py
+-rw-r--r--   0        0        0     1312 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/hwm_history.py
+-rw-r--r--   0        0        0     6275 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/namespace.py
+-rw-r--r--   0        0        0     1102 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/namespace_history.py
+-rw-r--r--   0        0        0     1509 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/db/repositories/user.py
+-rw-r--r--   0        0        0      151 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/dependencies/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/dependencies/stub.py
+-rwxr-xr-x   0        0        0      482 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/export_openapi_schema.py
+-rw-r--r--   0        0        0     1555 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/application_version.py
+-rw-r--r--   0        0        0      522 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/cors.py
+-rw-r--r--   0        0        0      752 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/logging.py
+-rw-r--r--   0        0        0      303 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/monitoring/__init__.py
+-rw-r--r--   0        0        0     1337 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/monitoring/metrics.py
+-rw-r--r--   0        0        0     2912 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/monitoring/stats.py
+-rw-r--r--   0        0        0     4252 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/openapi.py
+-rw-r--r--   0        0        0      629 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/request_id.py
+-rw-r--r--   0        0        0      633 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/middlewares/static_files.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/auth/__init__.py
+-rw-r--r--   0        0        0     3119 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/auth/base.py
+-rw-r--r--   0        0        0     5817 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/auth/cached_ldap.py
+-rw-r--r--   0        0        0     3791 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/auth/dummy.py
+-rw-r--r--   0        0        0    10441 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/providers/auth/ldap.py
+-rwxr-xr-x   0        0        0     3656 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/scripts/manage_admins.py
+-rw-r--r--   0        0        0      215 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/services/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/services/current_user.py
+-rw-r--r--   0        0        0     1241 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/services/uow.py
+-rw-r--r--   0        0        0     2136 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/__init__.py
+-rw-r--r--   0        0        0     1078 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/auth/__init__.py
+-rw-r--r--   0        0        0     2758 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/auth/cached_ldap.py
+-rw-r--r--   0        0        0      567 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/auth/dummy.py
+-rw-r--r--   0        0        0     1166 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/auth/jwt.py
+-rw-r--r--   0        0        0     7103 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/auth/ldap.py
+-rw-r--r--   0        0        0     1133 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/database.py
+-rw-r--r--   0        0        0     2678 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/application_version.py
+-rw-r--r--   0        0        0     2102 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/cors.py
+-rw-r--r--   0        0        0     2862 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/log/__init__.py
+-rw-r--r--   0        0        0      952 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/log/colored.yml
+-rw-r--r--   0        0        0      921 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/log/json.yml
+-rw-r--r--   0        0        0      937 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/log/plain.yml
+-rw-r--r--   0        0        0     2205 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/monitoring.py
+-rw-r--r--   0        0        0     4345 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/openapi.py
+-rw-r--r--   0        0        0     1048 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/request_id.py
+-rw-r--r--   0        0        0     1025 2024-05-15 08:55:17.097771 data_horizon-0.2.0/horizon/backend/settings/server/static_files.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/backend/static/.gitkeep
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/backend/utils/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/backend/utils/jwt.py
+-rw-r--r--   0        0        0      343 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/backend/utils/slug.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/auth/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/auth/access_token.py
+-rw-r--r--   0        0        0      795 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/auth/base.py
+-rw-r--r--   0        0        0     1381 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/auth/login_password.py
+-rw-r--r--   0        0        0     6593 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/base.py
+-rw-r--r--   0        0        0    34600 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/client/sync.py
+-rw-r--r--   0        0        0       99 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/dto/__init__.py
+-rw-r--r--   0        0        0     1003 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/dto/pagination.py
+-rw-r--r--   0        0        0      583 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/dto/unset.py
+-rw-r--r--   0        0        0      480 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/__init__.py
+-rw-r--r--   0        0        0      860 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/base.py
+-rw-r--r--   0        0        0     2261 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/registration.py
+-rw-r--r--   0        0        0      730 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/__init__.py
+-rw-r--r--   0        0        0      982 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/already_exists.py
+-rw-r--r--   0        0        0      525 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/bad_request.py
+-rw-r--r--   0        0        0     1219 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/invalid_request.py
+-rw-r--r--   0        0        0      753 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/not_authorized.py
+-rw-r--r--   0        0        0      939 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/not_found.py
+-rw-r--r--   0        0        0      927 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/errors/schemas/permission_denied.py
+-rw-r--r--   0        0        0      724 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/auth.py
+-rw-r--r--   0        0        0     1016 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/bad_request.py
+-rw-r--r--   0        0        0      550 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/base.py
+-rw-r--r--   0        0        0     2346 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/entity.py
+-rw-r--r--   0        0        0     1300 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/permission.py
+-rw-r--r--   0        0        0      760 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/exceptions/service.py
+-rw-r--r--   0        0        0      189 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/ping.py
+-rw-r--r--   0        0        0     1929 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/auth.py
+-rw-r--r--   0        0        0     4589 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/hwm.py
+-rw-r--r--   0        0        0     1700 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/hwm_history.py
+-rw-r--r--   0        0        0     2358 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/namespace.py
+-rw-r--r--   0        0        0     1371 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/namespace_history.py
+-rw-r--r--   0        0        0     2174 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/pagination.py
+-rw-r--r--   0        0        0     2209 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/permission.py
+-rw-r--r--   0        0        0      770 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/commons/schemas/v1/user.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:55:17.101771 data_horizon-0.2.0/horizon/py.typed
+-rw-r--r--   0        0        0    15137 2024-05-15 08:55:17.101771 data_horizon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7390 1970-01-01 00:00:00.000000 data_horizon-0.2.0/PKG-INFO
```

### Comparing `data_horizon-0.1.3/LICENSE.txt` & `data_horizon-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/README.rst` & `data_horizon-0.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/9dfa8bf2b8acf18c1ba8e78f0b48e868a59694fe/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/c4a529ab582c522ca5ea9003c089902c39be5cf4/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
```

### Comparing `data_horizon-0.1.3/horizon/__init__.py` & `data_horizon-0.2.0/horizon/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 # _raw_version could contain pre-release version, like 0.0.1dev123
 # value is updated automatically by `poetry version ...` and poetry-bumpversion plugin
-_raw_version = "0.1.3"
+_raw_version = "0.2.0"
 
 # version always contain only release number like 0.0.1
 __version__ = ".".join(_raw_version.split(".")[:3])  # noqa: WPS410
 
 # version tuple always contains only integer parts, like (0, 0, 1)
 __version_tuple__ = tuple(map(int, __version__.split(".")))
```

### Comparing `data_horizon-0.1.3/horizon/backend/__init__.py` & `data_horizon-0.2.0/horizon/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/__main__.py` & `data_horizon-0.2.0/horizon/backend/__main__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/api/handlers.py` & `data_horizon-0.2.0/horizon/backend/api/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         status=exc.status_code,
         content=content,
         headers=exc.headers,
     )
 
 
 def unknown_exception_handler(request: Request, exc: Exception) -> Response:
-    logger.exception("Got unhandled error")
+    logger.exception("Got unhandled error: %s", exc, exc_info=exc)
 
     server: ServerSettings = request.app.state.settings.server
     details = None
     if request.app.debug:
         details = exc.args
 
     content = BaseErrorSchema(
@@ -49,15 +49,15 @@
         content=content,
         # https://github.com/snok/asgi-correlation-id#exception-handling
         headers={server.request_id.header_name: correlation_id.get() or ""},
     )
 
 
 def service_exception_handler(request: Request, exc: ServiceError) -> Response:
-    logger.exception("Got service error")
+    logger.exception("Got service error: %s", exc, exc_info=exc)
 
     server: ServerSettings = request.app.state.settings.server
     details = None
     if request.app.debug:
         details = exc.message
 
     content = BaseErrorSchema(
```

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/__init__.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from horizon.backend.api.v1.router.auth import router as auth_router
 from horizon.backend.api.v1.router.hwm import router as hwm_router
 from horizon.backend.api.v1.router.hwm_history import router as hwm_history_router
 from horizon.backend.api.v1.router.namespace_history import (
     router as namespace_history_router,
 )
 from horizon.backend.api.v1.router.namespaces import router as namespaces_router
-from horizon.backend.api.v1.router.permission import router as permission_router
 from horizon.backend.api.v1.router.users import router as users_router
 
 router = APIRouter(prefix="/v1")
 router.include_router(auth_router)
 router.include_router(users_router)
 router.include_router(namespaces_router)
 router.include_router(hwm_router)
 router.include_router(hwm_history_router)
 router.include_router(namespace_history_router)
-router.include_router(permission_router)
```

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/auth.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/hwm.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/hwm_history.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/namespace_history.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/api/v1/router/users.py` & `data_horizon-0.2.0/horizon/backend/api/v1/router/users.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/factory.py` & `data_horizon-0.2.0/horizon/backend/db/factory.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/__main__.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/__main__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/alembic.ini` & `data_horizon-0.2.0/horizon/backend/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/env.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py` & `data_horizon-0.2.0/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/mixins/changed_by.py` & `data_horizon-0.2.0/horizon/backend/db/mixins/changed_by.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/mixins/timestamp.py` & `data_horizon-0.2.0/horizon/backend/db/mixins/timestamp.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/__init__.py` & `data_horizon-0.2.0/horizon/backend/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/base.py` & `data_horizon-0.2.0/horizon/backend/db/models/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/credentials_cache.py` & `data_horizon-0.2.0/horizon/backend/db/models/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/hwm.py` & `data_horizon-0.2.0/horizon/backend/db/models/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/hwm_history.py` & `data_horizon-0.2.0/horizon/backend/db/models/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/namespace.py` & `data_horizon-0.2.0/horizon/backend/db/models/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/namespace_history.py` & `data_horizon-0.2.0/horizon/backend/db/models/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/namespace_user.py` & `data_horizon-0.2.0/horizon/backend/db/models/namespace_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/models/user.py` & `data_horizon-0.2.0/horizon/backend/db/models/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/__init__.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/base.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/credentials_cache.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/hwm.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/hwm_history.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/namespace.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/namespace_history.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/db/repositories/user.py` & `data_horizon-0.2.0/horizon/backend/db/repositories/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/dependencies/stub.py` & `data_horizon-0.2.0/horizon/backend/dependencies/stub.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/__init__.py` & `data_horizon-0.2.0/horizon/backend/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/application_version.py` & `data_horizon-0.2.0/horizon/backend/middlewares/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/cors.py` & `data_horizon-0.2.0/horizon/backend/middlewares/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/logging.py` & `data_horizon-0.2.0/horizon/backend/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/monitoring/metrics.py` & `data_horizon-0.2.0/horizon/backend/middlewares/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/monitoring/stats.py` & `data_horizon-0.2.0/horizon/backend/middlewares/monitoring/stats.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/openapi.py` & `data_horizon-0.2.0/horizon/backend/middlewares/openapi.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/request_id.py` & `data_horizon-0.2.0/horizon/backend/middlewares/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/middlewares/static_files.py` & `data_horizon-0.2.0/horizon/backend/middlewares/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/providers/auth/base.py` & `data_horizon-0.2.0/horizon/backend/providers/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/providers/auth/cached_ldap.py` & `data_horizon-0.2.0/horizon/backend/providers/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/providers/auth/dummy.py` & `data_horizon-0.2.0/horizon/backend/providers/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/providers/auth/ldap.py` & `data_horizon-0.2.0/horizon/backend/providers/auth/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Similar to:
 * `JupyterHub LDAPAuthenticator <https://github.com/jupyterhub/ldapauthenticator>`_
 * `Flask-AppBuilder LDAP integration <https://github.com/dpgaspar/Flask-AppBuilder/blob/master/docs/config.rst>`_, used in Apache Airflow
 """
 
 import logging
+from asyncio import TimeoutError
 from contextlib import asynccontextmanager
 from time import time
 from typing import Any, AsyncContextManager, AsyncGenerator, Dict, List, Optional, Tuple
 
 from bonsai import InvalidDN, LDAPClient
 from bonsai.asyncio import AIOConnectionPool, AIOLDAPConnection
 from bonsai.errors import AuthenticationError, LDAPError
@@ -33,14 +34,16 @@
     AuthorizationError,
     EntityNotFoundError,
     ServiceError,
 )
 
 log = logging.getLogger(__name__)
 
+LDAPUnrecoverableError = (LDAPError, TimeoutError)
+
 
 class LDAPAuthProvider(AuthProvider):
     def __init__(
         self,
         auth_settings: Annotated[LDAPAuthProviderSettings, Depends(Stub(LDAPAuthProviderSettings))],
         pool: Annotated[Optional[AIOConnectionPool], Depends(Stub(AIOConnectionPool))],
         unit_of_work: Annotated[UnitOfWork, Depends()],
@@ -132,14 +135,15 @@
             return None
 
         log.debug("Lookup enabled, creating connection pool")
         return AIOConnectionPool(
             client,
             minconn=settings.ldap.lookup.pool.initial,
             maxconn=settings.ldap.lookup.pool.max,
+            timeout=settings.ldap.timeout_seconds,
         )
 
     @asynccontextmanager
     async def _get_lookup_connection(self) -> AsyncGenerator[AIOLDAPConnection, None]:
         """Create connection used for lookup queries"""
         try:
             connect: AsyncContextManager[AIOLDAPConnection]
@@ -151,20 +155,21 @@
                 log.debug("Creating non-pooled connection for lookup")
                 client = self._get_lookup_client(self._auth_settings)
                 connect = client.connect(is_async=True, timeout=self._auth_settings.ldap.timeout_seconds)
 
             async with connect as connection:
                 try:  # noqa: WPS505
                     yield connection
-                except LDAPError:
+                except LDAPUnrecoverableError:
                     # avoid returning connection back to the pool
+                    # https://bonsai.readthedocs.io/en/latest/advanced.html#connection-timeouts
                     connection.close()
                     raise
 
-        except LDAPError as e:
+        except LDAPUnrecoverableError as e:
             raise ServiceError("Failed to connect to LDAP") from e
 
     async def _resolve_username_from_ldap(self, login: str, password: str) -> str:
         log.info("Resolve user %r in LDAP", login)
         username = login
 
         if self._auth_settings.ldap.lookup.enabled:
@@ -220,15 +225,15 @@
         client.set_credentials(self._auth_settings.ldap.auth_mechanism, login, password)
         try:
             connection = client.connect(is_async=True, timeout=self._auth_settings.ldap.timeout_seconds)
             async with connection:
                 await connection.whoami()
         except (AuthenticationError, InvalidDN) as e:
             raise AuthorizationError("Wrong credentials") from e
-        except LDAPError as e:
+        except LDAPUnrecoverableError as e:
             raise ServiceError("Failed to connect to LDAP") from e
 
     def _generate_access_token(self, user: User) -> Tuple[str, float]:
         expires_at = time() + self._auth_settings.access_token.expire_seconds
         payload = {
             "user_id": user.id,
             "exp": expires_at,
```

### Comparing `data_horizon-0.1.3/horizon/backend/scripts/manage_admins.py` & `data_horizon-0.2.0/horizon/backend/scripts/manage_admins.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/services/current_user.py` & `data_horizon-0.2.0/horizon/backend/services/current_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/services/uow.py` & `data_horizon-0.2.0/horizon/backend/services/uow.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/__init__.py` & `data_horizon-0.2.0/horizon/backend/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/auth/__init__.py` & `data_horizon-0.2.0/horizon/backend/settings/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/auth/cached_ldap.py` & `data_horizon-0.2.0/horizon/backend/settings/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/auth/dummy.py` & `data_horizon-0.2.0/horizon/backend/settings/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/auth/jwt.py` & `data_horizon-0.2.0/horizon/backend/settings/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/auth/ldap.py` & `data_horizon-0.2.0/horizon/backend/settings/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/database.py` & `data_horizon-0.2.0/horizon/backend/settings/database.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/__init__.py` & `data_horizon-0.2.0/horizon/backend/settings/server/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/application_version.py` & `data_horizon-0.2.0/horizon/backend/settings/server/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/cors.py` & `data_horizon-0.2.0/horizon/backend/settings/server/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/log/__init__.py` & `data_horizon-0.2.0/horizon/backend/settings/server/log/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/log/colored.yml` & `data_horizon-0.2.0/horizon/backend/settings/server/log/colored.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     uuid_length: 32
     default_value: '-'
 
 formatters:
   colored:
     (): coloredlogs.ColoredFormatter
     # Add correlation_id to log records
-    fmt: '%(asctime)s.%(msecs)03d %(name)s:%(lineno)d [%(levelname)s] %(correlation_id)s %(message)s'
+    fmt: '%(asctime)s.%(msecs)03d %(processName)s:%(process)d %(name)s:%(lineno)d [%(levelname)s] %(correlation_id)s %(message)s'
     datefmt: '%Y-%m-%d %H:%M:%S'
 
 handlers:
   main:
     class: logging.StreamHandler
     formatter: colored
     filters: [correlation_id]
```

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/log/json.yml` & `data_horizon-0.2.0/horizon/backend/settings/server/log/plain.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+# development usage only
 version: 1
 disable_existing_loggers: false
 
 filters:
   # Add request ID as extra field named `correlation_id` to each log record.
   # This is used in combination with settings.server.request_id.enabled=True
   # See https://github.com/snok/asgi-correlation-id#configure-logging
   correlation_id:
     (): asgi_correlation_id.CorrelationIdFilter
     uuid_length: 32
     default_value: '-'
 
 formatters:
-  json:
-    (): pythonjsonlogger.jsonlogger.JsonFormatter
+  plain:
+    (): logging.Formatter
     # Add correlation_id to log records
-    fmt: '%(name)s %(lineno)d %(levelname)s %(message)s %(correlation_id)s'
-    timestamp: true
+    fmt: '%(asctime)s.%(msecs)03d %(processName)s:%(process)d %(name)s:%(lineno)d [%(levelname)s] %(correlation_id)s %(message)s'
+    datefmt: '%Y-%m-%d %H:%M:%S'
 
 handlers:
   main:
     class: logging.StreamHandler
-    formatter: json
+    formatter: plain
     filters: [correlation_id]
     stream: ext://sys.stdout
 
 loggers:
   '':
     handlers: [main]
     level: INFO
```

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/log/plain.yml` & `data_horizon-0.2.0/horizon/backend/settings/server/log/json.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# development usage only
 version: 1
 disable_existing_loggers: false
 
 filters:
   # Add request ID as extra field named `correlation_id` to each log record.
   # This is used in combination with settings.server.request_id.enabled=True
   # See https://github.com/snok/asgi-correlation-id#configure-logging
   correlation_id:
     (): asgi_correlation_id.CorrelationIdFilter
     uuid_length: 32
     default_value: '-'
 
 formatters:
-  plain:
-    (): logging.Formatter
+  json:
+    (): pythonjsonlogger.jsonlogger.JsonFormatter
     # Add correlation_id to log records
-    fmt: '%(asctime)s.%(msecs)03d %(name)s:%(lineno)d [%(levelname)s] %(correlation_id)s %(message)s'
-    datefmt: '%Y-%m-%d %H:%M:%S'
+    fmt: '%(processName)s %(process)d %(threadName)s %(thread)d %(name)s %(lineno)d %(levelname)s %(message)s %(correlation_id)s'
+    timestamp: true
 
 handlers:
   main:
     class: logging.StreamHandler
-    formatter: plain
+    formatter: json
     filters: [correlation_id]
     stream: ext://sys.stdout
 
 loggers:
   '':
     handlers: [main]
     level: INFO
```

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/monitoring.py` & `data_horizon-0.2.0/horizon/backend/settings/server/monitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     # These will be new defaults in starlette-exporter 0.18:
     # https://github.com/stephenhillier/starlette_exporter/issues/79
     group_paths: bool = Field(
         default=True,
         description=textwrap.dedent(
             """
             If ``True`` (recommended), add request path to metrics literally as described
-            in OpenAPI schema, e.g. ``/namespace/{id}``, without substitution with path real values.
+            in OpenAPI schema, e.g. ``/namespaces/{id}``, without substitution with path real values.
 
-            If ``False``, all real request paths to metrics, e.g. ``/namespace/123``.
+            If ``False``, all real request paths to metrics, e.g. ``/namespaces/123``.
             """,
         ),
     )
     filter_unhandled_paths: bool = Field(
         default=True,
         description=textwrap.dedent(
             """
```

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/openapi.py` & `data_horizon-0.2.0/horizon/backend/settings/server/openapi.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/request_id.py` & `data_horizon-0.2.0/horizon/backend/settings/server/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/settings/server/static_files.py` & `data_horizon-0.2.0/horizon/backend/settings/server/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/backend/utils/jwt.py` & `data_horizon-0.2.0/horizon/backend/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/client/auth/access_token.py` & `data_horizon-0.2.0/horizon/client/auth/access_token.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/client/auth/base.py` & `data_horizon-0.2.0/horizon/client/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/client/auth/login_password.py` & `data_horizon-0.2.0/horizon/client/auth/login_password.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/client/base.py` & `data_horizon-0.2.0/horizon/client/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/client/sync.py` & `data_horizon-0.2.0/horizon/client/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -862,15 +862,15 @@
         --------
 
         >>> client.get_namespace_permissions(namespace_id=234)
         """
 
         return self._request(  # type: ignore[return-value]
             "GET",
-            f"{self.base_url}/v1/namespace/{namespace_id}/permissions",
+            f"{self.base_url}/v1/namespaces/{namespace_id}/permissions",
             response_class=PermissionsResponseV1,
         )
 
     def update_namespace_permissions(
         self,
         namespace_id: int,
         changes: PermissionsUpdateRequestV1,
@@ -891,15 +891,15 @@
 
         Raises
         ------
         :obj:`EntityNotFoundError <horizon.commons.exceptions.entity.EntityNotFoundError>`
             Namespace or provided user not found.
         :obj:`PermissionDeniedError <horizon.commons.exceptions.permission.PermissionDeniedError>`
             Permission denied for performing the requested action.
-        :obj:`BadRequestError <horizon.commons.exceptions.permission.BadRequestError>`
+        :obj:`BadRequestError <horizon.commons.exceptions.bad_request.BadRequestError>`
             Bad request with incorrect operating logic.
 
         Examples
         --------
 
         >>> from horizon.commons.schemas.v1 import PermissionsUpdateRequestV1, PermissionUpdateRequestItemV1
         >>> to_update = PermissionsUpdateRequestV1([
@@ -907,15 +907,15 @@
         ...     PermissionUpdateRequestItemV1(username="add_developer", role="DEVELOPER"),
         ...     PermissionUpdateRequestItemV1(username="make_read_only", role=None),
         ... ])
         >>> client.update_namespace_permissions(namespace_id=234, changes=to_update)
         """
         return self._request(  # type: ignore[return-value]
             "PATCH",
-            f"{self.base_url}/v1/namespace/{namespace_id}/permissions",
+            f"{self.base_url}/v1/namespaces/{namespace_id}/permissions",
             json=changes.dict(exclude_unset=True),
             response_class=PermissionsResponseV1,
         )
 
     def paginate_hwm_history(
         self,
         query: HWMHistoryPaginateQueryV1,
```

### Comparing `data_horizon-0.1.3/horizon/commons/dto/pagination.py` & `data_horizon-0.2.0/horizon/commons/dto/pagination.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/dto/unset.py` & `data_horizon-0.2.0/horizon/commons/dto/unset.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/base.py` & `data_horizon-0.2.0/horizon/commons/errors/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/registration.py` & `data_horizon-0.2.0/horizon/commons/errors/registration.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/__init__.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/already_exists.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/already_exists.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/bad_request.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/invalid_request.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/invalid_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 import http
-from typing import Any, List
+from typing import Any, List, Union
 
 from pydantic import BaseModel, Field, ValidationError
 from pydantic import __version__ as pydantic_version
 from typing_extensions import Literal
 
 from horizon.commons.errors.base import BaseErrorSchema
 from horizon.commons.errors.registration import register_error_response
 
 
 class InvalidRequestBaseErrorSchema(BaseModel):
-    loc: List[str] = Field(alias="location")
+    loc: List[Union[str, int]] = Field(alias="location")
     msg: str = Field(alias="message")
     type: str = Field(alias="code")
 
     if pydantic_version >= "2":
         ctx: dict = Field(default_factory=dict, alias="context")
         input: Any = Field(default=None)
```

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/not_authorized.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/not_authorized.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/not_found.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/not_found.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/errors/schemas/permission_denied.py` & `data_horizon-0.2.0/horizon/commons/errors/schemas/permission_denied.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/__init__.py` & `data_horizon-0.2.0/horizon/commons/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/auth.py` & `data_horizon-0.2.0/horizon/commons/exceptions/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/bad_request.py` & `data_horizon-0.2.0/horizon/commons/exceptions/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/base.py` & `data_horizon-0.2.0/horizon/commons/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/entity.py` & `data_horizon-0.2.0/horizon/commons/exceptions/entity.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/permission.py` & `data_horizon-0.2.0/horizon/commons/exceptions/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/exceptions/service.py` & `data_horizon-0.2.0/horizon/commons/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/__init__.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/hwm.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/hwm_history.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/namespace.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/namespace_history.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/pagination.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/pagination.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/permission.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/horizon/commons/schemas/v1/user.py` & `data_horizon-0.2.0/horizon/commons/schemas/v1/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.3/pyproject.toml` & `data_horizon-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "data-horizon"
-version = "0.1.3"
+version = "0.2.0"
 license = "Apache-2.0"
 description = "Horizon REST API + client"
 authors = ["DataOps.ETL <onetools@mts.ru>"]
 readme = "README.rst"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Pydantic",
```

### Comparing `data_horizon-0.1.3/PKG-INFO` & `data_horizon-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-horizon
-Version: 0.1.3
+Version: 0.2.0
 Summary: Horizon REST API + client
 License: Apache-2.0
 Keywords: Horizon,REST,API,HWM
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -101,15 +101,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/9dfa8bf2b8acf18c1ba8e78f0b48e868a59694fe/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/c4a529ab582c522ca5ea9003c089902c39be5cf4/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
```

