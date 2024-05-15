# Comparing `tmp/pulumi_ovh-0.43.1.tar.gz` & `tmp/pulumi_ovh-0.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ovh-0.43.1.tar", last modified: Tue Apr 23 11:49:08 2024, max compression
+gzip compressed data, was "pulumi_ovh-0.44.0.tar", last modified: Wed May 15 11:56:39 2024, max compression
```

## Comparing `pulumi_ovh-0.43.1.tar` & `pulumi_ovh-0.44.0.tar`

### file list

```diff
@@ -1,281 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.219506 pulumi_ovh-0.43.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 11:49:08.215506 pulumi_ovh-0.43.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.175506 pulumi_ovh-0.43.1/pulumi_ovh/
--rw-r--r--   0 runner    (1001) docker     (127)    20078 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.175506 pulumi_ovh-0.43.1/pulumi_ovh/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloud/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloud/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.187506 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76758 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    39886 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    63390 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_v_rack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    56647 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    43320 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/network_private.py
--rw-r--r--   0 runner    (1001) docker     (127)    28355 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/network_private_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    91949 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/region_storage_presign.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/workflow_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.195506 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/log_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    35161 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17488 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18400 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.195506 pulumi_ovh-0.43.1/pulumi_ovh/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.195506 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_input_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    45978 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dbaas/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.199506 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/ceph_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_ceph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_nas_ha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_boots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_specifications_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_specifications_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    35590 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33661 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_install_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_reboot_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.199506 pulumi_ovh-0.43.1/pulumi_ovh/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/get_zone_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25381 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_redirection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/get_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/get_vrack_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.203506 pulumi_ovh-0.43.1/pulumi_ovh/hosting/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_user_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42087 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_user_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.203506 pulumi_ovh-0.43.1/pulumi_ovh/iam/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_permissions_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_reference_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_reference_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/get_resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iam/resource_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.207506 pulumi_ovh-0.43.1/pulumi_ovh/ip/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    29412 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/get_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/get_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/ip_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/mitigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/move.py
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/ip/reverse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.207506 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/get_vrack_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    39241 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21453 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/udp_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/vrack_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.211506 pulumi_ovh-0.43.1/pulumi_ovh/me/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_apio_auth2_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_paymentmean_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_paymentmean_credit_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    28876 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    18686 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/me/ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.215506 pulumi_ovh-0.43.1/pulumi_ovh/order/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_options_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/order/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.215506 pulumi_ovh-0.43.1/pulumi_ovh/vps/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/get_vps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/get_vpss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vps/vps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.215506 pulumi_ovh-0.43.1/pulumi_ovh/vrack/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/cloud_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/dedicated_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/dedicated_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/get_vracks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/ip_loadbalancing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/pulumi_ovh/vrack/vrack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:49:08.175506 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 11:49:08.000000 pulumi_ovh-0.43.1/pulumi_ovh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:49:08.219506 pulumi_ovh-0.43.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 11:49:07.000000 pulumi_ovh-0.43.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.916531 pulumi_ovh-0.44.0/pulumi_ovh/
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.916531 pulumi_ovh-0.44.0/pulumi_ovh/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloud/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloud/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.924531 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77073 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62985 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18451 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17591 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_v_rack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56335 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43164 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/network_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/network_private_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92875 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24852 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/region_storage_presign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/workflow_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.932531 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15599 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14741 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22907 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22742 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35005 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17488 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18400 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.932531 pulumi_ovh-0.44.0/pulumi_ovh/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.932531 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_input_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29731 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31132 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45978 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dbaas/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.936531 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/ceph_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_ceph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_nas_ha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_boots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_specifications_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32853 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33193 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_install_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_reboot_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.936531 pulumi_ovh-0.44.0/pulumi_ovh/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/get_zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26230 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_redirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/get_installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/get_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/get_vrack_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.940531 pulumi_ovh-0.44.0/pulumi_ovh/hosting/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_user_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_user_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.940531 pulumi_ovh-0.44.0/pulumi_ovh/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_permissions_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_reference_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_reference_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/get_resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14487 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iam/resource_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.944531 pulumi_ovh-0.44.0/pulumi_ovh/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9804 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/get_firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/get_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19983 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/ip/reverse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.948531 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35629 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/get_vrack_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31735 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23867 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21521 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30675 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27524 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17488 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22213 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21230 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/udp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/vrack_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.948531 pulumi_ovh-0.44.0/pulumi_ovh/me/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_apio_auth2_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_paymentmean_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/get_paymentmean_credit_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18530 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25828 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/me/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/pulumi_ovh/order/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_options_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/order/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/pulumi_ovh/vps/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/get_vps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/get_vpss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19100 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vps/vps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/pulumi_ovh/vrack/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/cloud_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/dedicated_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/dedicated_server_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/get_vracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/ip_loadbalancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24562 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh/vrack/vrack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:56:39.916531 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/pulumi_ovh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:56:39.952531 pulumi_ovh-0.44.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-15 11:56:39.000000 pulumi_ovh-0.44.0/setup.py
```

### Comparing `pulumi_ovh-0.43.1/PKG-INFO` & `pulumi_ovh-0.44.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ovh
-Version: 0.43.1
+Version: 0.44.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.43.1 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.44.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.43.1/README.md` & `pulumi_ovh-0.44.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .get_installation_template import *
 from .get_installation_templates import *
 from .get_server import *
 from .get_servers import *
 from .get_vrack_networks import *
 from .provider import *
 from . import outputs
 
@@ -758,22 +759,14 @@
   "fqn": "pulumi_ovh.me",
   "classes": {
    "ovh:Me/installationTemplatePartitionSchemePartition:InstallationTemplatePartitionSchemePartition": "InstallationTemplatePartitionSchemePartition"
   }
  },
  {
   "pkg": "ovh",
-  "mod": "Me/sshKey",
-  "fqn": "pulumi_ovh.me",
-  "classes": {
-   "ovh:Me/sshKey:SshKey": "SshKey"
-  }
- },
- {
-  "pkg": "ovh",
   "mod": "Vps/vps",
   "fqn": "pulumi_ovh.vps",
   "classes": {
    "ovh:Vps/vps:Vps": "Vps"
   }
  },
  {
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/_utilities.py` & `pulumi_ovh-0.44.0/pulumi_ovh/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloud/get_project.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloud/get_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,22 +204,20 @@
 def get_project(service_name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectResult:
     """
     Get the details of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project = ovh.Cloud.get_project(service_name="XXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -247,21 +245,19 @@
 def get_project_output(service_name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
     Get the details of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project = ovh.Cloud.get_project(service_name="XXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloud/get_projects.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloud/get_projects.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,22 +56,20 @@
 
 def get_projects(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectsResult:
     """
     Get the details of your public cloud projects.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     projects = ovh.Cloud.get_projects()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Cloud/getProjects:getProjects', __args__, opts=opts, typ=GetProjectsResult).value
 
     return AwaitableGetProjectsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -81,17 +79,15 @@
 @_utilities.lift_output_func(get_projects)
 def get_projects_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectsResult]:
     """
     Get the details of your public cloud projects.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     projects = ovh.Cloud.get_projects()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloud/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     'AlertingFormattedMonthlyThresholdArgs',
     'ContainerRegistryPlanArgs',
     'ContainerRegistryPlanFeatureArgs',
     'ContainerRegistryPlanRegistryLimitArgs',
     'DatabaseEndpointArgs',
     'DatabaseIpRestrictionArgs',
     'DatabaseNodeArgs',
+    'GatewayExternalInformationArgs',
+    'GatewayExternalInformationIpArgs',
+    'GatewayInterfaceArgs',
     'KubeCustomizationArgs',
     'KubeCustomizationApiserverArgs',
     'KubeCustomizationApiserverAdmissionpluginArgs',
     'KubeCustomizationKubeProxyArgs',
     'KubeCustomizationKubeProxyIptablesArgs',
     'KubeCustomizationKubeProxyIpvsArgs',
     'KubeKubeconfigAttributeArgs',
@@ -528,14 +531,163 @@
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
 
 @pulumi.input_type
+class GatewayExternalInformationArgs:
+    def __init__(__self__, *,
+                 ips: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationIpArgs']]]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationIpArgs']]] ips: List of external ips of the gateway.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        """
+        if ips is not None:
+            pulumi.set(__self__, "ips", ips)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
+
+    @property
+    @pulumi.getter
+    def ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationIpArgs']]]]:
+        """
+        List of external ips of the gateway.
+        """
+        return pulumi.get(self, "ips")
+
+    @ips.setter
+    def ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationIpArgs']]]]):
+        pulumi.set(self, "ips", value)
+
+    @property
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the private network.
+        """
+        return pulumi.get(self, "network_id")
+
+    @network_id.setter
+    def network_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_id", value)
+
+
+@pulumi.input_type
+class GatewayExternalInformationIpArgs:
+    def __init__(__self__, *,
+                 ip: Optional[pulumi.Input[str]] = None,
+                 subnet_id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] ip: IP of the interface.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
+        """
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if subnet_id is not None:
+            pulumi.set(__self__, "subnet_id", subnet_id)
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        IP of the interface.
+        """
+        return pulumi.get(self, "ip")
+
+    @ip.setter
+    def ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip", value)
+
+    @property
+    @pulumi.getter(name="subnetId")
+    def subnet_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the subnet.
+        """
+        return pulumi.get(self, "subnet_id")
+
+    @subnet_id.setter
+    def subnet_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subnet_id", value)
+
+
+@pulumi.input_type
+class GatewayInterfaceArgs:
+    def __init__(__self__, *,
+                 id: Optional[pulumi.Input[str]] = None,
+                 ip: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 subnet_id: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] id: ID of the interface.
+        :param pulumi.Input[str] ip: IP of the interface.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
+        if subnet_id is not None:
+            pulumi.set(__self__, "subnet_id", subnet_id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the interface.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        IP of the interface.
+        """
+        return pulumi.get(self, "ip")
+
+    @ip.setter
+    def ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip", value)
+
+    @property
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the private network.
+        """
+        return pulumi.get(self, "network_id")
+
+    @network_id.setter
+    def network_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_id", value)
+
+    @property
+    @pulumi.getter(name="subnetId")
+    def subnet_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the subnet.
+        """
+        return pulumi.get(self, "subnet_id")
+
+    @subnet_id.setter
+    def subnet_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subnet_id", value)
+
+
+@pulumi.input_type
 class KubeCustomizationArgs:
     def __init__(__self__, *,
                  apiservers: Optional[pulumi.Input[Sequence[pulumi.Input['KubeCustomizationApiserverArgs']]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input['KubeCustomizationApiserverArgs']]] apiservers: Kubernetes API server customization
         """
         if apiservers is not None:
@@ -584,41 +736,31 @@
 
 
 @pulumi.input_type
 class KubeCustomizationApiserverAdmissionpluginArgs:
     def __init__(__self__, *,
                  disableds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  enableds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] disableds: Array of admission plugins disabled, default is [] and only AlwaysPulImages can be disabled at this time.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] enableds: Array of admission plugins enabled, default is ["NodeRestriction","AlwaysPulImages"] and only these admission plugins can be enabled at this time.
-        """
         if disableds is not None:
             pulumi.set(__self__, "disableds", disableds)
         if enableds is not None:
             pulumi.set(__self__, "enableds", enableds)
 
     @property
     @pulumi.getter
     def disableds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Array of admission plugins disabled, default is [] and only AlwaysPulImages can be disabled at this time.
-        """
         return pulumi.get(self, "disableds")
 
     @disableds.setter
     def disableds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "disableds", value)
 
     @property
     @pulumi.getter
     def enableds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Array of admission plugins enabled, default is ["NodeRestriction","AlwaysPulImages"] and only these admission plugins can be enabled at this time.
-        """
         return pulumi.get(self, "enableds")
 
     @enableds.setter
     def enableds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "enableds", value)
 
 
@@ -662,41 +804,31 @@
 
 
 @pulumi.input_type
 class KubeCustomizationKubeProxyIptablesArgs:
     def __init__(__self__, *,
                  min_sync_period: Optional[pulumi.Input[str]] = None,
                  sync_period: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] min_sync_period: Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        :param pulumi.Input[str] sync_period: Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         if min_sync_period is not None:
             pulumi.set(__self__, "min_sync_period", min_sync_period)
         if sync_period is not None:
             pulumi.set(__self__, "sync_period", sync_period)
 
     @property
     @pulumi.getter(name="minSyncPeriod")
     def min_sync_period(self) -> Optional[pulumi.Input[str]]:
-        """
-        Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        """
         return pulumi.get(self, "min_sync_period")
 
     @min_sync_period.setter
     def min_sync_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "min_sync_period", value)
 
     @property
     @pulumi.getter(name="syncPeriod")
     def sync_period(self) -> Optional[pulumi.Input[str]]:
-        """
-        Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         return pulumi.get(self, "sync_period")
 
     @sync_period.setter
     def sync_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sync_period", value)
 
 
@@ -705,22 +837,14 @@
     def __init__(__self__, *,
                  min_sync_period: Optional[pulumi.Input[str]] = None,
                  scheduler: Optional[pulumi.Input[str]] = None,
                  sync_period: Optional[pulumi.Input[str]] = None,
                  tcp_fin_timeout: Optional[pulumi.Input[str]] = None,
                  tcp_timeout: Optional[pulumi.Input[str]] = None,
                  udp_timeout: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] min_sync_period: Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        :param pulumi.Input[str] scheduler: IPVS scheduler.
-        :param pulumi.Input[str] sync_period: Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        :param pulumi.Input[str] tcp_fin_timeout: Timeout value used for IPVS TCP sessions after receiving a FIN in RFC3339 duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        :param pulumi.Input[str] tcp_timeout: Timeout value used for idle IPVS TCP sessions in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        :param pulumi.Input[str] udp_timeout: timeout value used for IPVS UDP packets in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         if min_sync_period is not None:
             pulumi.set(__self__, "min_sync_period", min_sync_period)
         if scheduler is not None:
             pulumi.set(__self__, "scheduler", scheduler)
         if sync_period is not None:
             pulumi.set(__self__, "sync_period", sync_period)
         if tcp_fin_timeout is not None:
@@ -729,77 +853,59 @@
             pulumi.set(__self__, "tcp_timeout", tcp_timeout)
         if udp_timeout is not None:
             pulumi.set(__self__, "udp_timeout", udp_timeout)
 
     @property
     @pulumi.getter(name="minSyncPeriod")
     def min_sync_period(self) -> Optional[pulumi.Input[str]]:
-        """
-        Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        """
         return pulumi.get(self, "min_sync_period")
 
     @min_sync_period.setter
     def min_sync_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "min_sync_period", value)
 
     @property
     @pulumi.getter
     def scheduler(self) -> Optional[pulumi.Input[str]]:
-        """
-        IPVS scheduler.
-        """
         return pulumi.get(self, "scheduler")
 
     @scheduler.setter
     def scheduler(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scheduler", value)
 
     @property
     @pulumi.getter(name="syncPeriod")
     def sync_period(self) -> Optional[pulumi.Input[str]]:
-        """
-        Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         return pulumi.get(self, "sync_period")
 
     @sync_period.setter
     def sync_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sync_period", value)
 
     @property
     @pulumi.getter(name="tcpFinTimeout")
     def tcp_fin_timeout(self) -> Optional[pulumi.Input[str]]:
-        """
-        Timeout value used for IPVS TCP sessions after receiving a FIN in RFC3339 duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "tcp_fin_timeout")
 
     @tcp_fin_timeout.setter
     def tcp_fin_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tcp_fin_timeout", value)
 
     @property
     @pulumi.getter(name="tcpTimeout")
     def tcp_timeout(self) -> Optional[pulumi.Input[str]]:
-        """
-        Timeout value used for idle IPVS TCP sessions in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "tcp_timeout")
 
     @tcp_timeout.setter
     def tcp_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tcp_timeout", value)
 
     @property
     @pulumi.getter(name="udpTimeout")
     def udp_timeout(self) -> Optional[pulumi.Input[str]]:
-        """
-        timeout value used for IPVS UDP packets in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "udp_timeout")
 
     @udp_timeout.setter
     def udp_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "udp_timeout", value)
 
 
@@ -876,37 +982,37 @@
 
 @pulumi.input_type
 class KubeNodePoolTemplateArgs:
     def __init__(__self__, *,
                  metadata: pulumi.Input['KubeNodePoolTemplateMetadataArgs'],
                  spec: pulumi.Input['KubeNodePoolTemplateSpecArgs']):
         """
-        :param pulumi.Input['KubeNodePoolTemplateMetadataArgs'] metadata: Metadata of each node in the pool
-        :param pulumi.Input['KubeNodePoolTemplateSpecArgs'] spec: Spec of each node in the pool
+        :param pulumi.Input['KubeNodePoolTemplateMetadataArgs'] metadata: metadata
+        :param pulumi.Input['KubeNodePoolTemplateSpecArgs'] spec: spec
         """
         pulumi.set(__self__, "metadata", metadata)
         pulumi.set(__self__, "spec", spec)
 
     @property
     @pulumi.getter
     def metadata(self) -> pulumi.Input['KubeNodePoolTemplateMetadataArgs']:
         """
-        Metadata of each node in the pool
+        metadata
         """
         return pulumi.get(self, "metadata")
 
     @metadata.setter
     def metadata(self, value: pulumi.Input['KubeNodePoolTemplateMetadataArgs']):
         pulumi.set(self, "metadata", value)
 
     @property
     @pulumi.getter
     def spec(self) -> pulumi.Input['KubeNodePoolTemplateSpecArgs']:
         """
-        Spec of each node in the pool
+        spec
         """
         return pulumi.get(self, "spec")
 
     @spec.setter
     def spec(self, value: pulumi.Input['KubeNodePoolTemplateSpecArgs']):
         pulumi.set(self, "spec", value)
 
@@ -914,88 +1020,88 @@
 @pulumi.input_type
 class KubeNodePoolTemplateMetadataArgs:
     def __init__(__self__, *,
                  annotations: pulumi.Input[Mapping[str, pulumi.Input[str]]],
                  finalizers: pulumi.Input[Sequence[pulumi.Input[str]]],
                  labels: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] annotations: Annotations to apply to each node
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] finalizers: Finalizers to apply to each node. A finalizer name must be fully qualified, e.g. kubernetes.io/pv-protection , where you prefix it with hostname of your service which is related to the controller responsible for the finalizer.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Labels to apply to each node
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] annotations: annotations
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] finalizers: finalizers
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: labels
         """
         pulumi.set(__self__, "annotations", annotations)
         pulumi.set(__self__, "finalizers", finalizers)
         pulumi.set(__self__, "labels", labels)
 
     @property
     @pulumi.getter
     def annotations(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        Annotations to apply to each node
+        annotations
         """
         return pulumi.get(self, "annotations")
 
     @annotations.setter
     def annotations(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "annotations", value)
 
     @property
     @pulumi.getter
     def finalizers(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Finalizers to apply to each node. A finalizer name must be fully qualified, e.g. kubernetes.io/pv-protection , where you prefix it with hostname of your service which is related to the controller responsible for the finalizer.
+        finalizers
         """
         return pulumi.get(self, "finalizers")
 
     @finalizers.setter
     def finalizers(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "finalizers", value)
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
-        Labels to apply to each node
+        labels
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "labels", value)
 
 
 @pulumi.input_type
 class KubeNodePoolTemplateSpecArgs:
     def __init__(__self__, *,
                  taints: pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]],
                  unschedulable: pulumi.Input[bool]):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] taints: Taints to apply to each node [NodeSpec kubernetes documentation](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1/#NodeSpec)
-        :param pulumi.Input[bool] unschedulable: If true, set nodes as un-schedulable
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] taints: taints
+        :param pulumi.Input[bool] unschedulable: unschedulable
         """
         pulumi.set(__self__, "taints", taints)
         pulumi.set(__self__, "unschedulable", unschedulable)
 
     @property
     @pulumi.getter
     def taints(self) -> pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]:
         """
-        Taints to apply to each node [NodeSpec kubernetes documentation](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1/#NodeSpec)
+        taints
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]):
         pulumi.set(self, "taints", value)
 
     @property
     @pulumi.getter
     def unschedulable(self) -> pulumi.Input[bool]:
         """
-        If true, set nodes as un-schedulable
+        unschedulable
         """
         return pulumi.get(self, "unschedulable")
 
     @unschedulable.setter
     def unschedulable(self, value: pulumi.Input[bool]):
         pulumi.set(self, "unschedulable", value)
 
@@ -1006,19 +1112,17 @@
                  default_vrack_gateway: pulumi.Input[str],
                  private_network_routing_as_default: pulumi.Input[bool]):
         """
         :param pulumi.Input[str] default_vrack_gateway: If defined, all egress traffic will be routed towards this IP address, which should belong to the private network. Empty string means disabled.
         :param pulumi.Input[bool] private_network_routing_as_default: Defines whether routing should default to using the nodes' private interface, instead of their public interface. Default is false.
                
                In order to use the gateway IP advertised by the private network subnet DHCP, the following configuration shall be used.
-               <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                ```
-               <!--End PulumiCodeChooser -->
         """
         pulumi.set(__self__, "default_vrack_gateway", default_vrack_gateway)
         pulumi.set(__self__, "private_network_routing_as_default", private_network_routing_as_default)
 
     @property
     @pulumi.getter(name="defaultVrackGateway")
     def default_vrack_gateway(self) -> pulumi.Input[str]:
@@ -1034,19 +1138,17 @@
     @property
     @pulumi.getter(name="privateNetworkRoutingAsDefault")
     def private_network_routing_as_default(self) -> pulumi.Input[bool]:
         """
         Defines whether routing should default to using the nodes' private interface, instead of their public interface. Default is false.
 
         In order to use the gateway IP advertised by the private network subnet DHCP, the following configuration shall be used.
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         ```
-        <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "private_network_routing_as_default")
 
     @private_network_routing_as_default.setter
     def private_network_routing_as_default(self, value: pulumi.Input[bool]):
         pulumi.set(self, "private_network_routing_as_default", value)
 
@@ -1378,15 +1480,15 @@
                  duration: pulumi.Input[str],
                  plan_code: pulumi.Input[str],
                  pricing_mode: pulumi.Input[str],
                  catalog_name: Optional[pulumi.Input[str]] = None,
                  configurations: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectPlanConfigurationArgs']]]] = None):
         """
         :param pulumi.Input[str] duration: duration
-        :param pulumi.Input[str] plan_code: Plan code
+        :param pulumi.Input[str] plan_code: Plan code. This value must be adapted depending on your `OVH_ENDPOINT` value. It's `project.2018` for `ovh-{eu,ca}` and `project` when using `ovh-us`.
         :param pulumi.Input[str] pricing_mode: Pricing model identifier
         :param pulumi.Input[str] catalog_name: Catalog name
         :param pulumi.Input[Sequence[pulumi.Input['ProjectPlanConfigurationArgs']]] configurations: Representation of a configuration item for personalizing product
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
@@ -1407,15 +1509,15 @@
     def duration(self, value: pulumi.Input[str]):
         pulumi.set(self, "duration", value)
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> pulumi.Input[str]:
         """
-        Plan code
+        Plan code. This value must be adapted depending on your `OVH_ENDPOINT` value. It's `project.2018` for `ovh-{eu,ca}` and `project` when using `ovh-us`.
         """
         return pulumi.get(self, "plan_code")
 
     @plan_code.setter
     def plan_code(self, value: pulumi.Input[str]):
         pulumi.set(self, "plan_code", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/alerting.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/alerting.py`

 * *Files 10% similar despite different names*

```diff
@@ -200,26 +200,24 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an alert on a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_alert = ovh.cloud_project.Alerting("my-alert",
             delay=3600,
             email="aaa.bbb@domain.com",
             monthly_threshold=1000,
             service_name="XXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[float] delay: Delay between two alerts in seconds
         :param pulumi.Input[str] email: Email to contact
         :param pulumi.Input[float] monthly_threshold: Monthly threshold for this alerting in currency
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
@@ -232,26 +230,24 @@
                  args: AlertingArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an alert on a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_alert = ovh.cloud_project.Alerting("my-alert",
             delay=3600,
             email="aaa.bbb@domain.com",
             monthly_threshold=1000,
             service_name="XXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AlertingArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,28 +298,26 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a container registry associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         regcap = ovh.CloudProject.get_capabilities_container_filter(service_name="XXXXXX",
             plan_name="SMALL",
             region="GRA")
         my_registry = ovh.cloud_project.ContainerRegistry("my-registry",
             service_name=regcap.service_name,
             plan_id=regcap.id,
             region=regcap.region)
         ```
-        <!--End PulumiCodeChooser -->
 
         > __WARNING__ You can update and migrate to a higher plan at any time but not the contrary.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Registry name
         :param pulumi.Input[str] plan_id: Plan ID of the registry
@@ -334,28 +332,26 @@
                  args: ContainerRegistryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a container registry associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         regcap = ovh.CloudProject.get_capabilities_container_filter(service_name="XXXXXX",
             plan_name="SMALL",
             region="GRA")
         my_registry = ovh.cloud_project.ContainerRegistry("my-registry",
             service_name=regcap.service_name,
             plan_id=regcap.id,
             region=regcap.region)
         ```
-        <!--End PulumiCodeChooser -->
 
         > __WARNING__ You can update and migrate to a higher plan at any time but not the contrary.
 
         :param str resource_name: The name of the resource.
         :param ContainerRegistryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,30 +130,28 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Apply IP restrictions container registry associated with a public cloud project on Harbor UI and API.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         my_mgt_iprestrictions = ovh.cloud_project.ContainerRegistryIPRestrictionsManagement("my-mgt-iprestrictions",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             ip_restrictions=[{
                 "ip_block": "xxx.xxx.xxx.xxx/xx",
                 "description": "xxxxxxx",
             }])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] ip_restrictions: IP restrictions applied on Harbor UI and API.
         :param pulumi.Input[str] registry_id: The id of the Managed Private Registry.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
@@ -164,30 +162,28 @@
                  args: ContainerRegistryIPRestrictionsManagementArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Apply IP restrictions container registry associated with a public cloud project on Harbor UI and API.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         my_mgt_iprestrictions = ovh.cloud_project.ContainerRegistryIPRestrictionsManagement("my-mgt-iprestrictions",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             ip_restrictions=[{
                 "ip_block": "xxx.xxx.xxx.xxx/xx",
                 "description": "xxxxxxx",
             }])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ContainerRegistryIPRestrictionsManagementArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,30 +130,28 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Apply IP restrictions container registry associated with a public cloud project on artifact manager component.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         my_registry_iprestrictions = ovh.cloud_project.ContainerRegistryIPRestrictionsRegistry("my-registry-iprestrictions",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             ip_restrictions=[{
                 "ip_block": "xxx.xxx.xxx.xxx/xx",
                 "description": "xxxxxxx",
             }])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] ip_restrictions: IP restrictions applied on artifact manager component.
         :param pulumi.Input[str] registry_id: The id of the Managed Private Registry.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
@@ -164,30 +162,28 @@
                  args: ContainerRegistryIPRestrictionsRegistryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Apply IP restrictions container registry associated with a public cloud project on artifact manager component.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         my_registry_iprestrictions = ovh.cloud_project.ContainerRegistryIPRestrictionsRegistry("my-registry-iprestrictions",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             ip_restrictions=[{
                 "ip_block": "xxx.xxx.xxx.xxx/xx",
                 "description": "xxxxxxx",
             }])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ContainerRegistryIPRestrictionsRegistryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_oidc.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,14 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an OIDC configuration in an OVHcloud Managed Private Registry.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oidc = ovh.cloud_project.ContainerRegistryOIDC("my-oidc",
             service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
@@ -477,15 +476,14 @@
             oidc_admin_group="harbor-admin",
             oidc_verify_cert=True,
             oidc_auto_onboard=True,
             oidc_user_claim="preferred_username",
             delete_users=False)
         pulumi.export("oidcClientSecret", my_oidc.oidc_client_secret)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Private Registry OIDC can be imported using the tenant `service_name` and registry id `registry_id` separated by "/" E.g.,
 
         bash
 
@@ -516,15 +514,14 @@
                  args: ContainerRegistryOIDCArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an OIDC configuration in an OVHcloud Managed Private Registry.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oidc = ovh.cloud_project.ContainerRegistryOIDC("my-oidc",
             service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
@@ -537,15 +534,14 @@
             oidc_admin_group="harbor-admin",
             oidc_verify_cert=True,
             oidc_auto_onboard=True,
             oidc_user_claim="preferred_username",
             delete_users=False)
         pulumi.export("oidcClientSecret", my_oidc.oidc_client_secret)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Private Registry OIDC can be imported using the tenant `service_name` and registry id `registry_id` separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/container_registry_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/container_registry_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,28 +198,26 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a user for a container registry associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         user = ovh.cloud_project.ContainerRegistryUser("user",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             email="foo@bar.com",
             login="foobar")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] email: User email
         :param pulumi.Input[str] login: Registry name
         :param pulumi.Input[str] registry_id: Registry ID
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
@@ -232,28 +230,26 @@
                  args: ContainerRegistryUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a user for a container registry associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
             registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
         user = ovh.cloud_project.ContainerRegistryUser("user",
             service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
             registry_id=ovh_cloud_project_containerregistry["registry"]["id"],
             email="foo@bar.com",
             login="foobar")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ContainerRegistryUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/database.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                * Redis: "essential", "business"
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] version: The version of the engine in which the service should be deployed
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
-        :param pulumi.Input[str] description: Description of the IP restriction
+        :param pulumi.Input[str] description: Small description of the database service.
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
         :param pulumi.Input[bool] kafka_schema_registry: Defines whether the schema registry is enabled on a Kafka cluster
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         """
         pulumi.set(__self__, "engine", engine)
@@ -200,15 +200,15 @@
     def backup_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "backup_time", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of the IP restriction
+        Small description of the database service.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -299,15 +299,15 @@
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
         :param pulumi.Input[str] created_at: Date of the creation of the cluster.
-        :param pulumi.Input[str] description: Description of the IP restriction
+        :param pulumi.Input[str] description: Small description of the database service.
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] disk_type: Defines the disk type of the database service.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseEndpointArgs']]] endpoints: List of all endpoints objects of the service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
@@ -421,15 +421,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of the IP restriction
+        Small description of the database service.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -657,15 +657,14 @@
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Minimum settings for each engine (region choice is up to the user):
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         cassandradb = ovh.cloud_project.Database("cassandradb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-cassandra",
@@ -786,19 +785,17 @@
             version="9.1",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
                 region="GRA",
             )],
             flavor="db1-4")
         ```
-        <!--End PulumiCodeChooser -->
 
         To deploy a business PostgreSQL service with two nodes on public network:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         postgresql = ovh.cloud_project.Database("postgresql",
             description="my-first-postgresql",
             engine="postgresql",
@@ -811,19 +808,17 @@
                     region="GRA",
                 ),
             ],
             plan="business",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             version="14")
         ```
-        <!--End PulumiCodeChooser -->
 
         To deploy an enterprise MongoDB service with three nodes on private network:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mongodb = ovh.cloud_project.Database("mongodb",
             description="my-first-mongodb",
             engine="mongodb",
@@ -845,15 +840,14 @@
                     subnet_id="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
                 ),
             ],
             plan="production",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             version="5.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters can be imported using the `service_name`, `engine`, `id` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -862,15 +856,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
-        :param pulumi.Input[str] description: Description of the IP restriction
+        :param pulumi.Input[str] description: Small description of the database service.
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]] ip_restrictions: IP Blocks authorized to access to the cluster.
@@ -895,15 +889,14 @@
                  args: DatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Minimum settings for each engine (region choice is up to the user):
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         cassandradb = ovh.cloud_project.Database("cassandradb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-cassandra",
@@ -1024,19 +1017,17 @@
             version="9.1",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
                 region="GRA",
             )],
             flavor="db1-4")
         ```
-        <!--End PulumiCodeChooser -->
 
         To deploy a business PostgreSQL service with two nodes on public network:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         postgresql = ovh.cloud_project.Database("postgresql",
             description="my-first-postgresql",
             engine="postgresql",
@@ -1049,19 +1040,17 @@
                     region="GRA",
                 ),
             ],
             plan="business",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             version="14")
         ```
-        <!--End PulumiCodeChooser -->
 
         To deploy an enterprise MongoDB service with three nodes on private network:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mongodb = ovh.cloud_project.Database("mongodb",
             description="my-first-mongodb",
             engine="mongodb",
@@ -1083,15 +1072,14 @@
                     subnet_id="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
                 ),
             ],
             plan="production",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             version="5.0")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters can be imported using the `service_name`, `engine`, `id` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -1209,15 +1197,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
         :param pulumi.Input[str] created_at: Date of the creation of the cluster.
-        :param pulumi.Input[str] description: Description of the IP restriction
+        :param pulumi.Input[str] description: Small description of the database service.
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] disk_type: Defines the disk type of the database service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseEndpointArgs']]]] endpoints: List of all endpoints objects of the service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
@@ -1299,15 +1287,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Description of the IP restriction
+        Small description of the database service.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/failover_ip_attach.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/failover_ip_attach.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,25 +283,23 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Attaches a failover IP address to a compute instance
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfailoverip = ovh.cloud_project.FailoverIpAttach("myfailoverip",
             ip="XXXXXX",
             routed_to="XXXXXX",
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] block: The IP block
         :param pulumi.Input[str] continent_code: Ip continent
         :param pulumi.Input[str] geo_loc: Ip location
         :param pulumi.Input[str] ip: The failover ip address to attach
@@ -316,25 +314,23 @@
                  args: FailoverIpAttachArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Attaches a failover IP address to a compute instance
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfailoverip = ovh.cloud_project.FailoverIpAttach("myfailoverip",
             ip="XXXXXX",
             routed_to="XXXXXX",
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FailoverIpAttachArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/gateway.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/gateway.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,136 +4,146 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['GatewayArgs', 'Gateway']
 
 @pulumi.input_type
 class GatewayArgs:
     def __init__(__self__, *,
                  model: pulumi.Input[str],
                  network_id: pulumi.Input[str],
                  region: pulumi.Input[str],
                  service_name: pulumi.Input[str],
                  subnet_id: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Gateway resource.
-        :param pulumi.Input[str] model: The model of the gateway.
-        :param pulumi.Input[str] network_id: The ID of the private network.
-        :param pulumi.Input[str] region: The region of the gateway.
-        :param pulumi.Input[str] service_name: The ID of the private network.
-        :param pulumi.Input[str] subnet_id: The ID of the subnet.
-        :param pulumi.Input[str] name: The name of the gateway.
+        :param pulumi.Input[str] model: Model of the gateway.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        :param pulumi.Input[str] region: Region of the gateway.
+        :param pulumi.Input[str] service_name: ID of the private network.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
+        :param pulumi.Input[str] name: Name of the gateway.
         """
         pulumi.set(__self__, "model", model)
         pulumi.set(__self__, "network_id", network_id)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "subnet_id", subnet_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def model(self) -> pulumi.Input[str]:
         """
-        The model of the gateway.
+        Model of the gateway.
         """
         return pulumi.get(self, "model")
 
     @model.setter
     def model(self, value: pulumi.Input[str]):
         pulumi.set(self, "model", value)
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> pulumi.Input[str]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "network_id")
 
     @network_id.setter
     def network_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "network_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Input[str]:
         """
-        The region of the gateway.
+        Region of the gateway.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> pulumi.Input[str]:
         """
-        The ID of the subnet.
+        ID of the subnet.
         """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "subnet_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the gateway.
+        Name of the gateway.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class _GatewayState:
     def __init__(__self__, *,
+                 external_informations: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationArgs']]]] = None,
+                 interfaces: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayInterfaceArgs']]]] = None,
                  model: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Gateway resources.
-        :param pulumi.Input[str] model: The model of the gateway.
-        :param pulumi.Input[str] name: The name of the gateway.
-        :param pulumi.Input[str] network_id: The ID of the private network.
-        :param pulumi.Input[str] region: The region of the gateway.
-        :param pulumi.Input[str] service_name: The ID of the private network.
-        :param pulumi.Input[str] status: The status of the gateway.
-        :param pulumi.Input[str] subnet_id: The ID of the subnet.
-        """
+        :param pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationArgs']]] external_informations: List of External Information of the gateway.
+        :param pulumi.Input[Sequence[pulumi.Input['GatewayInterfaceArgs']]] interfaces: Interfaces list of the gateway.
+        :param pulumi.Input[str] model: Model of the gateway.
+        :param pulumi.Input[str] name: Name of the gateway.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        :param pulumi.Input[str] region: Region of the gateway.
+        :param pulumi.Input[str] service_name: ID of the private network.
+        :param pulumi.Input[str] status: Status of the gateway.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
+        """
+        if external_informations is not None:
+            pulumi.set(__self__, "external_informations", external_informations)
+        if interfaces is not None:
+            pulumi.set(__self__, "interfaces", interfaces)
         if model is not None:
             pulumi.set(__self__, "model", model)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
         if region is not None:
@@ -142,90 +152,114 @@
             pulumi.set(__self__, "service_name", service_name)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if subnet_id is not None:
             pulumi.set(__self__, "subnet_id", subnet_id)
 
     @property
+    @pulumi.getter(name="externalInformations")
+    def external_informations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationArgs']]]]:
+        """
+        List of External Information of the gateway.
+        """
+        return pulumi.get(self, "external_informations")
+
+    @external_informations.setter
+    def external_informations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayExternalInformationArgs']]]]):
+        pulumi.set(self, "external_informations", value)
+
+    @property
+    @pulumi.getter
+    def interfaces(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GatewayInterfaceArgs']]]]:
+        """
+        Interfaces list of the gateway.
+        """
+        return pulumi.get(self, "interfaces")
+
+    @interfaces.setter
+    def interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GatewayInterfaceArgs']]]]):
+        pulumi.set(self, "interfaces", value)
+
+    @property
     @pulumi.getter
     def model(self) -> Optional[pulumi.Input[str]]:
         """
-        The model of the gateway.
+        Model of the gateway.
         """
         return pulumi.get(self, "model")
 
     @model.setter
     def model(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "model", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the gateway.
+        Name of the gateway.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "network_id")
 
     @network_id.setter
     def network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the gateway.
+        Region of the gateway.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        The status of the gateway.
+        Status of the gateway.
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the subnet.
+        ID of the subnet.
         """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
@@ -241,32 +275,52 @@
                  region: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a new Gateway for existing subnet in the specified public cloud project.
 
+        ## Import
+
+        A gateway can be imported using the `service_name`, `region` and `id` (identifier of the gateway) properties, separated by a `/`.
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:CloudProject/gateway:Gateway gateway service_name/region/id
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] model: The model of the gateway.
-        :param pulumi.Input[str] name: The name of the gateway.
-        :param pulumi.Input[str] network_id: The ID of the private network.
-        :param pulumi.Input[str] region: The region of the gateway.
-        :param pulumi.Input[str] service_name: The ID of the private network.
-        :param pulumi.Input[str] subnet_id: The ID of the subnet.
+        :param pulumi.Input[str] model: Model of the gateway.
+        :param pulumi.Input[str] name: Name of the gateway.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        :param pulumi.Input[str] region: Region of the gateway.
+        :param pulumi.Input[str] service_name: ID of the private network.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GatewayArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a new Gateway for existing subnet in the specified public cloud project.
 
+        ## Import
+
+        A gateway can be imported using the `service_name`, `region` and `id` (identifier of the gateway) properties, separated by a `/`.
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:CloudProject/gateway:Gateway gateway service_name/region/id
+        ```
+
         :param str resource_name: The name of the resource.
         :param GatewayArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(GatewayArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -305,109 +359,133 @@
             __props__.__dict__["region"] = region
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
             if subnet_id is None and not opts.urn:
                 raise TypeError("Missing required property 'subnet_id'")
             __props__.__dict__["subnet_id"] = subnet_id
+            __props__.__dict__["external_informations"] = None
+            __props__.__dict__["interfaces"] = None
             __props__.__dict__["status"] = None
         super(Gateway, __self__).__init__(
             'ovh:CloudProject/gateway:Gateway',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            external_informations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GatewayExternalInformationArgs']]]]] = None,
+            interfaces: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GatewayInterfaceArgs']]]]] = None,
             model: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             network_id: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             service_name: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             subnet_id: Optional[pulumi.Input[str]] = None) -> 'Gateway':
         """
         Get an existing Gateway resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] model: The model of the gateway.
-        :param pulumi.Input[str] name: The name of the gateway.
-        :param pulumi.Input[str] network_id: The ID of the private network.
-        :param pulumi.Input[str] region: The region of the gateway.
-        :param pulumi.Input[str] service_name: The ID of the private network.
-        :param pulumi.Input[str] status: The status of the gateway.
-        :param pulumi.Input[str] subnet_id: The ID of the subnet.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GatewayExternalInformationArgs']]]] external_informations: List of External Information of the gateway.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GatewayInterfaceArgs']]]] interfaces: Interfaces list of the gateway.
+        :param pulumi.Input[str] model: Model of the gateway.
+        :param pulumi.Input[str] name: Name of the gateway.
+        :param pulumi.Input[str] network_id: ID of the private network.
+        :param pulumi.Input[str] region: Region of the gateway.
+        :param pulumi.Input[str] service_name: ID of the private network.
+        :param pulumi.Input[str] status: Status of the gateway.
+        :param pulumi.Input[str] subnet_id: ID of the subnet.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GatewayState.__new__(_GatewayState)
 
+        __props__.__dict__["external_informations"] = external_informations
+        __props__.__dict__["interfaces"] = interfaces
         __props__.__dict__["model"] = model
         __props__.__dict__["name"] = name
         __props__.__dict__["network_id"] = network_id
         __props__.__dict__["region"] = region
         __props__.__dict__["service_name"] = service_name
         __props__.__dict__["status"] = status
         __props__.__dict__["subnet_id"] = subnet_id
         return Gateway(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="externalInformations")
+    def external_informations(self) -> pulumi.Output[Sequence['outputs.GatewayExternalInformation']]:
+        """
+        List of External Information of the gateway.
+        """
+        return pulumi.get(self, "external_informations")
+
+    @property
+    @pulumi.getter
+    def interfaces(self) -> pulumi.Output[Sequence['outputs.GatewayInterface']]:
+        """
+        Interfaces list of the gateway.
+        """
+        return pulumi.get(self, "interfaces")
+
+    @property
     @pulumi.getter
     def model(self) -> pulumi.Output[str]:
         """
-        The model of the gateway.
+        Model of the gateway.
         """
         return pulumi.get(self, "model")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the gateway.
+        Name of the gateway.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> pulumi.Output[str]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "network_id")
 
     @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
-        The region of the gateway.
+        Region of the gateway.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The ID of the private network.
+        ID of the private network.
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
-        The status of the gateway.
+        Status of the gateway.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> pulumi.Output[str]:
         """
-        The ID of the subnet.
+        ID of the subnet.
         """
         return pulumi.get(self, "subnet_id")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_capabilities_container_filter.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,24 +149,22 @@
                                       service_name: Optional[str] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCapabilitiesContainerFilterResult:
     """
     Use this data source to filter the list of container registry capabilities associated with a public cloud project to match one and only one capability.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     capability = ovh.CloudProject.get_capabilities_container_filter(plan_name="SMALL",
         region="GRA",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str plan_name: The plan name. It can be 'SMALL', 'MEDIUM' or 'LARGE'.
     :param str region: The region name
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -196,24 +194,22 @@
                                              service_name: Optional[pulumi.Input[str]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCapabilitiesContainerFilterResult]:
     """
     Use this data source to filter the list of container registry capabilities associated with a public cloud project to match one and only one capability.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     capability = ovh.CloudProject.get_capabilities_container_filter(plan_name="SMALL",
         region="GRA",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str plan_name: The plan name. It can be 'SMALL', 'MEDIUM' or 'LARGE'.
     :param str region: The region name
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_capabilities_container_registry.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_capabilities_container_registry(service_name: Optional[str] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCapabilitiesContainerRegistryResult:
     """
     Use this data source to get the container registry capabilities of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     capabilities = ovh.CloudProject.get_capabilities_container_registry(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -101,21 +99,19 @@
 def get_capabilities_container_registry_output(service_name: Optional[pulumi.Input[str]] = None,
                                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCapabilitiesContainerRegistryResult]:
     """
     Use this data source to get the container registry capabilities of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     capabilities = ovh.CloudProject.get_capabilities_container_registry(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registries.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registries.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,20 @@
 def get_container_registries(service_name: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetContainerRegistriesResult:
     """
     Use this data source to get the container registries of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     registries = ovh.CloudProject.get_container_registries(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -101,21 +99,19 @@
 def get_container_registries_output(service_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContainerRegistriesResult]:
     """
     Use this data source to get the container registries of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     registries = ovh.CloudProject.get_container_registries(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,23 +174,21 @@
                            service_name: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetContainerRegistryResult:
     """
     Use this data source to get information about a container registry associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_registry = ovh.CloudProject.get_container_registry(registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str registry_id: Registry ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -219,23 +217,21 @@
                                   service_name: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContainerRegistryResult]:
     """
     Use this data source to get information about a container registry associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_registry = ovh.CloudProject.get_container_registry(registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str registry_id: Registry ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_oidc.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,24 +189,22 @@
                                 service_name: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetContainerRegistryOIDCResult:
     """
     Use this data source to get a OVHcloud Managed Private Registry OIDC.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oidc = ovh.CloudProject.get_container_registry_oidc(service_name="XXXXXX",
         registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("oidc-client-id", my_oidc.oidc_client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str oidc_admin_group: Specify an OIDC admin group name. All OIDC users in this group will have harbor admin privilege. Keep it blank if you do not want to.
     :param bool oidc_auto_onboard: Skip the onboarding screen, so user cannot change its username. Username is provided from ID Token.
     :param str oidc_client_id: The client ID with which Harbor is registered as client application with the OIDC provider.
     :param str oidc_endpoint: The URL of an OIDC-compliant server.
     :param str oidc_groups_claim: The name of Claim in the ID token whose value is the list of group names.
@@ -261,24 +259,22 @@
                                        service_name: Optional[pulumi.Input[str]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContainerRegistryOIDCResult]:
     """
     Use this data source to get a OVHcloud Managed Private Registry OIDC.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oidc = ovh.CloudProject.get_container_registry_oidc(service_name="XXXXXX",
         registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("oidc-client-id", my_oidc.oidc_client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str oidc_admin_group: Specify an OIDC admin group name. All OIDC users in this group will have harbor admin privilege. Keep it blank if you do not want to.
     :param bool oidc_auto_onboard: Skip the onboarding screen, so user cannot change its username. Username is provided from ID Token.
     :param str oidc_client_id: The client ID with which Harbor is registered as client application with the OIDC provider.
     :param str oidc_endpoint: The URL of an OIDC-compliant server.
     :param str oidc_groups_claim: The name of Claim in the ID token whose value is the list of group names.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_container_registry_users.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_container_registry_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,25 +79,23 @@
                                  service_name: Optional[str] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetContainerRegistryUsersResult:
     """
     Use this data source to get the list of users of a container registry associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
         registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     users = ovh.CloudProject.get_container_registry_users(service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
         registry_id=ovh_cloud_project_containerregistry["registry"]["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str registry_id: Registry ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -118,25 +116,23 @@
                                         service_name: Optional[pulumi.Input[str]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetContainerRegistryUsersResult]:
     """
     Use this data source to get the list of users of a container registry associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_registry = ovh.CloudProject.get_container_registry(service_name="XXXXXX",
         registry_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     users = ovh.CloudProject.get_container_registry_users(service_name=ovh_cloud_project_containerregistry["registry"]["service_name"],
         registry_id=ovh_cloud_project_containerregistry["registry"]["id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str registry_id: Registry ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_failover_ip_attach.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,23 +145,21 @@
                            service_name: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFailoverIpAttachResult:
     """
     Use this data source to get the details of a failover IP address of a service in a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfailoverip = ovh.CloudProject.get_failover_ip_attach(ip="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str block: The IP block
     :param str ip: The failover ip address to query
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -197,23 +195,21 @@
                                   service_name: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFailoverIpAttachResult]:
     """
     Use this data source to get the details of a failover IP address of a service in a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfailoverip = ovh.CloudProject.get_failover_ip_attach(ip="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str block: The IP block
     :param str ip: The failover ip address to query
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,24 +265,22 @@
              version: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeResult:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_kube_cluster = ovh.CloudProject.get_kube(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("version", my_kube_cluster.version)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetKubeCustomizationApiserverArgs']] customization_apiservers: Kubernetes API server customization
     :param pulumi.InputType['GetKubeCustomizationKubeProxyArgs'] customization_kube_proxy: Kubernetes kube-proxy customization
     :param Sequence[pulumi.InputType['GetKubeCustomizationArgs']] customizations: **Deprecated** (Optional) Use `customization_apiserver` and `customization_kube_proxy` instead. Kubernetes cluster customization
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str kube_proxy_mode: Selected mode for kube-proxy.
@@ -340,24 +338,22 @@
                     version: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeResult]:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_kube_cluster = ovh.CloudProject.get_kube(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("version", my_kube_cluster.version)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetKubeCustomizationApiserverArgs']] customization_apiservers: Kubernetes API server customization
     :param pulumi.InputType['GetKubeCustomizationKubeProxyArgs'] customization_kube_proxy: Kubernetes kube-proxy customization
     :param Sequence[pulumi.InputType['GetKubeCustomizationArgs']] customizations: **Deprecated** (Optional) Use `customization_apiserver` and `customization_kube_proxy` instead. Kubernetes cluster customization
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str kube_proxy_mode: Selected mode for kube-proxy.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                              service_name: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeIpRestrictionsResult:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster IP restrictions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     iprestrictions = ovh.CloudProject.get_kube_ip_restrictions(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("ips", iprestrictions.ips)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                                     service_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeIpRestrictionsResult]:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster IP restrictions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     iprestrictions = ovh.CloudProject.get_kube_ip_restrictions(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("ips", iprestrictions.ips)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_node_pool.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_node_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,25 +334,23 @@
                        template: Optional[pulumi.InputType['GetKubeNodePoolTemplateArgs']] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeNodePoolResult:
     """
     Use this data source to get a OVHcloud Managed Kubernetes node pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodepool = ovh.CloudProject.get_kube_node_pool(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
         name="xxxxxx")
     pulumi.export("maxNodes", nodepool.max_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str name: The name of the node pool.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -398,25 +396,23 @@
                               template: Optional[pulumi.Input[Optional[pulumi.InputType['GetKubeNodePoolTemplateArgs']]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeNodePoolResult]:
     """
     Use this data source to get a OVHcloud Managed Kubernetes node pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodepool = ovh.CloudProject.get_kube_node_pool(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
         name="xxxxxx")
     pulumi.export("maxNodes", nodepool.max_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str name: The name of the node pool.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,25 +98,23 @@
                              service_name: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeNodePoolNodesResult:
     """
     Use this data source to get a list of OVHcloud Managed Kubernetes nodes in a specific node pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodes_kube_node_pool_nodes = ovh.CloudProject.get_kube_node_pool_nodes(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
         name="XXXXXX")
     pulumi.export("nodes", nodes_kube_node_pool_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The ID of the managed kubernetes cluster.
     :param str name: Name of the node pool from which we want the nodes.
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -141,25 +139,23 @@
                                     service_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeNodePoolNodesResult]:
     """
     Use this data source to get a list of OVHcloud Managed Kubernetes nodes in a specific node pool.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodes_kube_node_pool_nodes = ovh.CloudProject.get_kube_node_pool_nodes(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
         name="XXXXXX")
     pulumi.export("nodes", nodes_kube_node_pool_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The ID of the managed kubernetes cluster.
     :param str name: Name of the node pool from which we want the nodes.
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_nodes.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,24 +85,22 @@
                    service_name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeNodesResult:
     """
     Use this data source to get a list of OVHcloud Managed Kubernetes nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodes_kube_nodes = ovh.CloudProject.get_kube_nodes(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx")
     pulumi.export("nodes", nodes_kube_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The ID of the managed kubernetes cluster.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -123,24 +121,22 @@
                           service_name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeNodesResult]:
     """
     Use this data source to get a list of OVHcloud Managed Kubernetes nodes.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     nodes_kube_nodes = ovh.CloudProject.get_kube_nodes(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx")
     pulumi.export("nodes", nodes_kube_nodes)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str kube_id: The ID of the managed kubernetes cluster.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_kube_oidc.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_kube_oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,24 +189,22 @@
                   service_name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeOidcResult:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster OIDC.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     oidc = ovh.CloudProject.get_kube_oidc(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("oidc-val", oidc.client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The OIDC client ID.
     :param str issuer_url: The OIDC issuer url.
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str oidc_ca_content: Content of the certificate for the CA, in base64 format, that signed your identity provider's web certificate. Defaults to the host's root CAs.
     :param Sequence[str] oidc_groups_claims: Array of JWT claim to use as the user's group. If the claim is present it must be an array of strings.
@@ -262,24 +260,22 @@
                          service_name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeOidcResult]:
     """
     Use this data source to get a OVHcloud Managed Kubernetes Service cluster OIDC.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     oidc = ovh.CloudProject.get_kube_oidc(service_name="XXXXXX",
         kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
     pulumi.export("oidc-val", oidc.client_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: The OIDC client ID.
     :param str issuer_url: The OIDC issuer url.
     :param str kube_id: The id of the managed kubernetes cluster.
     :param str oidc_ca_content: Content of the certificate for the CA, in base64 format, that signed your identity provider's web certificate. Defaults to the host's root CAs.
     :param Sequence[str] oidc_groups_claims: Array of JWT claim to use as the user's group. If the claim is present it must be an array of strings.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_namespace.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,25 +193,23 @@
                        service_name: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbNamespaceResult:
     """
     Use this data source to get information about a namespace of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     m3dbnamespace = ovh.CloudProject.get_m3db_namespace(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("m3dbnamespaceType", m3dbnamespace.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the namespace.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -244,25 +242,23 @@
                               service_name: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbNamespaceResult]:
     """
     Use this data source to get information about a namespace of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     m3dbnamespace = ovh.CloudProject.get_m3db_namespace(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("m3dbnamespaceType", m3dbnamespace.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the namespace.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_namespaces.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                         service_name: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbNamespacesResult:
     """
     Use this data source to get the list of namespaces of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     namespaces = ovh.CloudProject.get_m3db_namespaces(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("namespaceIds", namespaces.namespace_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                                service_name: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbNamespacesResult]:
     """
     Use this data source to get the list of namespaces of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     namespaces = ovh.CloudProject.get_m3db_namespaces(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("namespaceIds", namespaces.namespace_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_m3db_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_m3db_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,25 +121,23 @@
                   service_name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbUserResult:
     """
     Use this data source to get information about a user of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     m3dbuser = ovh.CloudProject.get_m3db_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("m3dbuserGroup", m3dbuser.group)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -166,25 +164,23 @@
                          service_name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbUserResult]:
     """
     Use this data source to get information about a user of a M3DB cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     m3dbuser = ovh.CloudProject.get_m3db_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("m3dbuserGroup", m3dbuser.group)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_mongo_db_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_mongo_db_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,25 +121,23 @@
                       service_name: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMongoDbUserResult:
     """
     Use this data source to get information about a user of a mongodb cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mongouser = ovh.CloudProject.get_mongo_db_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ@admin")
     pulumi.export("mongouserRoles", mongouser.roles)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user with the authentication database in the format name@authDB, for example: johndoe@admin
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -166,25 +164,23 @@
                              service_name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMongoDbUserResult]:
     """
     Use this data source to get information about a user of a mongodb cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mongouser = ovh.CloudProject.get_mongo_db_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ@admin")
     pulumi.export("mongouserRoles", mongouser.roles)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user with the authentication database in the format name@authDB, for example: johndoe@admin
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_pattern.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,25 +97,23 @@
                             service_name: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchPatternResult:
     """
     Use this data source to get information about a pattern of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     pattern = ovh.CloudProject.get_open_search_pattern(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("patternPattern", pattern.pattern)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Pattern ID.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -140,25 +138,23 @@
                                    service_name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchPatternResult]:
     """
     Use this data source to get information about a pattern of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     pattern = ovh.CloudProject.get_open_search_pattern(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("patternPattern", pattern.pattern)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Pattern ID.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_patterns.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                              service_name: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchPatternsResult:
     """
     Use this data source to get the list of pattern of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     patterns = ovh.CloudProject.get_open_search_patterns(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("patternIds", patterns.pattern_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                                     service_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchPatternsResult]:
     """
     Use this data source to get the list of pattern of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     patterns = ovh.CloudProject.get_open_search_patterns(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("patternIds", patterns.pattern_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_open_search_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_open_search_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,25 +122,23 @@
                          service_name: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchUserResult:
     """
     Use this data source to get information about a user of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     osuser = ovh.CloudProject.get_open_search_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("osuserAcls", osuser.acls)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -167,25 +165,23 @@
                                 service_name: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchUserResult]:
     """
     Use this data source to get information about a user of a opensearch cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     osuser = ovh.CloudProject.get_open_search_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("osuserAcls", osuser.acls)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_redis_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_redis_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,25 +157,23 @@
                    service_name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRedisUserResult:
     """
     Use this data source to get information about a user of a redis cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     redisuser = ovh.CloudProject.get_redis_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("redisuserCommands", redisuser.commands)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -205,25 +203,23 @@
                           service_name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRedisUserResult]:
     """
     Use this data source to get information about a user of a redis cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     redisuser = ovh.CloudProject.get_redis_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("redisuserCommands", redisuser.commands)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_region.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_region.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,23 +108,21 @@
                service_name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegionResult:
     """
     Use this data source to retrieve information about a region associated with a public cloud project. The region must be associated with the project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     g_ra1 = ovh.CloudProject.get_region(name="GRA1",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the region associated with the public cloud
            project.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -148,23 +146,21 @@
                       service_name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionResult]:
     """
     Use this data source to retrieve information about a region associated with a public cloud project. The region must be associated with the project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     g_ra1 = ovh.CloudProject.get_region(name="GRA1",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the region associated with the public cloud
            project.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_regions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,23 +78,21 @@
                 service_name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegionsResult:
     """
     Use this data source to get the regions of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     regions = ovh.CloudProject.get_regions(has_services_ups=["network"],
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] has_services_ups: List of services which has to be UP in regions.
            Example: "image", "instance", "network", "storage", "volume", "workflow", ...
            If left blank, returns all regions associated with the service_name.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
@@ -117,23 +115,21 @@
                        service_name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionsResult]:
     """
     Use this data source to get the regions of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     regions = ovh.CloudProject.get_regions(has_services_ups=["network"],
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] has_services_ups: List of services which has to be UP in regions.
            Example: "image", "instance", "network", "storage", "volume", "workflow", ...
            If left blank, returns all regions associated with the service_name.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,27 +128,25 @@
              user_id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Get the user details of a previously created public cloud project user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     my_user = ovh.CloudProject.get_user(service_name=project_users.service_name,
         user_id=s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     __args__ = dict()
@@ -173,27 +171,25 @@
                     user_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Get the user details of a previously created public cloud project user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     my_user = ovh.CloudProject.get_user(service_name=project_users.service_name,
         user_id=s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_credential.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,14 @@
                            user_id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserS3CredentialResult:
     """
     Use this data source to retrieve the Secret Access Key of an Access Key ID associated with a public cloud project's user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
@@ -105,15 +104,14 @@
         user_id=s3_user_id)
     my_s3_credential = ovh.CloudProject.get_user_s3_credential(service_name=my_s3_credentials.service_name,
         user_id=my_s3_credentials.user_id,
         access_key_id=my_s3_credentials.access_key_ids[0])
     pulumi.export("myAccessKeyId", my_s3_credential.access_key_id)
     pulumi.export("mySecretAccessKey", my_s3_credential.secret_access_key)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str access_key_id: the Access Key ID
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
@@ -138,15 +136,14 @@
                                   user_id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserS3CredentialResult]:
     """
     Use this data source to retrieve the Secret Access Key of an Access Key ID associated with a public cloud project's user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
@@ -155,15 +152,14 @@
         user_id=s3_user_id)
     my_s3_credential = ovh.CloudProject.get_user_s3_credential(service_name=my_s3_credentials.service_name,
         user_id=my_s3_credentials.user_id,
         access_key_id=my_s3_credentials.access_key_ids[0])
     pulumi.export("myAccessKeyId", my_s3_credential.access_key_id)
     pulumi.export("mySecretAccessKey", my_s3_credential.secret_access_key)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str access_key_id: the Access Key ID
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_credentials.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,24 +78,22 @@
                             user_id: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserS3CredentialsResult:
     """
     Use this data source to retrieve the list of all the S3 access_key_id associated with a public cloud project's user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_s3_credentials = ovh.CloudProject.get_user_s3_credentials(service_name="XXXXXX",
         user_id="1234")
     pulumi.export("accessKeyIds", my_s3_credentials.access_key_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     __args__ = dict()
@@ -116,24 +114,22 @@
                                    user_id: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserS3CredentialsResult]:
     """
     Use this data source to retrieve the list of all the S3 access_key_id associated with a public cloud project's user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_s3_credentials = ovh.CloudProject.get_user_s3_credentials(service_name="XXXXXX",
         user_id="1234")
     pulumi.export("accessKeyIds", my_s3_credentials.access_key_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_user_s3_policy.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_user_s3_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,27 +78,25 @@
                        user_id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserS3PolicyResult:
     """
     Get the S3 Policy of a public cloud project user. The policy can be set by using the `CloudProject.S3Policy` resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     policy = ovh.CloudProject.get_user_s3_policy(service_name=project_users.service_name,
         user_id=s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     __args__ = dict()
@@ -119,27 +117,25 @@
                               user_id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserS3PolicyResult]:
     """
     Get the S3 Policy of a public cloud project user. The policy can be set by using the `CloudProject.S3Policy` resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     policy = ovh.CloudProject.get_user_s3_policy(service_name=project_users.service_name,
         user_id=s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: The ID of a public cloud project's user.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_users.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_users.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,26 +69,24 @@
 def get_users(service_name: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Get the list of all users of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     pulumi.export("userId", s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -105,25 +103,23 @@
 def get_users_output(service_name: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Get the list of all users of a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     project_users = ovh.CloudProject.get_users(service_name="XXX")
     # Get the user ID of a previously created user with the description "S3-User"
     users = [user.user_id for user in project_users.users if user.description == "S3-User"]
     s3_user_id = users[0]
     pulumi.export("userId", s3_user_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The ID of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/get_v_rack.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/get_v_rack.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,23 +80,21 @@
 def get_v_rack(service_name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVRackResult:
     """
     Use this data source to get the linked vrack on your public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     vrack_v_rack = ovh.CloudProject.get_v_rack(service_name="XXXXXX")
     pulumi.export("vrack", vrack_v_rack)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -114,22 +112,20 @@
 def get_v_rack_output(service_name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVRackResult]:
     """
     Use this data source to get the linked vrack on your public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     vrack_v_rack = ovh.CloudProject.get_v_rack(service_name="XXXXXX")
     pulumi.export("vrack", vrack_v_rack)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_ip_restrictions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,25 +130,23 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Apply IP restrictions to an OVHcloud Managed Kubernetes cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         vrack_only = ovh.cloud_project.KubeIpRestrictions("vrackOnly",
             ips=["10.42.0.0/16"],
             kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster IP restrictions can be imported using the `service_name` and the `id` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -169,25 +167,23 @@
                  args: KubeIpRestrictionsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Apply IP restrictions to an OVHcloud Managed Kubernetes cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         vrack_only = ovh.cloud_project.KubeIpRestrictions("vrackOnly",
             ips=["10.42.0.0/16"],
             kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster IP restrictions can be imported using the `service_name` and the `id` of the cluster, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_node_pool.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_node_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -661,32 +661,29 @@
         """
         Creates a nodepool in a OVHcloud Managed Kubernetes Service cluster.
 
         ## Example Usage
 
         Create a simple node pool in your Kubernetes cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         node_pool = ovh.cloud_project.KubeNodePool("nodePool",
             desired_nodes=3,
             flavor_name="b2-7",
             kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
             max_nodes=3,
             min_nodes=3,
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         Create an advanced node pool in your Kubernetes cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         pool = ovh.cloud_project.KubeNodePool("pool",
             desired_nodes=3,
             flavor_name="b2-7",
@@ -715,15 +712,14 @@
                         "key": "k",
                         "value": "v",
                     }],
                     unschedulable=False,
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster node pool can be imported using the `service_name`, the `id` of the cluster, and the `id` of the nodepool separated by "/" E.g.,
 
         bash
 
@@ -762,32 +758,29 @@
         """
         Creates a nodepool in a OVHcloud Managed Kubernetes Service cluster.
 
         ## Example Usage
 
         Create a simple node pool in your Kubernetes cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         node_pool = ovh.cloud_project.KubeNodePool("nodePool",
             desired_nodes=3,
             flavor_name="b2-7",
             kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
             max_nodes=3,
             min_nodes=3,
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         Create an advanced node pool in your Kubernetes cluster:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         pool = ovh.cloud_project.KubeNodePool("pool",
             desired_nodes=3,
             flavor_name="b2-7",
@@ -816,15 +809,14 @@
                         "key": "k",
                         "value": "v",
                     }],
                     unschedulable=False,
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster node pool can be imported using the `service_name`, the `id` of the cluster, and the `id` of the nodepool separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/kube_oidc.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/kube_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,14 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an OIDC configuration in an OVHcloud Managed Kubernetes cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oidc = ovh.cloud_project.KubeOidc("my-oidc",
             service_name=var["projectid"],
             kube_id=ovh_cloud_project_kube["mykube"]["id"],
@@ -411,15 +410,14 @@
             oidc_username_prefix="ovh:",
             oidc_groups_claims=["groups"],
             oidc_groups_prefix="ovh:",
             oidc_required_claims=["claim1=val1"],
             oidc_signing_algs=["RS512"],
             oidc_ca_content="LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZhekNDQTFPZ0F3SUJBZ0lVYm9YRkZrL1hCQmdQUUI4UHlqbkttUGVWekNjd0RRWUpLb1pJaHZjTkFRRUwKQlFBd1JURUxNQWtHQTFVRUJoTUNRVlV4RXpBUkJnTlZCQWdNQ2xOdmJXVXRVM1JoZEdVeElUQWZCZ05WQkFvTQpHRWx1ZEdWeWJtVjBJRmRwWkdkcGRITWdVSFI1SUV4MFpEQWVGdzB5TWpFd01UUXdOalE0TlROYUZ3MHlNekV3Ck1UUXdOalE0TlROYU1FVXhDekFKQmdOVkJBWVRBa0ZWTVJNd0VRWURWUVFJREFwVGIyMWxMVk4wWVhSbE1TRXcKSHdZRFZRUUtEQmhKYm5SbGNtNWxkQ0JYYVdSbmFYUnpJRkIwZVNCTWRHUXdnZ0lpTUEwR0NTcUdTSWIzRFFFQgpBUVVBQTRJQ0R3QXdnZ0lLQW9JQ0FRQytPMk53bGx2QTQyT05SUHMyZWlqTUp2UHhpN21RblVSS3FrOHJEV1VkCkwzZU0yM1JXeVhtS1AydDQ5Zi9LVGsweEZNVStOSTUzTEhwWmh6N3NpK3dEUFUvWWZWSS9rQmZsRm8zeVZCMSsKZWdCSnpyNGIrQ3FoaWlCUkh0Vm5LblFKUmdvOVJjVkxhRm82UEY0N1V0UWJ2bWVuNGdERnExVkYwVHhUdnFMdwpIMzRZL0U2QUJsSlZnWFBzaWQzNm54eTErNnlKV05vRXNVekFiekpWMHhzTGhxc2hOazA0TWx4YnBhcG1XcEUxCmFFMHRIZGpjUlI3Y1dTRUUwMnRSQzNYL2tSNjBKb3MxR0N0Y0ZQTTVIN3NjOFBXNFRUem1EWWhOeDRiVjV4T28KU0xYRnI5ajBzZEgxbm1wSlI1dWxJT2dPTWV3MHA2d3JOYVV2MGpxc1hzdVdqMVpxdTRLRi81aEQ3azVhRlhKNQpjYWNTUi9mRWxreW1uZis0eHZFOG8wdkRWNFR5NHo3K3lSS1U0clZvZFNBZWZIN3lqeitLV1RRck96L0lHU2NwCmV1YTdqV0hRMDdMYWxyTjV2b0tFaU1JM3MrWjhzeUdVUGVyYXQwdzJMWlc3NnhxVGl4R002clZxUldxVlQ4L1oKQTJMMEc4WGRvNTZvV2lFYVF5RkJtRDFnMXU2UEsvTmFGVDI1L2tTNWJ1dnF5L1dLVGt0UVNhNHNZc1ZLbUlQTQp0Zys0NUZ2aFErNkRuQzd0TmVnaTZDTkdTb0w0R1dPOEE5UDZRNjE5RkJJZ1VjcGpFMTgvUHpQOEJmcTAxajhnCjZmdm1jNkVPMkxHVHhDcW1DbVp0TnI3OCtQaUxkMHZIY3pqY3E3NzhiNW5WRXRpUVNRQkUyb0ozTVlIZUFIUUkKYVFJREFRQUJvMU13VVRBZEJnTlZIUTRFRmdRVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdId1lEVlIwagpCQmd3Rm9BVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdEd1lEVlIwVEFRSC9CQVV3QXdFQi96QU5CZ2txCmhraUc5dzBCQVFzRkFBT0NBZ0VBQlhNSlU2MjJZVFZVNnZ1K2svNnkwMGNaWlRmVnZtdVJMOXhTcWxVM0I1QmQKVWdyVWx1TmdjN2dhUUlrYzkvWmh2MnhNd0xxUldMWEhiTWx1NkNvdkNiVTVpeWt0NHVWMnl5UzlZYWhmVVRNVQo3TVE0WFRta2hoS0dGbWZBQ2QzTUVwRE55T3hmWXh0UVBwM1NZT2IxRGFKMmUwY01Gc081bytORGQ5aFVBVzFoCjFLMjMwQnZzYldYYVo4MStIdTU4U1BsYTM5R3FMTG85MzR6dEs4WkRWNFRGTVJxMnNVQ1cxcWFidDh5ejd2RzAKSGV3dXdxelRwR1lTSFI1U0ZvMm45R0xKVUN4SnhxcDlOWVJjMlhUdXRUdkJESzVPMXFZZEJaQzd6cmcxSnczawp2SjI4UGx2TzBQRE42ZVlUdElJdC9yU05ZbW56eVVNRTRYREt0di9KRitLZWZNSWxDTkpzZDRHYXVTdlo5M1NOClhINmcrNEZvRkp4UzNxRmZ0WEc4czNRNnppNzNLRzh5UHZVNHU0WmZNRGd2aG92L0V5YkNLWUpFdVVZSlJWNGEKbmc3cWh3NDBabXQ0eWNCRzU5a2tFSGhNYWtxTWpPaUNkV2x4MEVjZXIxcEFGT1pqN3o1NktURXIxa0ZwUHVaRApjVER5SnNwTjh6dm9CQ0l1ancvQjR6S3kyWStOQitRR1p3dXhyTk9mRGR6ek9yQUE1Ym9OS2gwUUh4c0RxNTExClFaU3hCR21EcGJzN2QzMUQvQll3WEhIUWdwb3FoVUU5dFBGSThpN0pkM2FyeXZCdHlnTWlxSmt1VlRFVk1Ta0UKNTZ0VnFsMjlXenFhRXNrbDN3VUlmczVKKzN3RzRPcWNxRDdXaGQxWUtnc0VUMjdFTWlqVXZIYzQ4TXE0bU1rPQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster OIDC can be imported using the tenant `service_name` and cluster id `kube_id` separated by "/" E.g.,
 
         bash
 
@@ -448,15 +446,14 @@
                  args: KubeOidcArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an OIDC configuration in an OVHcloud Managed Kubernetes cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oidc = ovh.cloud_project.KubeOidc("my-oidc",
             service_name=var["projectid"],
             kube_id=ovh_cloud_project_kube["mykube"]["id"],
@@ -466,15 +463,14 @@
             oidc_username_prefix="ovh:",
             oidc_groups_claims=["groups"],
             oidc_groups_prefix="ovh:",
             oidc_required_claims=["claim1=val1"],
             oidc_signing_algs=["RS512"],
             oidc_ca_content="LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZhekNDQTFPZ0F3SUJBZ0lVYm9YRkZrL1hCQmdQUUI4UHlqbkttUGVWekNjd0RRWUpLb1pJaHZjTkFRRUwKQlFBd1JURUxNQWtHQTFVRUJoTUNRVlV4RXpBUkJnTlZCQWdNQ2xOdmJXVXRVM1JoZEdVeElUQWZCZ05WQkFvTQpHRWx1ZEdWeWJtVjBJRmRwWkdkcGRITWdVSFI1SUV4MFpEQWVGdzB5TWpFd01UUXdOalE0TlROYUZ3MHlNekV3Ck1UUXdOalE0TlROYU1FVXhDekFKQmdOVkJBWVRBa0ZWTVJNd0VRWURWUVFJREFwVGIyMWxMVk4wWVhSbE1TRXcKSHdZRFZRUUtEQmhKYm5SbGNtNWxkQ0JYYVdSbmFYUnpJRkIwZVNCTWRHUXdnZ0lpTUEwR0NTcUdTSWIzRFFFQgpBUVVBQTRJQ0R3QXdnZ0lLQW9JQ0FRQytPMk53bGx2QTQyT05SUHMyZWlqTUp2UHhpN21RblVSS3FrOHJEV1VkCkwzZU0yM1JXeVhtS1AydDQ5Zi9LVGsweEZNVStOSTUzTEhwWmh6N3NpK3dEUFUvWWZWSS9rQmZsRm8zeVZCMSsKZWdCSnpyNGIrQ3FoaWlCUkh0Vm5LblFKUmdvOVJjVkxhRm82UEY0N1V0UWJ2bWVuNGdERnExVkYwVHhUdnFMdwpIMzRZL0U2QUJsSlZnWFBzaWQzNm54eTErNnlKV05vRXNVekFiekpWMHhzTGhxc2hOazA0TWx4YnBhcG1XcEUxCmFFMHRIZGpjUlI3Y1dTRUUwMnRSQzNYL2tSNjBKb3MxR0N0Y0ZQTTVIN3NjOFBXNFRUem1EWWhOeDRiVjV4T28KU0xYRnI5ajBzZEgxbm1wSlI1dWxJT2dPTWV3MHA2d3JOYVV2MGpxc1hzdVdqMVpxdTRLRi81aEQ3azVhRlhKNQpjYWNTUi9mRWxreW1uZis0eHZFOG8wdkRWNFR5NHo3K3lSS1U0clZvZFNBZWZIN3lqeitLV1RRck96L0lHU2NwCmV1YTdqV0hRMDdMYWxyTjV2b0tFaU1JM3MrWjhzeUdVUGVyYXQwdzJMWlc3NnhxVGl4R002clZxUldxVlQ4L1oKQTJMMEc4WGRvNTZvV2lFYVF5RkJtRDFnMXU2UEsvTmFGVDI1L2tTNWJ1dnF5L1dLVGt0UVNhNHNZc1ZLbUlQTQp0Zys0NUZ2aFErNkRuQzd0TmVnaTZDTkdTb0w0R1dPOEE5UDZRNjE5RkJJZ1VjcGpFMTgvUHpQOEJmcTAxajhnCjZmdm1jNkVPMkxHVHhDcW1DbVp0TnI3OCtQaUxkMHZIY3pqY3E3NzhiNW5WRXRpUVNRQkUyb0ozTVlIZUFIUUkKYVFJREFRQUJvMU13VVRBZEJnTlZIUTRFRmdRVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdId1lEVlIwagpCQmd3Rm9BVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdEd1lEVlIwVEFRSC9CQVV3QXdFQi96QU5CZ2txCmhraUc5dzBCQVFzRkFBT0NBZ0VBQlhNSlU2MjJZVFZVNnZ1K2svNnkwMGNaWlRmVnZtdVJMOXhTcWxVM0I1QmQKVWdyVWx1TmdjN2dhUUlrYzkvWmh2MnhNd0xxUldMWEhiTWx1NkNvdkNiVTVpeWt0NHVWMnl5UzlZYWhmVVRNVQo3TVE0WFRta2hoS0dGbWZBQ2QzTUVwRE55T3hmWXh0UVBwM1NZT2IxRGFKMmUwY01Gc081bytORGQ5aFVBVzFoCjFLMjMwQnZzYldYYVo4MStIdTU4U1BsYTM5R3FMTG85MzR6dEs4WkRWNFRGTVJxMnNVQ1cxcWFidDh5ejd2RzAKSGV3dXdxelRwR1lTSFI1U0ZvMm45R0xKVUN4SnhxcDlOWVJjMlhUdXRUdkJESzVPMXFZZEJaQzd6cmcxSnczawp2SjI4UGx2TzBQRE42ZVlUdElJdC9yU05ZbW56eVVNRTRYREt0di9KRitLZWZNSWxDTkpzZDRHYXVTdlo5M1NOClhINmcrNEZvRkp4UzNxRmZ0WEc4czNRNnppNzNLRzh5UHZVNHU0WmZNRGd2aG92L0V5YkNLWUpFdVVZSlJWNGEKbmc3cWh3NDBabXQ0eWNCRzU5a2tFSGhNYWtxTWpPaUNkV2x4MEVjZXIxcEFGT1pqN3o1NktURXIxa0ZwUHVaRApjVER5SnNwTjh6dm9CQ0l1ancvQjR6S3kyWStOQitRR1p3dXhyTk9mRGR6ek9yQUE1Ym9OS2gwUUh4c0RxNTExClFaU3hCR21EcGJzN2QzMUQvQll3WEhIUWdwb3FoVUU5dFBGSThpN0pkM2FyeXZCdHlnTWlxSmt1VlRFVk1Ta0UKNTZ0VnFsMjlXenFhRXNrbDN3VUlmczVKKzN3RzRPcWNxRDdXaGQxWUtnc0VUMjdFTWlqVXZIYzQ4TXE0bU1rPQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kubernetes Service cluster OIDC can be imported using the tenant `service_name` and cluster id `kube_id` separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/network_private.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/network_private.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,27 +259,25 @@
                  vlan_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Creates a private network in a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         net = ovh.cloud_project.NetworkPrivate("net",
             regions=[
                 "GRA1",
                 "BHS1",
             ],
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Private network in a public cloud project can be imported using the `service_name` and the `network_id`, separated by "/" E.g.,
 
         bash
 
@@ -304,27 +302,25 @@
                  args: NetworkPrivateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a private network in a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         net = ovh.cloud_project.NetworkPrivate("net",
             regions=[
                 "GRA1",
                 "BHS1",
             ],
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Private network in a public cloud project can be imported using the `service_name` and the `network_id`, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/network_private_subnet.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/network_private_subnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,30 +388,28 @@
                  start: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a subnet in a private network of a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
             dhcp=True,
             end="192.168.168.200",
             network="192.168.168.0/24",
             network_id="0234543",
             no_gateway=False,
             region="GRA1",
             service_name="xxxxx",
             start="192.168.168.100")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
 
         bash
 
@@ -446,30 +444,28 @@
                  args: NetworkPrivateSubnetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a subnet in a private network of a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
             dhcp=True,
             end="192.168.168.200",
             network="192.168.168.0/24",
             network_id="0234543",
             no_gateway=False,
             region="GRA1",
             service_name="xxxxx",
             start="192.168.168.100")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     'AlertingFormattedMonthlyThreshold',
     'ContainerRegistryPlan',
     'ContainerRegistryPlanFeature',
     'ContainerRegistryPlanRegistryLimit',
     'DatabaseEndpoint',
     'DatabaseIpRestriction',
     'DatabaseNode',
+    'GatewayExternalInformation',
+    'GatewayExternalInformationIp',
+    'GatewayInterface',
     'KubeCustomization',
     'KubeCustomizationApiserver',
     'KubeCustomizationApiserverAdmissionplugin',
     'KubeCustomizationKubeProxy',
     'KubeCustomizationKubeProxyIptables',
     'KubeCustomizationKubeProxyIpvs',
     'KubeKubeconfigAttribute',
@@ -529,14 +532,184 @@
         """
         Private subnet ID in which the node is.
         """
         return pulumi.get(self, "subnet_id")
 
 
 @pulumi.output_type
+class GatewayExternalInformation(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "networkId":
+            suggest = "network_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in GatewayExternalInformation. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        GatewayExternalInformation.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        GatewayExternalInformation.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ips: Optional[Sequence['outputs.GatewayExternalInformationIp']] = None,
+                 network_id: Optional[str] = None):
+        """
+        :param Sequence['GatewayExternalInformationIpArgs'] ips: List of external ips of the gateway.
+        :param str network_id: ID of the private network.
+        """
+        if ips is not None:
+            pulumi.set(__self__, "ips", ips)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
+
+    @property
+    @pulumi.getter
+    def ips(self) -> Optional[Sequence['outputs.GatewayExternalInformationIp']]:
+        """
+        List of external ips of the gateway.
+        """
+        return pulumi.get(self, "ips")
+
+    @property
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[str]:
+        """
+        ID of the private network.
+        """
+        return pulumi.get(self, "network_id")
+
+
+@pulumi.output_type
+class GatewayExternalInformationIp(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "subnetId":
+            suggest = "subnet_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in GatewayExternalInformationIp. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        GatewayExternalInformationIp.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        GatewayExternalInformationIp.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ip: Optional[str] = None,
+                 subnet_id: Optional[str] = None):
+        """
+        :param str ip: IP of the interface.
+        :param str subnet_id: ID of the subnet.
+        """
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if subnet_id is not None:
+            pulumi.set(__self__, "subnet_id", subnet_id)
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[str]:
+        """
+        IP of the interface.
+        """
+        return pulumi.get(self, "ip")
+
+    @property
+    @pulumi.getter(name="subnetId")
+    def subnet_id(self) -> Optional[str]:
+        """
+        ID of the subnet.
+        """
+        return pulumi.get(self, "subnet_id")
+
+
+@pulumi.output_type
+class GatewayInterface(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "networkId":
+            suggest = "network_id"
+        elif key == "subnetId":
+            suggest = "subnet_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in GatewayInterface. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        GatewayInterface.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        GatewayInterface.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 ip: Optional[str] = None,
+                 network_id: Optional[str] = None,
+                 subnet_id: Optional[str] = None):
+        """
+        :param str id: ID of the interface.
+        :param str ip: IP of the interface.
+        :param str network_id: ID of the private network.
+        :param str subnet_id: ID of the subnet.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
+        if subnet_id is not None:
+            pulumi.set(__self__, "subnet_id", subnet_id)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        ID of the interface.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[str]:
+        """
+        IP of the interface.
+        """
+        return pulumi.get(self, "ip")
+
+    @property
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[str]:
+        """
+        ID of the private network.
+        """
+        return pulumi.get(self, "network_id")
+
+    @property
+    @pulumi.getter(name="subnetId")
+    def subnet_id(self) -> Optional[str]:
+        """
+        ID of the subnet.
+        """
+        return pulumi.get(self, "subnet_id")
+
+
+@pulumi.output_type
 class KubeCustomization(dict):
     def __init__(__self__, *,
                  apiservers: Optional[Sequence['outputs.KubeCustomizationApiserver']] = None):
         """
         :param Sequence['KubeCustomizationApiserverArgs'] apiservers: Kubernetes API server customization
         """
         if apiservers is not None:
@@ -574,37 +747,27 @@
 
 
 @pulumi.output_type
 class KubeCustomizationApiserverAdmissionplugin(dict):
     def __init__(__self__, *,
                  disableds: Optional[Sequence[str]] = None,
                  enableds: Optional[Sequence[str]] = None):
-        """
-        :param Sequence[str] disableds: Array of admission plugins disabled, default is [] and only AlwaysPulImages can be disabled at this time.
-        :param Sequence[str] enableds: Array of admission plugins enabled, default is ["NodeRestriction","AlwaysPulImages"] and only these admission plugins can be enabled at this time.
-        """
         if disableds is not None:
             pulumi.set(__self__, "disableds", disableds)
         if enableds is not None:
             pulumi.set(__self__, "enableds", enableds)
 
     @property
     @pulumi.getter
     def disableds(self) -> Optional[Sequence[str]]:
-        """
-        Array of admission plugins disabled, default is [] and only AlwaysPulImages can be disabled at this time.
-        """
         return pulumi.get(self, "disableds")
 
     @property
     @pulumi.getter
     def enableds(self) -> Optional[Sequence[str]]:
-        """
-        Array of admission plugins enabled, default is ["NodeRestriction","AlwaysPulImages"] and only these admission plugins can be enabled at this time.
-        """
         return pulumi.get(self, "enableds")
 
 
 @pulumi.output_type
 class KubeCustomizationKubeProxy(dict):
     def __init__(__self__, *,
                  iptables: Optional['outputs.KubeCustomizationKubeProxyIptables'] = None,
@@ -655,37 +818,27 @@
     def get(self, key: str, default = None) -> Any:
         KubeCustomizationKubeProxyIptables.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  min_sync_period: Optional[str] = None,
                  sync_period: Optional[str] = None):
-        """
-        :param str min_sync_period: Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        :param str sync_period: Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         if min_sync_period is not None:
             pulumi.set(__self__, "min_sync_period", min_sync_period)
         if sync_period is not None:
             pulumi.set(__self__, "sync_period", sync_period)
 
     @property
     @pulumi.getter(name="minSyncPeriod")
     def min_sync_period(self) -> Optional[str]:
-        """
-        Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        """
         return pulumi.get(self, "min_sync_period")
 
     @property
     @pulumi.getter(name="syncPeriod")
     def sync_period(self) -> Optional[str]:
-        """
-        Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         return pulumi.get(self, "sync_period")
 
 
 @pulumi.output_type
 class KubeCustomizationKubeProxyIpvs(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -715,22 +868,14 @@
     def __init__(__self__, *,
                  min_sync_period: Optional[str] = None,
                  scheduler: Optional[str] = None,
                  sync_period: Optional[str] = None,
                  tcp_fin_timeout: Optional[str] = None,
                  tcp_timeout: Optional[str] = None,
                  udp_timeout: Optional[str] = None):
-        """
-        :param str min_sync_period: Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        :param str scheduler: IPVS scheduler.
-        :param str sync_period: Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        :param str tcp_fin_timeout: Timeout value used for IPVS TCP sessions after receiving a FIN in RFC3339 duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        :param str tcp_timeout: Timeout value used for idle IPVS TCP sessions in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        :param str udp_timeout: timeout value used for IPVS UDP packets in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         if min_sync_period is not None:
             pulumi.set(__self__, "min_sync_period", min_sync_period)
         if scheduler is not None:
             pulumi.set(__self__, "scheduler", scheduler)
         if sync_period is not None:
             pulumi.set(__self__, "sync_period", sync_period)
         if tcp_fin_timeout is not None:
@@ -739,57 +884,39 @@
             pulumi.set(__self__, "tcp_timeout", tcp_timeout)
         if udp_timeout is not None:
             pulumi.set(__self__, "udp_timeout", udp_timeout)
 
     @property
     @pulumi.getter(name="minSyncPeriod")
     def min_sync_period(self) -> Optional[str]:
-        """
-        Minimum period that IPVS rules are refreshed in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`).
-        """
         return pulumi.get(self, "min_sync_period")
 
     @property
     @pulumi.getter
     def scheduler(self) -> Optional[str]:
-        """
-        IPVS scheduler.
-        """
         return pulumi.get(self, "scheduler")
 
     @property
     @pulumi.getter(name="syncPeriod")
     def sync_period(self) -> Optional[str]:
-        """
-        Minimum period that IPVS rules are refreshed, in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration format (e.g. `PT60S`).
-        """
         return pulumi.get(self, "sync_period")
 
     @property
     @pulumi.getter(name="tcpFinTimeout")
     def tcp_fin_timeout(self) -> Optional[str]:
-        """
-        Timeout value used for IPVS TCP sessions after receiving a FIN in RFC3339 duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "tcp_fin_timeout")
 
     @property
     @pulumi.getter(name="tcpTimeout")
     def tcp_timeout(self) -> Optional[str]:
-        """
-        Timeout value used for idle IPVS TCP sessions in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "tcp_timeout")
 
     @property
     @pulumi.getter(name="udpTimeout")
     def udp_timeout(self) -> Optional[str]:
-        """
-        timeout value used for IPVS UDP packets in [RFC3339](https://www.rfc-editor.org/rfc/rfc3339) duration (e.g. `PT60S`). The default value is `PT0S`, which preserves the current timeout value on the system.
-        """
         return pulumi.get(self, "udp_timeout")
 
 
 @pulumi.output_type
 class KubeKubeconfigAttribute(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -867,102 +994,102 @@
 
 @pulumi.output_type
 class KubeNodePoolTemplate(dict):
     def __init__(__self__, *,
                  metadata: 'outputs.KubeNodePoolTemplateMetadata',
                  spec: 'outputs.KubeNodePoolTemplateSpec'):
         """
-        :param 'KubeNodePoolTemplateMetadataArgs' metadata: Metadata of each node in the pool
-        :param 'KubeNodePoolTemplateSpecArgs' spec: Spec of each node in the pool
+        :param 'KubeNodePoolTemplateMetadataArgs' metadata: metadata
+        :param 'KubeNodePoolTemplateSpecArgs' spec: spec
         """
         pulumi.set(__self__, "metadata", metadata)
         pulumi.set(__self__, "spec", spec)
 
     @property
     @pulumi.getter
     def metadata(self) -> 'outputs.KubeNodePoolTemplateMetadata':
         """
-        Metadata of each node in the pool
+        metadata
         """
         return pulumi.get(self, "metadata")
 
     @property
     @pulumi.getter
     def spec(self) -> 'outputs.KubeNodePoolTemplateSpec':
         """
-        Spec of each node in the pool
+        spec
         """
         return pulumi.get(self, "spec")
 
 
 @pulumi.output_type
 class KubeNodePoolTemplateMetadata(dict):
     def __init__(__self__, *,
                  annotations: Mapping[str, str],
                  finalizers: Sequence[str],
                  labels: Mapping[str, str]):
         """
-        :param Mapping[str, str] annotations: Annotations to apply to each node
-        :param Sequence[str] finalizers: Finalizers to apply to each node. A finalizer name must be fully qualified, e.g. kubernetes.io/pv-protection , where you prefix it with hostname of your service which is related to the controller responsible for the finalizer.
-        :param Mapping[str, str] labels: Labels to apply to each node
+        :param Mapping[str, str] annotations: annotations
+        :param Sequence[str] finalizers: finalizers
+        :param Mapping[str, str] labels: labels
         """
         pulumi.set(__self__, "annotations", annotations)
         pulumi.set(__self__, "finalizers", finalizers)
         pulumi.set(__self__, "labels", labels)
 
     @property
     @pulumi.getter
     def annotations(self) -> Mapping[str, str]:
         """
-        Annotations to apply to each node
+        annotations
         """
         return pulumi.get(self, "annotations")
 
     @property
     @pulumi.getter
     def finalizers(self) -> Sequence[str]:
         """
-        Finalizers to apply to each node. A finalizer name must be fully qualified, e.g. kubernetes.io/pv-protection , where you prefix it with hostname of your service which is related to the controller responsible for the finalizer.
+        finalizers
         """
         return pulumi.get(self, "finalizers")
 
     @property
     @pulumi.getter
     def labels(self) -> Mapping[str, str]:
         """
-        Labels to apply to each node
+        labels
         """
         return pulumi.get(self, "labels")
 
 
 @pulumi.output_type
 class KubeNodePoolTemplateSpec(dict):
     def __init__(__self__, *,
                  taints: Sequence[Mapping[str, Any]],
                  unschedulable: bool):
         """
-        :param Sequence[Mapping[str, Any]] taints: Taints to apply to each node [NodeSpec kubernetes documentation](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1/#NodeSpec)
-        :param bool unschedulable: If true, set nodes as un-schedulable
+        :param Sequence[Mapping[str, Any]] taints: taints
+        :param bool unschedulable: unschedulable
         """
         pulumi.set(__self__, "taints", taints)
         pulumi.set(__self__, "unschedulable", unschedulable)
 
     @property
     @pulumi.getter
     def taints(self) -> Sequence[Mapping[str, Any]]:
         """
-        Taints to apply to each node [NodeSpec kubernetes documentation](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1/#NodeSpec)
+        taints
         """
         return pulumi.get(self, "taints")
 
     @property
     @pulumi.getter
     def unschedulable(self) -> bool:
         """
-        If true, set nodes as un-schedulable
+        unschedulable
         """
         return pulumi.get(self, "unschedulable")
 
 
 @pulumi.output_type
 class KubePrivateNetworkConfiguration(dict):
     @staticmethod
@@ -988,19 +1115,17 @@
                  default_vrack_gateway: str,
                  private_network_routing_as_default: bool):
         """
         :param str default_vrack_gateway: If defined, all egress traffic will be routed towards this IP address, which should belong to the private network. Empty string means disabled.
         :param bool private_network_routing_as_default: Defines whether routing should default to using the nodes' private interface, instead of their public interface. Default is false.
                
                In order to use the gateway IP advertised by the private network subnet DHCP, the following configuration shall be used.
-               <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                ```
-               <!--End PulumiCodeChooser -->
         """
         pulumi.set(__self__, "default_vrack_gateway", default_vrack_gateway)
         pulumi.set(__self__, "private_network_routing_as_default", private_network_routing_as_default)
 
     @property
     @pulumi.getter(name="defaultVrackGateway")
     def default_vrack_gateway(self) -> str:
@@ -1012,19 +1137,17 @@
     @property
     @pulumi.getter(name="privateNetworkRoutingAsDefault")
     def private_network_routing_as_default(self) -> bool:
         """
         Defines whether routing should default to using the nodes' private interface, instead of their public interface. Default is false.
 
         In order to use the gateway IP advertised by the private network subnet DHCP, the following configuration shall be used.
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         ```
-        <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "private_network_routing_as_default")
 
 
 @pulumi.output_type
 class NetworkPrivateRegionsAttribute(dict):
     def __init__(__self__, *,
@@ -1337,15 +1460,15 @@
                  duration: str,
                  plan_code: str,
                  pricing_mode: str,
                  catalog_name: Optional[str] = None,
                  configurations: Optional[Sequence['outputs.ProjectPlanConfiguration']] = None):
         """
         :param str duration: duration
-        :param str plan_code: Plan code
+        :param str plan_code: Plan code. This value must be adapted depending on your `OVH_ENDPOINT` value. It's `project.2018` for `ovh-{eu,ca}` and `project` when using `ovh-us`.
         :param str pricing_mode: Pricing model identifier
         :param str catalog_name: Catalog name
         :param Sequence['ProjectPlanConfigurationArgs'] configurations: Representation of a configuration item for personalizing product
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
@@ -1362,15 +1485,15 @@
         """
         return pulumi.get(self, "duration")
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> str:
         """
-        Plan code
+        Plan code. This value must be adapted depending on your `OVH_ENDPOINT` value. It's `project.2018` for `ovh-{eu,ca}` and `project` when using `ovh-us`.
         """
         return pulumi.get(self, "plan_code")
 
     @property
     @pulumi.getter(name="pricingMode")
     def pricing_mode(self) -> str:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/project.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 
 @pulumi.input_type
 class ProjectArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['ProjectPlanArgs'],
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectPlanOptionArgs']]]] = None):
         """
         The set of arguments for constructing a Project resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['ProjectPlanArgs'] plan: Product Plan to order
         :param pulumi.Input[str] description: A description associated with the user.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectOrderArgs']]] orders: Details about the order that was used to create the public cloud project
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['ProjectPlanOptionArgs']]] plan_options: Product Plan to order
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -74,14 +78,26 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectOrderArgs']]]]:
+        """
+        Details about the order that was used to create the public cloud project
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -293,14 +309,15 @@
 
 class Project(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['ProjectPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectPlanOptionArgs']]]]] = None,
                  __props__=None):
         """
         ## Import
@@ -312,14 +329,15 @@
         ```sh
         $ pulumi import ovh:CloudProject/project:Project my_cloud_project order_id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description associated with the user.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectOrderArgs']]]] orders: Details about the order that was used to create the public cloud project
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['ProjectPlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectPlanOptionArgs']]]] plan_options: Product Plan to order
         """
         ...
     @overload
@@ -350,39 +368,40 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['ProjectPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectPlanOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
             __props__.__dict__["description"] = description
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
             __props__.__dict__["plan_options"] = plan_options
             __props__.__dict__["project_urn"] = None
             __props__.__dict__["access"] = None
-            __props__.__dict__["orders"] = None
             __props__.__dict__["project_id"] = None
             __props__.__dict__["project_name"] = None
             __props__.__dict__["status"] = None
         super(Project, __self__).__init__(
             'ovh:CloudProject/project:Project',
             resource_name,
             __props__,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/region_storage_presign.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/region_storage_presign.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,28 +253,26 @@
         """
         Generates a temporary presigned S3 URLs to download or upload an object.
 
         > __NOTE__ This resource is only compatible with the `High Performance - S3` solution for object storage.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         presigned_url_region_storage_presign = ovh.cloud_project.RegionStoragePresign("presignedUrlRegionStoragePresign",
             service_name="xxxxxxxxxxxxxxxxx",
             region_name="GRA",
             expire=3600,
             method="GET",
             object="an-object-in-the-bucket")
         pulumi.export("presignedUrl", presigned_url_region_storage_presign.url)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] expire: Define, in seconds, for how long your URL will be valid.
         :param pulumi.Input[str] method: The method you want to use to interact with your object. Can be either 'GET' or 'PUT'.
         :param pulumi.Input[str] name: The name of your S3 storage container/bucket.
         :param pulumi.Input[str] object: The name of the object in your S3 bucket.
@@ -292,28 +290,26 @@
         """
         Generates a temporary presigned S3 URLs to download or upload an object.
 
         > __NOTE__ This resource is only compatible with the `High Performance - S3` solution for object storage.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         presigned_url_region_storage_presign = ovh.cloud_project.RegionStoragePresign("presignedUrlRegionStoragePresign",
             service_name="xxxxxxxxxxxxxxxxx",
             region_name="GRA",
             expire=3600,
             method="GET",
             object="an-object-in-the-bucket")
         pulumi.export("presignedUrl", presigned_url_region_storage_presign.url)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RegionStoragePresignArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/s3_credential.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/s3_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/s3_policy.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/s3_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,14 @@
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Set the S3 Policy of a public cloud project user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ovh as ovh
 
         user = ovh.cloud_project.User("user",
             service_name="XXX",
@@ -171,15 +170,14 @@
                     "Resource": [
                         "arn:aws:s3:::hp-bucket",
                         "arn:aws:s3:::hp-bucket/*",
                     ],
                 }],
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud User S3 Policy can be imported using the `service_name`, `user_id` of the policy, separated by "/" E.g.,
 
         bash
 
@@ -201,15 +199,14 @@
                  args: S3PolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Set the S3 Policy of a public cloud project user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ovh as ovh
 
         user = ovh.cloud_project.User("user",
             service_name="XXX",
@@ -238,15 +235,14 @@
                     "Resource": [
                         "arn:aws:s3:::hp-bucket",
                         "arn:aws:s3:::hp-bucket/*",
                     ],
                 }],
             }))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud User S3 Policy can be imported using the `service_name`, `user_id` of the policy, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,22 +342,20 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a user in a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user1 = ovh.cloud_project.User("user1", service_name="XXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description associated with the user.
         :param pulumi.Input[Mapping[str, Any]] openstack_rc: a convenient map representing an openstack_rc file.
                Note: no password nor sensitive token is set in this map.
         :param pulumi.Input[str] role_name: The name of a role. See `role_names`.
@@ -384,22 +382,20 @@
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a user in a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user1 = ovh.cloud_project.User("user1", service_name="XXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudproject/workflow_backup.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudproject/workflow_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,28 +298,26 @@
                  __props__=None):
         """
         Manage a worflow that schedules backups of public cloud instance.
         Note that upon deletion, the workflow is deleted but any backups that have been created by this workflow are not.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_backup = ovh.cloud_project.WorkflowBackup("myBackup",
             cron="50 4 * * *",
             instance_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
             max_execution_count=0,
             region_name="GRA11",
             rotation=7,
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] backup_name: The name of the backup files that are created. If empty, the `name` attribute is used.
         :param pulumi.Input[str] cron: The cron periodicity at which the backup workflow is scheduled
         :param pulumi.Input[int] max_execution_count: The number of times the worflow is run. Default value is `0` which means that the workflow will be scheduled continously until its deletion
         :param pulumi.Input[str] name: The worflow name that is used in the UI
@@ -335,28 +333,26 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage a worflow that schedules backups of public cloud instance.
         Note that upon deletion, the workflow is deleted but any backups that have been created by this workflow are not.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_backup = ovh.cloud_project.WorkflowBackup("myBackup",
             cron="50 4 * * *",
             instance_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx",
             max_execution_count=0,
             region_name="GRA11",
             rotation=7,
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param WorkflowBackupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/database_instance.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/database_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,28 +192,26 @@
         With this resource you can create a database for the following database engine:
 
           * `mysql`
           * `postgresql`
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         db = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="YYYY",
             id="ZZZZ")
         database = ovh.cloud_project_database.DatabaseInstance("database",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters databases can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the database, separated by "/" E.g.,
 
         bash
 
@@ -242,28 +240,26 @@
         With this resource you can create a database for the following database engine:
 
           * `mysql`
           * `postgresql`
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         db = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="YYYY",
             id="ZZZZ")
         database = ovh.cloud_project_database.DatabaseInstance("database",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters databases can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the database, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_capabilities.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_certificates.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,25 +97,23 @@
                      service_name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCertificatesResult:
     """
     Use this data source to get information about certificates of a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     certificates = ovh.CloudProjectDatabase.get_certificates(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("certificatesCa", certificates.ca)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want database information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str service_name: The id of the public cloud project. If omitted,
@@ -142,25 +140,23 @@
                             service_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCertificatesResult]:
     """
     Use this data source to get information about certificates of a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     certificates = ovh.CloudProjectDatabase.get_certificates(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("certificatesCa", certificates.ca)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want database information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str service_name: The id of the public cloud project. If omitted,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,25 +301,23 @@
     """
     Use this data source to get the managed database of a public cloud project.
 
     ## Example Usage
 
     To get information of a database cluster service:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     db = ovh.CloudProjectDatabase.get_database(service_name="XXXXXX",
         engine="YYYY",
         id="ZZZZ")
     pulumi.export("clusterId", db.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str engine: The database engine you want to get information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
@@ -364,25 +362,23 @@
     """
     Use this data source to get the managed database of a public cloud project.
 
     ## Example Usage
 
     To get information of a database cluster service:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     db = ovh.CloudProjectDatabase.get_database(service_name="XXXXXX",
         engine="YYYY",
         id="ZZZZ")
     pulumi.export("clusterId", db.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str engine: The database engine you want to get information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_instance.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,26 +110,24 @@
                           service_name: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseInstanceResult:
     """
     Use this data source to get information about a database of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     database = ovh.CloudProjectDatabase.get_database_instance(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         name="UUU")
     pulumi.export("databaseName", database.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want database information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str name: Name of the database.
@@ -160,26 +158,24 @@
                                  service_name: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseInstanceResult]:
     """
     Use this data source to get information about a database of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     database = ovh.CloudProjectDatabase.get_database_instance(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         name="UUU")
     pulumi.export("databaseName", database.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want database information. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str name: Name of the database.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_instances.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,25 +97,23 @@
                            service_name: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseInstancesResult:
     """
     Use this data source to get the list of databases of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     databases = ovh.CloudProjectDatabase.get_database_instances(service_name="XXXX",
         engine="YYYY",
         cluster_id="ZZZ")
     pulumi.export("databaseIds", databases.database_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list databases. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str service_name: The id of the public cloud project. If omitted,
@@ -142,25 +140,23 @@
                                   service_name: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseInstancesResult]:
     """
     Use this data source to get the list of databases of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     databases = ovh.CloudProjectDatabase.get_database_instances(service_name="XXXX",
         engine="YYYY",
         cluster_id="ZZZ")
     pulumi.export("databaseIds", databases.database_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list databases. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str service_name: The id of the public cloud project. If omitted,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_integration.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,26 +146,24 @@
                              service_name: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseIntegrationResult:
     """
     Use this data source to get information about an integration of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     integration = ovh.CloudProjectDatabase.get_database_integration(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         id="UUU")
     pulumi.export("integrationType", integration.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            All engines available exept `mongodb`
     :param str id: Integration ID
     :param str service_name: The id of the public cloud project. If omitted,
@@ -198,26 +196,24 @@
                                     service_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseIntegrationResult]:
     """
     Use this data source to get information about an integration of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     integration = ovh.CloudProjectDatabase.get_database_integration(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         id="UUU")
     pulumi.export("integrationType", integration.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            All engines available exept `mongodb`
     :param str id: Integration ID
     :param str service_name: The id of the public cloud project. If omitted,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,25 +97,23 @@
                               service_name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseIntegrationsResult:
     """
     Use this data source to get the list of integrations of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     integrations = ovh.CloudProjectDatabase.get_database_integrations(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("integrationIds", integrations.integration_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list integrations. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            All engines available exept `mongodb`
     :param str service_name: The id of the public cloud project. If omitted,
@@ -142,25 +140,23 @@
                                      service_name: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseIntegrationsResult]:
     """
     Use this data source to get the list of integrations of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     integrations = ovh.CloudProjectDatabase.get_database_integrations(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("integrationIds", integrations.integration_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list integrations. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            All engines available exept `mongodb`
     :param str service_name: The id of the public cloud project. If omitted,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,26 +170,24 @@
                                   service_name: Optional[str] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseLogSubscriptionResult:
     """
     Use this data source to get information about a log subscription for a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     subscription = ovh.CloudProjectDatabase.get_database_log_subscription(service_name="VVV",
         engine="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("subscriptionLdpName", subscription.ldp_service_name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The database engine for which you want to retrieve a subscription. To get a full list of available engine visit.
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str id: Id of the log subscription.
     :param str service_name: The id of the public cloud project. If omitted,
@@ -224,26 +222,24 @@
                                          service_name: Optional[pulumi.Input[str]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseLogSubscriptionResult]:
     """
     Use this data source to get information about a log subscription for a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     subscription = ovh.CloudProjectDatabase.get_database_log_subscription(service_name="VVV",
         engine="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("subscriptionLdpName", subscription.ldp_service_name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The database engine for which you want to retrieve a subscription. To get a full list of available engine visit.
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str id: Id of the log subscription.
     :param str service_name: The id of the public cloud project. If omitted,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,25 +97,23 @@
                                    service_name: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseLogSubscriptionsResult:
     """
     Use this data source to get the list of log subscrition for a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     subscriptions = ovh.CloudProjectDatabase.get_database_log_subscriptions(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("subscriptionIds", subscriptions.subscription_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The database engine for which you want to retrieve a subscription. To get a full list of available engine visit.
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
@@ -141,25 +139,23 @@
                                           service_name: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseLogSubscriptionsResult]:
     """
     Use this data source to get the list of log subscrition for a cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     subscriptions = ovh.CloudProjectDatabase.get_database_log_subscriptions(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ")
     pulumi.export("subscriptionIds", subscriptions.subscription_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str engine: The database engine for which you want to retrieve a subscription. To get a full list of available engine visit.
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                                               service_name: Optional[str] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabasePostgreSQLConnectionPoolsResult:
     """
     Use this data source to get the list of  connection pools of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     test_pools = ovh.CloudProjectDatabase.get_database_postgre_sql_connection_pools(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("connectionPoolIds", test_pools.connection_pool_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                                                      service_name: Optional[pulumi.Input[str]] = None,
                                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabasePostgreSQLConnectionPoolsResult]:
     """
     Use this data source to get the list of  connection pools of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     test_pools = ovh.CloudProjectDatabase.get_database_postgre_sql_connection_pools(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("connectionPoolIds", test_pools.connection_pool_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_databases.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_databases.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,24 +86,22 @@
     """
     Use this data source to get the list of managed databases of a public cloud project.
 
     ## Example Usage
 
     To get the list of database clusters service for a given engine:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     dbs = ovh.CloudProjectDatabase.get_databases(service_name="XXXXXX",
         engine="YYYY")
     pulumi.export("clusterIds", dbs.cluster_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str engine: The database engine you want to list. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -127,24 +125,22 @@
     """
     Use this data source to get the list of managed databases of a public cloud project.
 
     ## Example Usage
 
     To get the list of database clusters service for a given engine:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     dbs = ovh.CloudProjectDatabase.get_databases(service_name="XXXXXX",
         engine="YYYY")
     pulumi.export("clusterIds", dbs.cluster_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str engine: The database engine you want to list. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,25 +101,23 @@
 
     Use this data source to get the list of IP restrictions associated with a public cloud project.
 
     ## Example Usage
 
     To get the list of IP restriction on a database cluster service:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     iprestrictions = ovh.CloudProjectDatabase.get_ip_restrictions(service_name="XXXXXX",
         engine="YYYY",
         cluster_id="ZZZZ")
     pulumi.export("ips", iprestrictions.ips)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list IP restrictions. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
@@ -149,25 +147,23 @@
 
     Use this data source to get the list of IP restrictions associated with a public cloud project.
 
     ## Example Usage
 
     To get the list of IP restriction on a database cluster service:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     iprestrictions = ovh.CloudProjectDatabase.get_ip_restrictions(service_name="XXXXXX",
         engine="YYYY",
         cluster_id="ZZZZ")
     pulumi.export("ips", iprestrictions.ips)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list IP restrictions. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,25 +109,23 @@
                   service_name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaAclResult:
     """
     Use this data source to get information about an ACL of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     acl = ovh.CloudProjectDatabase.get_kafka_acl(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("aclPermission", acl.permission)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: ACL ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -153,25 +151,23 @@
                          service_name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaAclResult]:
     """
     Use this data source to get information about an ACL of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     acl = ovh.CloudProjectDatabase.get_kafka_acl(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("aclPermission", acl.permission)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: ACL ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                    service_name: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaAclsResult:
     """
     Use this data source to get the list of ACLs of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     acls = ovh.CloudProjectDatabase.get_kafka_acls(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("aclIds", acls.acl_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                           service_name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaAclsResult]:
     """
     Use this data source to get the list of ACLs of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     acls = ovh.CloudProjectDatabase.get_kafka_acls(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("aclIds", acls.acl_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,25 +109,23 @@
                                   service_name: Optional[str] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaSchemaRegistryAclResult:
     """
     Use this data source to get information about a schema registry ACL of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     schema_registry_acl = ovh.CloudProjectDatabase.get_kafka_schema_registry_acl(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("aclPermission", schema_registry_acl.permission)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Schema registry ACL ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -153,25 +151,23 @@
                                          service_name: Optional[pulumi.Input[str]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaSchemaRegistryAclResult]:
     """
     Use this data source to get information about a schema registry ACL of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     schema_registry_acl = ovh.CloudProjectDatabase.get_kafka_schema_registry_acl(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("aclPermission", schema_registry_acl.permission)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Schema registry ACL ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                                    service_name: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaSchemaRegistryAclsResult:
     """
     Use this data source to get the list of ACLs of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     schema_registry_acls = ovh.CloudProjectDatabase.get_kafka_schema_registry_acls(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("aclIds", schema_registry_acls.acl_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                                           service_name: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaSchemaRegistryAclsResult]:
     """
     Use this data source to get the list of ACLs of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     schema_registry_acls = ovh.CloudProjectDatabase.get_kafka_schema_registry_acls(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("aclIds", schema_registry_acls.acl_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,25 +145,23 @@
                     service_name: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaTopicResult:
     """
     Use this data source to get information about a topic of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     topic = ovh.CloudProjectDatabase.get_kafka_topic(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("topicName", topic.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Topic ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -192,25 +190,23 @@
                            service_name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaTopicResult]:
     """
     Use this data source to get information about a topic of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     topic = ovh.CloudProjectDatabase.get_kafka_topic(service_name="XXX",
         cluster_id="YYY",
         id="ZZZ")
     pulumi.export("topicName", topic.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str id: Topic ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,24 +84,22 @@
                      service_name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaTopicsResult:
     """
     Use this data source to get the list of topics of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     topics = ovh.CloudProjectDatabase.get_kafka_topics(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("topicIds", topics.topic_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     __args__ = dict()
@@ -122,24 +120,22 @@
                             service_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaTopicsResult]:
     """
     Use this data source to get the list of topics of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     topics = ovh.CloudProjectDatabase.get_kafka_topics(service_name="XXX",
         cluster_id="YYY")
     pulumi.export("topicIds", topics.topic_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,25 +109,23 @@
                           user_id: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKafkaUserAccessResult:
     """
     Use this data source to get information about user acces of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     access = ovh.CloudProjectDatabase.get_kafka_user_access(service_name="XXX",
         cluster_id="YYY",
         user_id="ZZZ")
     pulumi.export("accessCert", access.cert)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: User ID
     """
@@ -153,25 +151,23 @@
                                  user_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKafkaUserAccessResult]:
     """
     Use this data source to get information about user acces of a kafka cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     access = ovh.CloudProjectDatabase.get_kafka_user_access(service_name="XXX",
         cluster_id="YYY",
         user_id="ZZZ")
     pulumi.export("accessCert", access.cert)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     :param str user_id: User ID
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,14 @@
                                      service_name: Optional[str] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPostgresSqlConnectionPoolResult:
     """
     Use this data source to get information about a connection pool of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     test_pool_postgres_sql_connection_pool = ovh.CloudProjectDatabase.get_postgres_sql_connection_pool(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
@@ -191,15 +190,14 @@
         "size": test_pool_postgres_sql_connection_pool.size,
         "port": test_pool_postgres_sql_connection_pool.port,
         "ssl_mode": test_pool_postgres_sql_connection_pool.ssl_mode,
         "uri": test_pool_postgres_sql_connection_pool.uri,
         "user_id": test_pool_postgres_sql_connection_pool.user_id,
     })
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str name: Name of the Connection pool.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -230,15 +228,14 @@
                                             service_name: Optional[pulumi.Input[str]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPostgresSqlConnectionPoolResult]:
     """
     Use this data source to get information about a connection pool of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     test_pool_postgres_sql_connection_pool = ovh.CloudProjectDatabase.get_postgres_sql_connection_pool(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
@@ -251,15 +248,14 @@
         "size": test_pool_postgres_sql_connection_pool.size,
         "port": test_pool_postgres_sql_connection_pool.port,
         "ssl_mode": test_pool_postgres_sql_connection_pool.ssl_mode,
         "uri": test_pool_postgres_sql_connection_pool.uri,
         "user_id": test_pool_postgres_sql_connection_pool.user_id,
     })
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID.
     :param str name: Name of the Connection pool.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,25 +121,23 @@
                           service_name: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPostgresSqlUserResult:
     """
     Use this data source to get information about a user of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     pguser = ovh.CloudProjectDatabase.get_postgres_sql_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("pguserRoles", pguser.roles)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
@@ -166,25 +164,23 @@
                                  service_name: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPostgresSqlUserResult]:
     """
     Use this data source to get information about a user of a postgresql cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     pguser = ovh.CloudProjectDatabase.get_postgres_sql_user(service_name="XXX",
         cluster_id="YYY",
         name="ZZZ")
     pulumi.export("pguserRoles", pguser.roles)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str name: Name of the user.
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,26 +122,24 @@
              service_name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Use this data source to get information about a user of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user = ovh.CloudProjectDatabase.get_user(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         name="UUU")
     pulumi.export("userName", user.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want user information. To get a full list of available engine visit :
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str name: Name of the user.
@@ -173,26 +171,24 @@
                     service_name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to get information about a user of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user = ovh.CloudProjectDatabase.get_user(service_name="XXX",
         engine="YYY",
         cluster_id="ZZZ",
         name="UUU")
     pulumi.export("userName", user.name)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want user information. To get a full list of available engine visit :
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
            Available engines:
     :param str name: Name of the user.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/get_users.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/get_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,25 +97,23 @@
               service_name: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Use this data source to get the list of users of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     users = ovh.CloudProjectDatabase.get_users(service_name="XXXX",
         engine="YYYY",
         cluster_id="ZZZ")
     pulumi.export("userIds", users.user_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list users. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
@@ -141,25 +139,23 @@
                      service_name: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Use this data source to get the list of users of a database cluster associated with a public cloud project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     users = ovh.CloudProjectDatabase.get_users(service_name="XXXX",
         engine="YYYY",
         cluster_id="ZZZ")
     pulumi.export("userIds", users.user_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID
     :param str engine: The engine of the database cluster you want to list users. To get a full list of available engine visit:
            [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
     :param str service_name: The id of the public cloud project. If omitted,
            the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/integration.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,14 @@
 
         Please take a look at the list of available `types` in the `Argument references` section in order to know the list of avaulable integrations. For example, thanks to the integration feature you can have your PostgreSQL logs in your OpenSearch Database.
 
         ## Example Usage
 
         Push PostgreSQL logs in an OpenSearch DB:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         dbpostgresql = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="postgresql",
             id="ZZZZ")
@@ -313,15 +312,14 @@
             service_name=dbpostgresql.service_name,
             engine=dbpostgresql.engine,
             cluster_id=dbpostgresql.id,
             source_service_id=dbpostgresql.id,
             destination_service_id=dbopensearch.id,
             type="opensearchLogs")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters users can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the user, separated by "/" E.g.,
 
         bash
 
@@ -355,15 +353,14 @@
 
         Please take a look at the list of available `types` in the `Argument references` section in order to know the list of avaulable integrations. For example, thanks to the integration feature you can have your PostgreSQL logs in your OpenSearch Database.
 
         ## Example Usage
 
         Push PostgreSQL logs in an OpenSearch DB:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         dbpostgresql = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="postgresql",
             id="ZZZZ")
@@ -374,15 +371,14 @@
             service_name=dbpostgresql.service_name,
             engine=dbpostgresql.engine,
             cluster_id=dbpostgresql.id,
             source_service_id=dbpostgresql.id,
             destination_service_id=dbopensearch.id,
             type="opensearchLogs")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database clusters users can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the user, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/ip_restriction.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,29 +222,27 @@
         Deprecated: Use ip_restriction field in cloud_project_database resource instead.
         Continuing to use the CloudProjectDatabase.IpRestriction resource to add an IP restriction to a cloud_project_database resource will cause the cloud_project_database resource to be updated on every apply
 
         Apply IP restrictions to an OVHcloud Managed Database cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         db = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="YYYY",
             id="ZZZZ")
         iprestriction = ovh.cloud_project_database.IpRestriction("iprestriction",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id,
             ip="178.97.6.0/24")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database cluster IP restrictions can be imported using the `service_name`, `engine`, `cluster_id` and the `ip`, separated by "/" E.g.,
 
         bash
 
@@ -272,29 +270,27 @@
         Deprecated: Use ip_restriction field in cloud_project_database resource instead.
         Continuing to use the CloudProjectDatabase.IpRestriction resource to add an IP restriction to a cloud_project_database resource will cause the cloud_project_database resource to be updated on every apply
 
         Apply IP restrictions to an OVHcloud Managed Database cluster.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         db = ovh.CloudProjectDatabase.get_database(service_name="XXXX",
             engine="YYYY",
             id="ZZZZ")
         iprestriction = ovh.cloud_project_database.IpRestriction("iprestriction",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id,
             ip="178.97.6.0/24")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed database cluster IP restrictions can be imported using the `service_name`, `engine`, `cluster_id` and the `ip`, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_acl.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,30 +202,28 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an ACL for a kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
         acl = ovh.cloud_project_database.KafkaAcl("acl",
             service_name=kafka.service_name,
             cluster_id=kafka.id,
             permission="read",
             topic="mytopic",
             username="johndoe")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed kafka clusters ACLs can be imported using the `service_name`, `cluster_id` and `id` of the acl, separated by "/" E.g.,
 
         bash
 
@@ -250,30 +248,28 @@
                  args: KafkaAclArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an ACL for a kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
         acl = ovh.cloud_project_database.KafkaAcl("acl",
             service_name=kafka.service_name,
             cluster_id=kafka.id,
             permission="read",
             topic="mytopic",
             username="johndoe")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed kafka clusters ACLs can be imported using the `service_name`, `cluster_id` and `id` of the acl, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,30 +202,28 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a schema registry ACL for a Kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
         schema_registry_acl = ovh.cloud_project_database.KafkaSchemaRegistryAcl("schemaRegistryAcl",
             service_name=kafka.service_name,
             cluster_id=kafka.id,
             permission="schema_registry_read",
             resource="Subject:myResource",
             username="johndoe")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kafka clusters schema registry ACLs can be imported using the `service_name`, `cluster_id` and `id` of the schema registry ACL, separated by "/" E.g.,
 
         bash
 
@@ -250,30 +248,28 @@
                  args: KafkaSchemaRegistryAclArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a schema registry ACL for a Kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
         schema_registry_acl = ovh.cloud_project_database.KafkaSchemaRegistryAcl("schemaRegistryAcl",
             service_name=kafka.service_name,
             cluster_id=kafka.id,
             permission="schema_registry_read",
             resource="Subject:myResource",
             username="johndoe")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed Kafka clusters schema registry ACLs can be imported using the `service_name`, `cluster_id` and `id` of the schema registry ACL, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/kafka_topic.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,14 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a topic for a kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
@@ -317,15 +316,14 @@
             cluster_id=kafka.id,
             min_insync_replicas=1,
             partitions=3,
             replication=2,
             retention_bytes=4,
             retention_hours=5)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed kafka clusters topics can be imported using the `service_name`, `cluster_id` and `id` of the topic, separated by "/" E.g.,
 
         bash
 
@@ -352,15 +350,14 @@
                  args: KafkaTopicArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a topic for a kafka cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         kafka = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="kafka",
             id="ZZZ")
@@ -369,15 +366,14 @@
             cluster_id=kafka.id,
             min_insync_replicas=1,
             partitions=3,
             replication=2,
             retention_bytes=4,
             retention_hours=5)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed kafka clusters topics can be imported using the `service_name`, `cluster_id` and `id` of the topic, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/log_subscription.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,14 @@
         """
         Creates a log subscrition for a cluster associated with a public cloud project.
 
         ## Example Usage
 
         Create a log subscription for a database.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         stream = ovh.Dbaas.get_logs_output_graylog_stream(service_name="ldp-xx-xxxxx",
             title="my stream")
         db = ovh.CloudProjectDatabase.get_database(service_name="XXX",
@@ -300,15 +299,14 @@
             id="ZZZ")
         subscription = ovh.cloud_project_database.LogSubscription("subscription",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id,
             stream_id=stream.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed clusters logs subscription can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the subscription, separated by "/" E.g.,
 
         bash
 
@@ -334,15 +332,14 @@
         """
         Creates a log subscrition for a cluster associated with a public cloud project.
 
         ## Example Usage
 
         Create a log subscription for a database.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         stream = ovh.Dbaas.get_logs_output_graylog_stream(service_name="ldp-xx-xxxxx",
             title="my stream")
         db = ovh.CloudProjectDatabase.get_database(service_name="XXX",
@@ -350,15 +347,14 @@
             id="ZZZ")
         subscription = ovh.cloud_project_database.LogSubscription("subscription",
             service_name=db.service_name,
             engine=db.engine,
             cluster_id=db.id,
             stream_id=stream.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed clusters logs subscription can be imported using the `service_name`, `engine`, `cluster_id` and `id` of the subscription, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,29 +413,27 @@
                  writes_to_commit_log_enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Creates a namespace for a M3DB cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         m3db = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="m3db",
             id="ZZZ")
         namespace = ovh.cloud_project_database.M3DbNamespace("namespace",
             service_name=m3db.service_name,
             cluster_id=m3db.id,
             resolution="P2D",
             retention_period_duration="PT48H")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed M3DB clusters namespaces can be imported using the `service_name`, `cluster_id` and `id` of the namespace, separated by "/" E.g.,
 
         bash
 
@@ -465,29 +463,27 @@
                  args: M3DbNamespaceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a namespace for a M3DB cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         m3db = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="m3db",
             id="ZZZ")
         namespace = ovh.cloud_project_database.M3DbNamespace("namespace",
             service_name=m3db.service_name,
             cluster_id=m3db.id,
             resolution="P2D",
             retention_period_duration="PT48H")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed M3DB clusters namespaces can be imported using the `service_name`, `cluster_id` and `id` of the namespace, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/m3_db_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,29 +167,27 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a pattern for a opensearch cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         opensearch = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="opensearch",
             id="ZZZ")
         pattern = ovh.cloud_project_database.OpensearchPattern("pattern",
             service_name=opensearch.service_name,
             cluster_id=opensearch.id,
             max_index_count=2,
             pattern="logs_*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed opensearch clusters patterns can be imported using the `service_name`, `cluster_id` and `id` of the pattern, separated by "/" E.g.,
 
         bash
 
@@ -212,29 +210,27 @@
                  args: OpensearchPatternArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a pattern for a opensearch cluster associated with a public cloud project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         opensearch = ovh.CloudProjectDatabase.get_database(service_name="XXX",
             engine="opensearch",
             id="ZZZ")
         pattern = ovh.cloud_project_database.OpensearchPattern("pattern",
             service_name=opensearch.service_name,
             cluster_id=opensearch.id,
             max_index_count=2,
             pattern="logs_*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Managed opensearch clusters patterns can be imported using the `service_name`, `cluster_id` and `id` of the pattern, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/opensearch_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/redis_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/cloudprojectdatabase/user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/cloudprojectdatabase/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/config/vars.py` & `pulumi_ovh-0.44.0/pulumi_ovh/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,37 +56,37 @@
 
 @pulumi.input_type
 class LogsInputConfigurationFlowggerArgs:
     def __init__(__self__, *,
                  log_format: pulumi.Input[str],
                  log_framing: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] log_format: Type of format to decode. One of "RFC5424", "LTSV", "GELF", "CAPNP"
-        :param pulumi.Input[str] log_framing: Indicates how messages are delimited. One of "LINE", "NUL", "SYSLEN", "CAPNP"
+        :param pulumi.Input[str] log_format: Type of format to decode
+        :param pulumi.Input[str] log_framing: Indicates how messages are delimited
         """
         pulumi.set(__self__, "log_format", log_format)
         pulumi.set(__self__, "log_framing", log_framing)
 
     @property
     @pulumi.getter(name="logFormat")
     def log_format(self) -> pulumi.Input[str]:
         """
-        Type of format to decode. One of "RFC5424", "LTSV", "GELF", "CAPNP"
+        Type of format to decode
         """
         return pulumi.get(self, "log_format")
 
     @log_format.setter
     def log_format(self, value: pulumi.Input[str]):
         pulumi.set(self, "log_format", value)
 
     @property
     @pulumi.getter(name="logFraming")
     def log_framing(self) -> pulumi.Input[str]:
         """
-        Indicates how messages are delimited. One of "LINE", "NUL", "SYSLEN", "CAPNP"
+        Indicates how messages are delimited
         """
         return pulumi.get(self, "log_framing")
 
     @log_framing.setter
     def log_framing(self, value: pulumi.Input[str]):
         pulumi.set(self, "log_framing", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_cluster.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,23 +198,21 @@
                      service_name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsClusterResult:
     """
     Use this data source to retrieve informations about a DBaas logs cluster tenant.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
         service_name="ldp-xx-xxxxx")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     __args__ = dict()
     __args__['clusterId'] = cluster_id
@@ -244,22 +242,20 @@
                             service_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsClusterResult]:
     """
     Use this data source to retrieve informations about a DBaas logs cluster tenant.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
         service_name="ldp-xx-xxxxx")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_clusters.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_clusters.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,22 +77,20 @@
 def get_logs_clusters(service_name: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsClustersResult:
     """
     Use this data source to retrieve UUIDs of DBaas logs clusters.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_clusters(service_name="ldp-xx-xxxxx")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -109,20 +107,18 @@
 def get_logs_clusters_output(service_name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsClustersResult]:
     """
     Use this data source to retrieve UUIDs of DBaas logs clusters.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_clusters(service_name="ldp-xx-xxxxx")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_input_engine.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_input_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,23 @@
                           version: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsInputEngineResult:
     """
     Use this data source to retrieve information about a DBaas logs input engine.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_input_engine(is_deprecated=True,
         name="logstash",
         service_name="ldp-xx-xxxxx",
         version="6.8")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool is_deprecated: Indicates if engine will soon not be supported.
     :param str name: The name of the logs input engine.
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     :param str version: Software version
     """
@@ -131,25 +129,23 @@
                                  version: Optional[pulumi.Input[Optional[str]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsInputEngineResult]:
     """
     Use this data source to retrieve information about a DBaas logs input engine.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     logstash = ovh.Dbaas.get_logs_input_engine(is_deprecated=True,
         name="logstash",
         service_name="ldp-xx-xxxxx",
         version="6.8")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool is_deprecated: Indicates if engine will soon not be supported.
     :param str name: The name of the logs input engine.
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     :param str version: Software version
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,23 +327,21 @@
                                    title: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsOutputGraylogStreamResult:
     """
     Use this data source to retrieve information about a DBaas logs output graylog stream.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     stream = ovh.Dbaas.get_logs_output_graylog_stream(service_name="ldp-xx-xxxxx",
         title="my stream")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     :param str title: Stream description
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -384,22 +382,20 @@
                                           title: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsOutputGraylogStreamResult]:
     """
     Use this data source to retrieve information about a DBaas logs output graylog stream.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     stream = ovh.Dbaas.get_logs_output_graylog_stream(service_name="ldp-xx-xxxxx",
         title="my stream")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     :param str title: Stream description
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_cluster.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,27 +356,25 @@
                  direct_input_allowed_networks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  query_allowed_networks: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         ldp = ovh.dbaas.LogsCluster("ldp",
             archive_allowed_networks=["10.0.0.0/16"],
             cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
             direct_input_allowed_networks=["10.0.0.0/16"],
             query_allowed_networks=["10.0.0.0/16"],
             service_name="ldp-xx-xxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud DBaaS Log Data Platform clusters can be imported using the `service_name` and `cluster_id` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -397,27 +395,25 @@
     def __init__(__self__,
                  resource_name: str,
                  args: LogsClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         ldp = ovh.dbaas.LogsCluster("ldp",
             archive_allowed_networks=["10.0.0.0/16"],
             cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
             direct_input_allowed_networks=["10.0.0.0/16"],
             query_allowed_networks=["10.0.0.0/16"],
             service_name="ldp-xx-xxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud DBaaS Log Data Platform clusters can be imported using the `service_name` and `cluster_id` of the cluster, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_input.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,14 @@
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a dbaas logs input.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         logstash = ovh.Dbaas.get_logs_input_engine(name="logstash",
             version="7.x")
         stream = ovh.dbaas.LogsOutputGraylogStream("stream",
@@ -487,15 +486,14 @@
             ssl_certificate => "/etc/ssl/private/server.crt"
             ssl_key => "/etc/ssl/private/server.key"
           }
         \"\"\",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_networks: List of IP blocks
         :param pulumi.Input[pulumi.InputType['LogsInputConfigurationArgs']] configuration: Input configuration
         :param pulumi.Input[str] description: Input description
         :param pulumi.Input[str] engine_id: Input engine ID
@@ -512,15 +510,14 @@
                  args: LogsInputArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a dbaas logs input.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         logstash = ovh.Dbaas.get_logs_input_engine(name="logstash",
             version="7.x")
         stream = ovh.dbaas.LogsOutputGraylogStream("stream",
@@ -544,15 +541,14 @@
             ssl_certificate => "/etc/ssl/private/server.crt"
             ssl_key => "/etc/ssl/private/server.key"
           }
         \"\"\",
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param LogsInputArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/logs_output_graylog_stream.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dbaas/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dbaas/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,33 +68,33 @@
         LogsInputConfigurationFlowgger.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  log_format: str,
                  log_framing: str):
         """
-        :param str log_format: Type of format to decode. One of "RFC5424", "LTSV", "GELF", "CAPNP"
-        :param str log_framing: Indicates how messages are delimited. One of "LINE", "NUL", "SYSLEN", "CAPNP"
+        :param str log_format: Type of format to decode
+        :param str log_framing: Indicates how messages are delimited
         """
         pulumi.set(__self__, "log_format", log_format)
         pulumi.set(__self__, "log_framing", log_framing)
 
     @property
     @pulumi.getter(name="logFormat")
     def log_format(self) -> str:
         """
-        Type of format to decode. One of "RFC5424", "LTSV", "GELF", "CAPNP"
+        Type of format to decode
         """
         return pulumi.get(self, "log_format")
 
     @property
     @pulumi.getter(name="logFraming")
     def log_framing(self) -> str:
         """
-        Indicates how messages are delimited. One of "LINE", "NUL", "SYSLEN", "CAPNP"
+        Indicates how messages are delimited
         """
         return pulumi.get(self, "log_framing")
 
 
 @pulumi.output_type
 class LogsInputConfigurationLogstash(dict):
     @staticmethod
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/ceph_acl.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,250 +5,292 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = [
-    'ServerInstallTaskDetailsArgs',
-    'ServerInstallTaskUserMetadataArgs',
-    'ServerNetworkingInterfaceArgs',
-]
+__all__ = ['CephAclArgs', 'CephAcl']
 
 @pulumi.input_type
-class ServerInstallTaskDetailsArgs:
+class CephAclArgs:
     def __init__(__self__, *,
-                 custom_hostname: Optional[pulumi.Input[str]] = None,
-                 disk_group_id: Optional[pulumi.Input[int]] = None,
-                 language: Optional[pulumi.Input[str]] = None,
-                 no_raid: Optional[pulumi.Input[bool]] = None,
-                 post_installation_script_link: Optional[pulumi.Input[str]] = None,
-                 post_installation_script_return: Optional[pulumi.Input[str]] = None,
-                 soft_raid_devices: Optional[pulumi.Input[int]] = None,
-                 use_spla: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
-        :param pulumi.Input[int] disk_group_id: Disk group id.
-        :param pulumi.Input[str] language: Deprecated, will be removed in next release.
-        :param pulumi.Input[bool] no_raid: Set to true to disable RAID.
-        :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
-        :param pulumi.Input[str] post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param pulumi.Input[int] soft_raid_devices: soft raid devices.
-        :param pulumi.Input[bool] use_spla: Deprecated, will be removed in next release.
-               
-               The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
-               
-               -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
-               
-               -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
-               
-               -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
-        """
-        if custom_hostname is not None:
-            pulumi.set(__self__, "custom_hostname", custom_hostname)
-        if disk_group_id is not None:
-            pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if language is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-            pulumi.log.warn("""language is deprecated: This field is deprecated and will be removed in a future release""")
-        if language is not None:
-            pulumi.set(__self__, "language", language)
-        if no_raid is not None:
-            pulumi.set(__self__, "no_raid", no_raid)
-        if post_installation_script_link is not None:
-            pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
-        if post_installation_script_return is not None:
-            pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if soft_raid_devices is not None:
-            pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
-        if use_spla is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-            pulumi.log.warn("""use_spla is deprecated: This field is deprecated and will be removed in a future release""")
-        if use_spla is not None:
-            pulumi.set(__self__, "use_spla", use_spla)
-
-    @property
-    @pulumi.getter(name="customHostname")
-    def custom_hostname(self) -> Optional[pulumi.Input[str]]:
-        """
-        Set up the server using the provided hostname instead of the default hostname.
-        """
-        return pulumi.get(self, "custom_hostname")
-
-    @custom_hostname.setter
-    def custom_hostname(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "custom_hostname", value)
+                 netmask: pulumi.Input[str],
+                 network: pulumi.Input[str],
+                 service_name: pulumi.Input[str]):
+        """
+        The set of arguments for constructing a CephAcl resource.
+        :param pulumi.Input[str] netmask: The network mask to apply
+        :param pulumi.Input[str] network: The network IP to authorize
+        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        """
+        pulumi.set(__self__, "netmask", netmask)
+        pulumi.set(__self__, "network", network)
+        pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter(name="diskGroupId")
-    def disk_group_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def netmask(self) -> pulumi.Input[str]:
         """
-        Disk group id.
+        The network mask to apply
         """
-        return pulumi.get(self, "disk_group_id")
+        return pulumi.get(self, "netmask")
 
-    @disk_group_id.setter
-    def disk_group_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "disk_group_id", value)
+    @netmask.setter
+    def netmask(self, value: pulumi.Input[str]):
+        pulumi.set(self, "netmask", value)
 
     @property
     @pulumi.getter
-    def language(self) -> Optional[pulumi.Input[str]]:
+    def network(self) -> pulumi.Input[str]:
         """
-        Deprecated, will be removed in next release.
+        The network IP to authorize
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-        pulumi.log.warn("""language is deprecated: This field is deprecated and will be removed in a future release""")
+        return pulumi.get(self, "network")
 
-        return pulumi.get(self, "language")
-
-    @language.setter
-    def language(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "language", value)
+    @network.setter
+    def network(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="noRaid")
-    def no_raid(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Input[str]:
         """
-        Set to true to disable RAID.
+        The internal name of your dedicated CEPH
         """
-        return pulumi.get(self, "no_raid")
+        return pulumi.get(self, "service_name")
 
-    @no_raid.setter
-    def no_raid(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "no_raid", value)
+    @service_name.setter
+    def service_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "service_name", value)
 
-    @property
-    @pulumi.getter(name="postInstallationScriptLink")
-    def post_installation_script_link(self) -> Optional[pulumi.Input[str]]:
-        """
-        Indicate the URL where your postinstall customisation script is located.
-        """
-        return pulumi.get(self, "post_installation_script_link")
 
-    @post_installation_script_link.setter
-    def post_installation_script_link(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "post_installation_script_link", value)
+@pulumi.input_type
+class _CephAclState:
+    def __init__(__self__, *,
+                 family: Optional[pulumi.Input[str]] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering CephAcl resources.
+        :param pulumi.Input[str] family: IP family. `IPv4` or `IPv6`
+        :param pulumi.Input[str] netmask: The network mask to apply
+        :param pulumi.Input[str] network: The network IP to authorize
+        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        """
+        if family is not None:
+            pulumi.set(__self__, "family", family)
+        if netmask is not None:
+            pulumi.set(__self__, "netmask", netmask)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if service_name is not None:
+            pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter(name="postInstallationScriptReturn")
-    def post_installation_script_return(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def family(self) -> Optional[pulumi.Input[str]]:
         """
-        Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
+        IP family. `IPv4` or `IPv6`
         """
-        return pulumi.get(self, "post_installation_script_return")
+        return pulumi.get(self, "family")
 
-    @post_installation_script_return.setter
-    def post_installation_script_return(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "post_installation_script_return", value)
+    @family.setter
+    def family(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "family", value)
 
     @property
-    @pulumi.getter(name="softRaidDevices")
-    def soft_raid_devices(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def netmask(self) -> Optional[pulumi.Input[str]]:
         """
-        soft raid devices.
+        The network mask to apply
         """
-        return pulumi.get(self, "soft_raid_devices")
+        return pulumi.get(self, "netmask")
 
-    @soft_raid_devices.setter
-    def soft_raid_devices(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "soft_raid_devices", value)
+    @netmask.setter
+    def netmask(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "netmask", value)
 
     @property
-    @pulumi.getter(name="useSpla")
-    def use_spla(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def network(self) -> Optional[pulumi.Input[str]]:
         """
-        Deprecated, will be removed in next release.
-
-        The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
-
-        -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
-
-        -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
-
-        -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
+        The network IP to authorize
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-        pulumi.log.warn("""use_spla is deprecated: This field is deprecated and will be removed in a future release""")
-
-        return pulumi.get(self, "use_spla")
-
-    @use_spla.setter
-    def use_spla(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "use_spla", value)
+        return pulumi.get(self, "network")
 
-
-@pulumi.input_type
-class ServerInstallTaskUserMetadataArgs:
-    def __init__(__self__, *,
-                 key: pulumi.Input[str],
-                 value: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] key: The key for the user_metadata
-        :param pulumi.Input[str] value: The value for the user_metadata
-        """
-        pulumi.set(__self__, "key", key)
-        pulumi.set(__self__, "value", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
+
+    @property
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The internal name of your dedicated CEPH
+        """
+        return pulumi.get(self, "service_name")
+
+    @service_name.setter
+    def service_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_name", value)
+
+
+class CephAcl(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Add a new access ACL for the given network/mask.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        my_ceph = ovh.Dedicated.get_ceph(service_name="94d423da-0e55-45f2-9812-836460a19939")
+        my_acl = ovh.dedicated.CephAcl("my-acl",
+            service_name=my_ceph.id,
+            network="1.2.3.4",
+            netmask="255.255.255.255")
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] netmask: The network mask to apply
+        :param pulumi.Input[str] network: The network IP to authorize
+        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: CephAclArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Add a new access ACL for the given network/mask.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        my_ceph = ovh.Dedicated.get_ceph(service_name="94d423da-0e55-45f2-9812-836460a19939")
+        my_acl = ovh.dedicated.CephAcl("my-acl",
+            service_name=my_ceph.id,
+            network="1.2.3.4",
+            netmask="255.255.255.255")
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param CephAclArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(CephAclArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 netmask: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = CephAclArgs.__new__(CephAclArgs)
+
+            if netmask is None and not opts.urn:
+                raise TypeError("Missing required property 'netmask'")
+            __props__.__dict__["netmask"] = netmask
+            if network is None and not opts.urn:
+                raise TypeError("Missing required property 'network'")
+            __props__.__dict__["network"] = network
+            if service_name is None and not opts.urn:
+                raise TypeError("Missing required property 'service_name'")
+            __props__.__dict__["service_name"] = service_name
+            __props__.__dict__["family"] = None
+        super(CephAcl, __self__).__init__(
+            'ovh:Dedicated/cephAcl:CephAcl',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            family: Optional[pulumi.Input[str]] = None,
+            netmask: Optional[pulumi.Input[str]] = None,
+            network: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'CephAcl':
+        """
+        Get an existing CephAcl resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] family: IP family. `IPv4` or `IPv6`
+        :param pulumi.Input[str] netmask: The network mask to apply
+        :param pulumi.Input[str] network: The network IP to authorize
+        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _CephAclState.__new__(_CephAclState)
+
+        __props__.__dict__["family"] = family
+        __props__.__dict__["netmask"] = netmask
+        __props__.__dict__["network"] = network
+        __props__.__dict__["service_name"] = service_name
+        return CephAcl(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
+    def family(self) -> pulumi.Output[str]:
         """
-        The key for the user_metadata
+        IP family. `IPv4` or `IPv6`
         """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
+        return pulumi.get(self, "family")
 
     @property
     @pulumi.getter
-    def value(self) -> pulumi.Input[str]:
-        """
-        The value for the user_metadata
+    def netmask(self) -> pulumi.Output[str]:
         """
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: pulumi.Input[str]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class ServerNetworkingInterfaceArgs:
-    def __init__(__self__, *,
-                 macs: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 type: pulumi.Input[str]):
+        The network mask to apply
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] macs: Interface Mac address
-        :param pulumi.Input[str] type: Interface type
-        """
-        pulumi.set(__self__, "macs", macs)
-        pulumi.set(__self__, "type", type)
+        return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter
-    def macs(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    def network(self) -> pulumi.Output[str]:
         """
-        Interface Mac address
+        The network IP to authorize
         """
-        return pulumi.get(self, "macs")
-
-    @macs.setter
-    def macs(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "macs", value)
+        return pulumi.get(self, "network")
 
     @property
-    @pulumi.getter
-    def type(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Output[str]:
         """
-        Interface type
+        The internal name of your dedicated CEPH
         """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: pulumi.Input[str]):
-        pulumi.set(self, "type", value)
-
+        return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/ceph_acl.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/refresh.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,296 +5,248 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['CephAclArgs', 'CephAcl']
+__all__ = ['RefreshArgs', 'Refresh']
 
 @pulumi.input_type
-class CephAclArgs:
+class RefreshArgs:
     def __init__(__self__, *,
-                 netmask: pulumi.Input[str],
-                 network: pulumi.Input[str],
+                 keepers: pulumi.Input[Sequence[pulumi.Input[str]]],
                  service_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a CephAcl resource.
-        :param pulumi.Input[str] netmask: The network mask to apply
-        :param pulumi.Input[str] network: The network IP to authorize
-        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        The set of arguments for constructing a Refresh resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         """
-        pulumi.set(__self__, "netmask", netmask)
-        pulumi.set(__self__, "network", network)
+        pulumi.set(__self__, "keepers", keepers)
         pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter
-    def netmask(self) -> pulumi.Input[str]:
+    def keepers(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        The network mask to apply
+        List of values tracked to trigger refresh, used also to form implicit dependencies
         """
-        return pulumi.get(self, "netmask")
+        return pulumi.get(self, "keepers")
 
-    @netmask.setter
-    def netmask(self, value: pulumi.Input[str]):
-        pulumi.set(self, "netmask", value)
-
-    @property
-    @pulumi.getter
-    def network(self) -> pulumi.Input[str]:
-        """
-        The network IP to authorize
-        """
-        return pulumi.get(self, "network")
-
-    @network.setter
-    def network(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network", value)
+    @keepers.setter
+    def keepers(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The internal name of your dedicated CEPH
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
 
 @pulumi.input_type
-class _CephAclState:
+class _RefreshState:
     def __init__(__self__, *,
-                 family: Optional[pulumi.Input[str]] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering CephAcl resources.
-        :param pulumi.Input[str] family: IP family. `IPv4` or `IPv6`
-        :param pulumi.Input[str] netmask: The network mask to apply
-        :param pulumi.Input[str] network: The network IP to authorize
-        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
-        """
-        if family is not None:
-            pulumi.set(__self__, "family", family)
-        if netmask is not None:
-            pulumi.set(__self__, "netmask", netmask)
-        if network is not None:
-            pulumi.set(__self__, "network", network)
+        Input properties used for looking up and filtering Refresh resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        """
+        if keepers is not None:
+            pulumi.set(__self__, "keepers", keepers)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter
-    def family(self) -> Optional[pulumi.Input[str]]:
+    def keepers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        IP family. `IPv4` or `IPv6`
+        List of values tracked to trigger refresh, used also to form implicit dependencies
         """
-        return pulumi.get(self, "family")
+        return pulumi.get(self, "keepers")
 
-    @family.setter
-    def family(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "family", value)
-
-    @property
-    @pulumi.getter
-    def netmask(self) -> Optional[pulumi.Input[str]]:
-        """
-        The network mask to apply
-        """
-        return pulumi.get(self, "netmask")
-
-    @netmask.setter
-    def netmask(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "netmask", value)
-
-    @property
-    @pulumi.getter
-    def network(self) -> Optional[pulumi.Input[str]]:
-        """
-        The network IP to authorize
-        """
-        return pulumi.get(self, "network")
-
-    @network.setter
-    def network(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network", value)
+    @keepers.setter
+    def keepers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The internal name of your dedicated CEPH
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
 
-class CephAcl(pulumi.CustomResource):
+class Refresh(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Add a new access ACL for the given network/mask.
+        Applies changes from other `ovh_iploadbalancing_*` resources to the production configuration of loadbalancers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        my_ceph = ovh.Dedicated.get_ceph(service_name="94d423da-0e55-45f2-9812-836460a19939")
-        my_acl = ovh.dedicated.CephAcl("my-acl",
-            service_name=my_ceph.id,
-            network="1.2.3.4",
-            netmask="255.255.255.255")
+        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
+            state="ok")
+        farmname = ovh.ip_load_balancing.TcpFarm("farmname",
+            port=8080,
+            service_name=lb.service_name,
+            zone="all")
+        backend = ovh.ip_load_balancing.TcpFarmServer("backend",
+            address="4.5.6.7",
+            backup=True,
+            display_name="mybackend",
+            farm_id=farmname.id,
+            port=80,
+            probe=True,
+            proxy_protocol_version="v2",
+            service_name=lb.service_name,
+            ssl=False,
+            status="active",
+            weight=2)
+        mylb = ovh.ip_load_balancing.Refresh("mylb",
+            keepers=[[__item.address for __item in [backend]]],
+            service_name=lb.service_name)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] netmask: The network mask to apply
-        :param pulumi.Input[str] network: The network IP to authorize
-        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CephAclArgs,
+                 args: RefreshArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Add a new access ACL for the given network/mask.
+        Applies changes from other `ovh_iploadbalancing_*` resources to the production configuration of loadbalancers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        my_ceph = ovh.Dedicated.get_ceph(service_name="94d423da-0e55-45f2-9812-836460a19939")
-        my_acl = ovh.dedicated.CephAcl("my-acl",
-            service_name=my_ceph.id,
-            network="1.2.3.4",
-            netmask="255.255.255.255")
+        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
+            state="ok")
+        farmname = ovh.ip_load_balancing.TcpFarm("farmname",
+            port=8080,
+            service_name=lb.service_name,
+            zone="all")
+        backend = ovh.ip_load_balancing.TcpFarmServer("backend",
+            address="4.5.6.7",
+            backup=True,
+            display_name="mybackend",
+            farm_id=farmname.id,
+            port=80,
+            probe=True,
+            proxy_protocol_version="v2",
+            service_name=lb.service_name,
+            ssl=False,
+            status="active",
+            weight=2)
+        mylb = ovh.ip_load_balancing.Refresh("mylb",
+            keepers=[[__item.address for __item in [backend]]],
+            service_name=lb.service_name)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
-        :param CephAclArgs args: The arguments to use to populate this resource's properties.
+        :param RefreshArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CephAclArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RefreshArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 netmask: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CephAclArgs.__new__(CephAclArgs)
+            __props__ = RefreshArgs.__new__(RefreshArgs)
 
-            if netmask is None and not opts.urn:
-                raise TypeError("Missing required property 'netmask'")
-            __props__.__dict__["netmask"] = netmask
-            if network is None and not opts.urn:
-                raise TypeError("Missing required property 'network'")
-            __props__.__dict__["network"] = network
+            if keepers is None and not opts.urn:
+                raise TypeError("Missing required property 'keepers'")
+            __props__.__dict__["keepers"] = keepers
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
-            __props__.__dict__["family"] = None
-        super(CephAcl, __self__).__init__(
-            'ovh:Dedicated/cephAcl:CephAcl',
+        super(Refresh, __self__).__init__(
+            'ovh:IpLoadBalancing/refresh:Refresh',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            family: Optional[pulumi.Input[str]] = None,
-            netmask: Optional[pulumi.Input[str]] = None,
-            network: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None) -> 'CephAcl':
+            keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'Refresh':
         """
-        Get an existing CephAcl resource's state with the given name, id, and optional extra
+        Get an existing Refresh resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] family: IP family. `IPv4` or `IPv6`
-        :param pulumi.Input[str] netmask: The network mask to apply
-        :param pulumi.Input[str] network: The network IP to authorize
-        :param pulumi.Input[str] service_name: The internal name of your dedicated CEPH
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _CephAclState.__new__(_CephAclState)
+        __props__ = _RefreshState.__new__(_RefreshState)
 
-        __props__.__dict__["family"] = family
-        __props__.__dict__["netmask"] = netmask
-        __props__.__dict__["network"] = network
+        __props__.__dict__["keepers"] = keepers
         __props__.__dict__["service_name"] = service_name
-        return CephAcl(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def family(self) -> pulumi.Output[str]:
-        """
-        IP family. `IPv4` or `IPv6`
-        """
-        return pulumi.get(self, "family")
-
-    @property
-    @pulumi.getter
-    def netmask(self) -> pulumi.Output[str]:
-        """
-        The network mask to apply
-        """
-        return pulumi.get(self, "netmask")
+        return Refresh(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def network(self) -> pulumi.Output[str]:
+    def keepers(self) -> pulumi.Output[Sequence[str]]:
         """
-        The network IP to authorize
+        List of values tracked to trigger refresh, used also to form implicit dependencies
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The internal name of your dedicated CEPH
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_ceph.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_ceph.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,22 +174,20 @@
              status: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCephResult:
     """
     Use this data source to retrieve information about a dedicated CEPH.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_ceph = ovh.Dedicated.get_ceph(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ceph_version: CEPH cluster version
     :param str service_name: The service name of the dedicated CEPH cluster.
     :param str status: the status of the service
     """
     __args__ = dict()
@@ -219,22 +217,20 @@
                     status: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCephResult]:
     """
     Use this data source to retrieve information about a dedicated CEPH.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_ceph = ovh.Dedicated.get_ceph(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ceph_version: CEPH cluster version
     :param str service_name: The service name of the dedicated CEPH cluster.
     :param str status: the status of the service
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_nas_ha.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_nas_ha.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,22 +167,20 @@
 def get_nas_ha(service_name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNasHAResult:
     """
     Use this data source to retrieve information about a dedicated HA-NAS.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_nas_ha = ovh.Dedicated.get_nas_ha(service_name="zpool-12345")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated HA-NAS.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -206,20 +204,18 @@
 def get_nas_ha_output(service_name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNasHAResult]:
     """
     Use this data source to retrieve information about a dedicated HA-NAS.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_nas_ha = ovh.Dedicated.get_nas_ha(service_name="zpool-12345")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated HA-NAS.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_boots.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_boots.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,23 +88,21 @@
                      service_name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerBootsResult:
     """
     Use this data source to get the list of compatible netboots for a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     netboots = ovh.Dedicated.get_server_boots(boot_type="harddisk",
         service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str boot_type: Filter the value of bootType property (harddisk, rescue, ipxeCustomerScript, internal, network)
     :param str kernel: Filter the value of kernel property (iPXE script name)
     :param str service_name: The internal name of your dedicated server.
     """
     __args__ = dict()
@@ -128,23 +126,21 @@
                             service_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerBootsResult]:
     """
     Use this data source to get the list of compatible netboots for a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     netboots = ovh.Dedicated.get_server_boots(boot_type="harddisk",
         service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str boot_type: Filter the value of bootType property (harddisk, rescue, ipxeCustomerScript, internal, network)
     :param str kernel: Filter the value of kernel property (iPXE script name)
     :param str service_name: The internal name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_specifications_hardware.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,22 +237,20 @@
 def get_server_specifications_hardware(service_name: Optional[str] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerSpecificationsHardwareResult:
     """
     Use this data source to get the hardward information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     spec = ovh.Dedicated.get_server_specifications_hardware(service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your dedicated server.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -282,20 +280,18 @@
 def get_server_specifications_hardware_output(service_name: Optional[pulumi.Input[str]] = None,
                                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerSpecificationsHardwareResult]:
     """
     Use this data source to get the hardward information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     spec = ovh.Dedicated.get_server_specifications_hardware(service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/get_server_specifications_network.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/get_server_specifications_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,22 +153,20 @@
 def get_server_specifications_network(service_name: Optional[str] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerSpecificationsNetworkResult:
     """
     Use this data source to get the network information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     spec = ovh.Dedicated.get_server_specifications_network(service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your dedicated server.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -191,20 +189,18 @@
 def get_server_specifications_network_output(service_name: Optional[pulumi.Input[str]] = None,
                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerSpecificationsNetworkResult]:
     """
     Use this data source to get the network information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     spec = ovh.Dedicated.get_server_specifications_network(service_name="myserver")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,25 +228,23 @@
                  size: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Provides a resource for managing partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartition("my-partition",
             protocol="NFS",
             service_name="zpool-12345",
             size=20)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS can be imported using the `{service_name}/{name}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartition:NasHAPartition my-partition zpool-12345/my-partition`
@@ -267,25 +265,23 @@
                  args: NasHAPartitionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource for managing partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartition("my-partition",
             protocol="NFS",
             service_name="zpool-12345",
             size=20)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS can be imported using the `{service_name}/{name}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartition:NasHAPartition my-partition zpool-12345/my-partition`
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition_access.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,26 +163,24 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a resource for managing access rights to partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartitionAccess("my-partition",
             ip="123.123.123.123/32",
             partition_name="my-partition",
             service_name="zpool-12345",
             type="readwrite")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition access can be imported using the `{service_name}/{partition_name}/{ip}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%2F32`
@@ -202,26 +200,24 @@
                  args: NasHAPartitionAccessArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource for managing access rights to partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartitionAccess("my-partition",
             ip="123.123.123.123/32",
             partition_name="my-partition",
             service_name="zpool-12345",
             type="readwrite")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition access can be imported using the `{service_name}/{partition_name}/{ip}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%2F32`
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,25 +130,23 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a resource for managing **snapshot** to partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartitionSnapshot("my-partition",
             partition_name="my-partition",
             service_name="zpool-12345",
             type="day-3")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition snapshot can be imported using the `{service_name}/{partition_name}/{type}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartitionSnapshot:NasHAPartitionSnapshot my-partition zpool-12345/my-partition/day-3`
@@ -167,25 +165,23 @@
                  args: NasHAPartitionSnapshotArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource for managing **snapshot** to partitions on HA-NAS services
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_partition = ovh.dedicated.NasHAPartitionSnapshot("my-partition",
             partition_name="my-partition",
             service_name="zpool-12345",
             type="day-3")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition snapshot can be imported using the `{service_name}/{partition_name}/{type}`, e.g.
 
         ```sh
         $ pulumi import ovh:Dedicated/nasHAPartitionSnapshot:NasHAPartitionSnapshot my-partition zpool-12345/my-partition/day-3`
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,14 @@
             suggest = "no_raid"
         elif key == "postInstallationScriptLink":
             suggest = "post_installation_script_link"
         elif key == "postInstallationScriptReturn":
             suggest = "post_installation_script_return"
         elif key == "softRaidDevices":
             suggest = "soft_raid_devices"
-        elif key == "useSpla":
-            suggest = "use_spla"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServerInstallTaskDetails. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServerInstallTaskDetails.__key_warning(key)
         return super().__getitem__(key)
@@ -73,54 +71,38 @@
     def get(self, key: str, default = None) -> Any:
         ServerInstallTaskDetails.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  custom_hostname: Optional[str] = None,
                  disk_group_id: Optional[int] = None,
-                 language: Optional[str] = None,
                  no_raid: Optional[bool] = None,
                  post_installation_script_link: Optional[str] = None,
                  post_installation_script_return: Optional[str] = None,
-                 soft_raid_devices: Optional[int] = None,
-                 use_spla: Optional[bool] = None):
+                 soft_raid_devices: Optional[int] = None):
         """
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param int disk_group_id: Disk group id.
-        :param str language: Deprecated, will be removed in next release.
         :param bool no_raid: Set to true to disable RAID.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param str post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         :param int soft_raid_devices: soft raid devices.
-        :param bool use_spla: Deprecated, will be removed in next release.
-               
-               The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
-               
-               -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
-               
-               -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
-               
-               -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if disk_group_id is not None:
             pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if language is not None:
-            pulumi.set(__self__, "language", language)
         if no_raid is not None:
             pulumi.set(__self__, "no_raid", no_raid)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
         if soft_raid_devices is not None:
             pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
-        if use_spla is not None:
-            pulumi.set(__self__, "use_spla", use_spla)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[str]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -131,25 +113,14 @@
     def disk_group_id(self) -> Optional[int]:
         """
         Disk group id.
         """
         return pulumi.get(self, "disk_group_id")
 
     @property
-    @pulumi.getter
-    def language(self) -> Optional[str]:
-        """
-        Deprecated, will be removed in next release.
-        """
-        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-        pulumi.log.warn("""language is deprecated: This field is deprecated and will be removed in a future release""")
-
-        return pulumi.get(self, "language")
-
-    @property
     @pulumi.getter(name="noRaid")
     def no_raid(self) -> Optional[bool]:
         """
         Set to true to disable RAID.
         """
         return pulumi.get(self, "no_raid")
 
@@ -173,33 +144,14 @@
     @pulumi.getter(name="softRaidDevices")
     def soft_raid_devices(self) -> Optional[int]:
         """
         soft raid devices.
         """
         return pulumi.get(self, "soft_raid_devices")
 
-    @property
-    @pulumi.getter(name="useSpla")
-    def use_spla(self) -> Optional[bool]:
-        """
-        Deprecated, will be removed in next release.
-
-        The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
-
-        -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
-
-        -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
-
-        -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
-        """
-        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
-        pulumi.log.warn("""use_spla is deprecated: This field is deprecated and will be removed in a future release""")
-
-        return pulumi.get(self, "use_spla")
-
 
 @pulumi.output_type
 class ServerInstallTaskUserMetadata(dict):
     def __init__(__self__, *,
                  key: str,
                  value: str):
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_install_task.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_install_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -327,15 +327,14 @@
                  template_name: Optional[pulumi.Input[str]] = None,
                  user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         Using a custom template based on an OVHCloud template
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
         debian = ovh.me.InstallationTemplate("debian",
@@ -353,19 +352,17 @@
                 custom_hostname="mytest",
             ),
             user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
                 key="sshKey",
                 value="ssh-ed25519 AAAAC3...",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Using a BringYourOwnLinux (BYOLinux) template (with userMetadata)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
@@ -420,19 +417,17 @@
           - vim
           - tree
         final_message: The system is finally up, after $UPTIME seconds
         \"\"\",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         Using a Microsoft Windows server OVHcloud template with a specific language
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
@@ -444,15 +439,14 @@
                 custom_hostname="mytest",
             ),
             user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
                 key="language",
                 value="fr-fr",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
 
         bash
 
@@ -475,15 +469,14 @@
                  resource_name: str,
                  args: ServerInstallTaskArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         Using a custom template based on an OVHCloud template
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
         debian = ovh.me.InstallationTemplate("debian",
@@ -501,19 +494,17 @@
                 custom_hostname="mytest",
             ),
             user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
                 key="sshKey",
                 value="ssh-ed25519 AAAAC3...",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         Using a BringYourOwnLinux (BYOLinux) template (with userMetadata)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
@@ -568,19 +559,17 @@
           - vim
           - tree
         final_message: The system is finally up, after $UPTIME seconds
         \"\"\",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         Using a Microsoft Windows server OVHcloud template with a specific language
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue")
@@ -592,15 +581,14 @@
                 custom_hostname="mytest",
             ),
             user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
                 key="language",
                 value="fr-fr",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_networking.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_reboot_task.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_reboot_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue",
             kernel="rescue64-pro")
@@ -209,15 +208,14 @@
             boot_id=rescue.results[0],
             monitoring=True,
             state="ok")
         server_reboot = ovh.dedicated.ServerRebootTask("serverReboot",
             service_name=rescue.service_name,
             keepers=[server_on_rescue.boot_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger reboot, used also to form implicit dependencies.
         :param pulumi.Input[str] service_name: The service_name of your dedicated server.
         """
         ...
@@ -225,15 +223,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServerRebootTaskArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue",
             kernel="rescue64-pro")
@@ -242,15 +239,14 @@
             boot_id=rescue.results[0],
             monitoring=True,
             state="ok")
         server_reboot = ovh.dedicated.ServerRebootTask("serverReboot",
             service_name=rescue.service_name,
             keepers=[server_on_rescue.boot_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ServerRebootTaskArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/dedicated/server_update.py` & `pulumi_ovh-0.44.0/pulumi_ovh/dedicated/server_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,29 +196,27 @@
                  monitoring: Optional[pulumi.Input[bool]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue",
             kernel="rescue64-pro")
         server = ovh.dedicated.ServerUpdate("server",
             service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_id=rescue.results[0],
             monitoring=True,
             state="ok")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] boot_id: boot id of the server
         :param pulumi.Input[str] boot_script: boot script of the server
         :param pulumi.Input[bool] monitoring: Icmp monitoring state
         :param pulumi.Input[str] service_name: The service_name of your dedicated server.
@@ -229,29 +227,27 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServerUpdateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_type="rescue",
             kernel="rescue64-pro")
         server = ovh.dedicated.ServerUpdate("server",
             service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
             boot_id=rescue.results[0],
             monitoring=True,
             state="ok")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ServerUpdateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                  catalog_name: Optional[pulumi.Input[str]] = None,
                  configurations: Optional[pulumi.Input[Sequence[pulumi.Input['ZonePlanConfigurationArgs']]]] = None):
         """
         :param pulumi.Input[str] duration: duration
         :param pulumi.Input[str] plan_code: Plan code
         :param pulumi.Input[str] pricing_mode: Pricing model identifier
         :param pulumi.Input[str] catalog_name: Catalog name
-        :param pulumi.Input[Sequence[pulumi.Input['ZonePlanConfigurationArgs']]] configurations: Representation of a configuration item for personalizing product
+        :param pulumi.Input[Sequence[pulumi.Input['ZonePlanConfigurationArgs']]] configurations: Representation of a configuration item for personalizing product. 2 configurations are required : one for `zone` and one for `template`
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
         if catalog_name is not None:
             pulumi.set(__self__, "catalog_name", catalog_name)
         if configurations is not None:
@@ -231,15 +231,15 @@
     def catalog_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "catalog_name", value)
 
     @property
     @pulumi.getter
     def configurations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ZonePlanConfigurationArgs']]]]:
         """
-        Representation of a configuration item for personalizing product
+        Representation of a configuration item for personalizing product. 2 configurations are required : one for `zone` and one for `template`
         """
         return pulumi.get(self, "configurations")
 
     @configurations.setter
     def configurations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ZonePlanConfigurationArgs']]]]):
         pulumi.set(self, "configurations", value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/get_zone.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/get_zone.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,22 +116,20 @@
 def get_zone(name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetZoneResult:
     """
     Use this data source to retrieve information about a domain zone.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     rootzone = ovh.Domain.get_zone(name="mysite.ovh")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the domain zone.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -151,20 +149,18 @@
 def get_zone_output(name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetZoneResult]:
     """
     Use this data source to retrieve information about a domain zone.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     rootzone = ovh.Domain.get_zone(name="mysite.ovh")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the domain zone.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/get_zone_dns_sec.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/get_zone_dns_sec.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,22 +68,20 @@
 def get_zone_dns_sec(zone_name: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetZoneDNSSecResult:
     """
     Use this data source to retrieve information about a domain zone DNSSEC status.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     dnssec = ovh.Domain.get_zone_dns_sec(zone_name="mysite.ovh")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str zone_name: The name of the domain zone
     """
     __args__ = dict()
     __args__['zoneName'] = zone_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -99,20 +97,18 @@
 def get_zone_dns_sec_output(zone_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetZoneDNSSecResult]:
     """
     Use this data source to retrieve information about a domain zone DNSSEC status.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     dnssec = ovh.Domain.get_zone_dns_sec(zone_name="mysite.ovh")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str zone_name: The name of the domain zone
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                  catalog_name: Optional[str] = None,
                  configurations: Optional[Sequence['outputs.ZonePlanConfiguration']] = None):
         """
         :param str duration: duration
         :param str plan_code: Plan code
         :param str pricing_mode: Pricing model identifier
         :param str catalog_name: Catalog name
-        :param Sequence['ZonePlanConfigurationArgs'] configurations: Representation of a configuration item for personalizing product
+        :param Sequence['ZonePlanConfigurationArgs'] configurations: Representation of a configuration item for personalizing product. 2 configurations are required : one for `zone` and one for `template`
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
         if catalog_name is not None:
             pulumi.set(__self__, "catalog_name", catalog_name)
         if configurations is not None:
@@ -241,15 +241,15 @@
         """
         return pulumi.get(self, "catalog_name")
 
     @property
     @pulumi.getter
     def configurations(self) -> Optional[Sequence['outputs.ZonePlanConfiguration']]:
         """
-        Representation of a configuration item for personalizing product
+        Representation of a configuration item for personalizing product. 2 configurations are required : one for `zone` and one for `template`
         """
         return pulumi.get(self, "configurations")
 
 
 @pulumi.output_type
 class ZonePlanConfiguration(dict):
     def __init__(__self__, *,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/zone.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 __all__ = ['ZoneArgs', 'Zone']
 
 @pulumi.input_type
 class ZoneArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['ZonePlanArgs'],
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['ZoneOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['ZonePlanOptionArgs']]]] = None):
         """
         The set of arguments for constructing a Zone resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['ZonePlanArgs'] plan: Product Plan to order
+        :param pulumi.Input[Sequence[pulumi.Input['ZoneOrderArgs']]] orders: Details about an Order
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['ZonePlanOptionArgs']]] plan_options: Product Plan to order
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -58,14 +62,26 @@
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: pulumi.Input['ZonePlanArgs']):
         pulumi.set(self, "plan", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ZoneOrderArgs']]]]:
+        """
+        Details about an Order
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ZoneOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -276,23 +292,23 @@
 
 
 class Zone(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZoneOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['ZonePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZonePlanOptionArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         zone_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -313,43 +329,42 @@
                     ovh.domain.ZonePlanConfigurationArgs(
                         label="template",
                         value="minimized",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Zone can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders) at the creation time of the zone.
 
         bash
 
         ```sh
         $ pulumi import ovh:Domain/zone:Zone zone order_id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZoneOrderArgs']]]] orders: Details about an Order
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['ZonePlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZonePlanOptionArgs']]]] plan_options: Product Plan to order
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ZoneArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         zone_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -370,15 +385,14 @@
                     ovh.domain.ZonePlanConfigurationArgs(
                         label="template",
                         value="minimized",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Zone can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders) at the creation time of the zone.
 
         bash
 
@@ -397,42 +411,43 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZoneOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['ZonePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ZonePlanOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ZoneArgs.__new__(ZoneArgs)
 
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
             __props__.__dict__["plan_options"] = plan_options
             __props__.__dict__["zone_urn"] = None
             __props__.__dict__["dnssec_supported"] = None
             __props__.__dict__["has_dns_anycast"] = None
             __props__.__dict__["last_update"] = None
             __props__.__dict__["name"] = None
             __props__.__dict__["name_servers"] = None
-            __props__.__dict__["orders"] = None
         super(Zone, __self__).__init__(
             'ovh:Domain/zone:Zone',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_dns_sec.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_dns_sec.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,22 +82,20 @@
                  zone_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Enable / disable DNSSEC on a domain zone.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         dnssec = ovh.domain.ZoneDNSSec("dnssec", zone_name="mysite.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] zone_name: The name of the domain zone
         """
         ...
     @overload
@@ -106,22 +104,20 @@
                  args: ZoneDNSSecArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Enable / disable DNSSEC on a domain zone.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         dnssec = ovh.domain.ZoneDNSSec("dnssec", zone_name="mysite.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ZoneDNSSecArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_record.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,28 +194,26 @@
                  target: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Add a record to a sub-domain
         test = ovh.domain.ZoneRecord("test",
             fieldtype="A",
             subdomain="test",
             target="0.0.0.0",
             ttl=3600,
             zone="testdemo.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](https://api.ovh.com/console/#/domain/zone/%7BzoneName%7D/record~GET), and the `zone`, separated by "." E.g.,
 
         bash
 
@@ -236,28 +234,26 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ZoneRecordArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Add a record to a sub-domain
         test = ovh.domain.ZoneRecord("test",
             fieldtype="A",
             subdomain="test",
             target="0.0.0.0",
             ttl=3600,
             zone="testdemo.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](https://api.ovh.com/console/#/domain/zone/%7BzoneName%7D/record~GET), and the `zone`, separated by "." E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/domain/zone_redirection.py` & `pulumi_ovh-0.44.0/pulumi_ovh/domain/zone_redirection.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,27 +262,25 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a OVHcloud domain zone redirection.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Add a redirection to a sub-domain
         test = ovh.domain.ZoneRedirection("test",
             subdomain="test",
             target="http://www.ovh",
             type="visiblePermanent",
             zone="testdemo.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A description of this redirection
         :param pulumi.Input[str] keywords: Keywords to describe this redirection
         :param pulumi.Input[str] subdomain: The name of the redirection
         :param pulumi.Input[str] target: The value of the redirection
@@ -297,27 +295,25 @@
                  args: ZoneRedirectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a OVHcloud domain zone redirection.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Add a redirection to a sub-domain
         test = ovh.domain.ZoneRedirection("test",
             subdomain="test",
             target="http://www.ovh",
             type="visiblePermanent",
             zone="testdemo.ovh")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ZoneRedirectionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/get_installation_templates.py` & `pulumi_ovh-0.44.0/pulumi_ovh/get_installation_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_installation_templates(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstallationTemplatesResult:
     """
     Use this data source to get the list of installation templates available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     templates = ovh.get_installation_templates()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:index/getInstallationTemplates:getInstallationTemplates', __args__, opts=opts, typ=GetInstallationTemplatesResult).value
 
     return AwaitableGetInstallationTemplatesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_installation_templates)
 def get_installation_templates_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstallationTemplatesResult]:
     """
     Use this data source to get the list of installation templates available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     templates = ovh.get_installation_templates()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/get_server.py` & `pulumi_ovh-0.44.0/pulumi_ovh/get_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,22 +345,20 @@
 def get_server(service_name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServerResult:
     """
     Use this data source to retrieve information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     server = ovh.get_server(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated server.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -399,20 +397,18 @@
 def get_server_output(service_name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerResult]:
     """
     Use this data source to retrieve information about a dedicated server associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     server = ovh.get_server(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/get_servers.py` & `pulumi_ovh-0.44.0/pulumi_ovh/get_servers.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_servers(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServersResult:
     """
     Use this data source to get the list of dedicated servers associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     servers = ovh.get_servers()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:index/getServers:getServers', __args__, opts=opts, typ=GetServersResult).value
 
     return AwaitableGetServersResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_servers)
 def get_servers_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServersResult]:
     """
     Use this data source to get the list of dedicated servers associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     servers = ovh.get_servers()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/get_vrack_networks.py` & `pulumi_ovh-0.44.0/pulumi_ovh/get_vrack_networks.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,23 +88,21 @@
                        vlan_id: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVrackNetworksResult:
     """
     Use this data source to get the list of Vrack network ids available for your IPLoadbalancer associated with your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb_networks = ovh.get_vrack_networks(service_name="XXXXXX",
         subnet="10.0.0.0/24")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your IP load balancing
     :param str subnet: Filters networks on the subnet.
     :param int vlan_id: Filters networks on the vlan id.
     """
     __args__ = dict()
@@ -128,23 +126,21 @@
                               vlan_id: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVrackNetworksResult]:
     """
     Use this data source to get the list of Vrack network ids available for your IPLoadbalancer associated with your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb_networks = ovh.get_vrack_networks(service_name="XXXXXX",
         subnet="10.0.0.0/24")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your IP load balancing
     :param str subnet: Filters networks on the subnet.
     :param int vlan_id: Filters networks on the vlan id.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -248,16 +248,14 @@
 class PrivateDatabasePlanConfigurationArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
         :param pulumi.Input[str] label: Identifier of the resource
         :param pulumi.Input[str] value: Path to the resource in API.OVH.COM
-               
-               Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
@@ -271,16 +269,14 @@
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
         Path to the resource in API.OVH.COM
-
-        Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
@@ -290,16 +286,16 @@
     def __init__(__self__, *,
                  duration: pulumi.Input[str],
                  plan_code: pulumi.Input[str],
                  pricing_mode: pulumi.Input[str],
                  catalog_name: Optional[pulumi.Input[str]] = None,
                  configurations: Optional[pulumi.Input[Sequence[pulumi.Input['PrivateDatabasePlanOptionConfigurationArgs']]]] = None):
         """
-        :param pulumi.Input[str] duration: duration.
-        :param pulumi.Input[str] plan_code: Plan code.
+        :param pulumi.Input[str] duration: Service duration
+        :param pulumi.Input[str] plan_code: Plan code
         :param pulumi.Input[str] pricing_mode: Pricing model identifier
         :param pulumi.Input[str] catalog_name: Catalog name
         :param pulumi.Input[Sequence[pulumi.Input['PrivateDatabasePlanOptionConfigurationArgs']]] configurations: Representation of a configuration item for personalizing product
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
@@ -308,27 +304,27 @@
         if configurations is not None:
             pulumi.set(__self__, "configurations", configurations)
 
     @property
     @pulumi.getter
     def duration(self) -> pulumi.Input[str]:
         """
-        duration.
+        Service duration
         """
         return pulumi.get(self, "duration")
 
     @duration.setter
     def duration(self, value: pulumi.Input[str]):
         pulumi.set(self, "duration", value)
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> pulumi.Input[str]:
         """
-        Plan code.
+        Plan code
         """
         return pulumi.get(self, "plan_code")
 
     @plan_code.setter
     def plan_code(self, value: pulumi.Input[str]):
         pulumi.set(self, "plan_code", value)
 
@@ -373,16 +369,14 @@
 class PrivateDatabasePlanOptionConfigurationArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
         :param pulumi.Input[str] label: Identifier of the resource
         :param pulumi.Input[str] value: Path to the resource in API.OVH.COM
-               
-               Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
@@ -396,16 +390,14 @@
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
         Path to the resource in API.OVH.COM
-
-        Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -281,22 +281,20 @@
 def get_private_database(service_name: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateDatabaseResult:
     """
     Use this data source to retrieve information about an hosting database.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     database = ovh.Hosting.get_private_database(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your private database
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -330,20 +328,18 @@
 def get_private_database_output(service_name: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateDatabaseResult]:
     """
     Use this data source to retrieve information about an hosting database.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     database = ovh.Hosting.get_private_database(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your private database
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_allowlist.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_allowlist.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,23 +138,21 @@
                                    service_name: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateDatabaseAllowlistResult:
     """
     Use this data source to retrieve information about an hosting privatedatabase whitelist.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     whitelist = ovh.Hosting.get_private_database_allowlist(ip="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The whitelisted IP in your instance
     :param str service_name: The internal name of your private database
     """
     __args__ = dict()
     __args__['ip'] = ip
@@ -179,22 +177,20 @@
                                           service_name: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateDatabaseAllowlistResult]:
     """
     Use this data source to retrieve information about an hosting privatedatabase whitelist.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     whitelist = ovh.Hosting.get_private_database_allowlist(ip="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The whitelisted IP in your instance
     :param str service_name: The internal name of your private database
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_db.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,23 +115,21 @@
                             service_name: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateDatabaseDbResult:
     """
     Use this data source to retrieve information about an hosting privatedatabase.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mydatabase = ovh.Hosting.get_private_database_db(database_name="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str database_name: Database name
     :param str service_name: The internal name of your private database
     """
     __args__ = dict()
     __args__['databaseName'] = database_name
@@ -154,22 +152,20 @@
                                    service_name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateDatabaseDbResult]:
     """
     Use this data source to retrieve information about an hosting privatedatabase.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mydatabase = ovh.Hosting.get_private_database_db(database_name="XXXXXX",
         service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str database_name: Database name
     :param str service_name: The internal name of your private database
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,23 +91,21 @@
                               user_name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateDatabaseUserResult:
     """
     Use this data source to retrieve information about an hosting privatedatabase user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user = ovh.Hosting.get_private_database_user(service_name="XXXXXX",
         user_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your private database
     :param str user_name: User name
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -128,22 +126,20 @@
                                      user_name: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateDatabaseUserResult]:
     """
     Use this data source to retrieve information about an hosting privatedatabase user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user = ovh.Hosting.get_private_database_user(service_name="XXXXXX",
         user_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your private database
     :param str user_name: User name
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/get_private_database_user_grant.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/get_private_database_user_grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,22 @@
                                     user_name: Optional[str] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrivateDatabaseUserGrantResult:
     """
     Use this data source to retrieve information about an hosting privatedatabase user grant.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user_grant = ovh.Hosting.get_private_database_user_grant(database_name="XXXXXX",
         service_name="XXXXXX",
         user_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str database_name: The database name on which grant the user
     :param str service_name: The internal name of your private database
     :param str user_name: The user name
     """
     __args__ = dict()
@@ -142,24 +140,22 @@
                                            user_name: Optional[pulumi.Input[str]] = None,
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateDatabaseUserGrantResult]:
     """
     Use this data source to retrieve information about an hosting privatedatabase user grant.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     user_grant = ovh.Hosting.get_private_database_user_grant(database_name="XXXXXX",
         service_name="XXXXXX",
         user_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str database_name: The database name on which grant the user
     :param str service_name: The internal name of your private database
     :param str user_name: The user name
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,16 +256,14 @@
 class PrivateDatabasePlanConfiguration(dict):
     def __init__(__self__, *,
                  label: str,
                  value: str):
         """
         :param str label: Identifier of the resource
         :param str value: Path to the resource in API.OVH.COM
-               
-               Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> str:
@@ -275,16 +273,14 @@
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
         Path to the resource in API.OVH.COM
-
-        Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class PrivateDatabasePlanOption(dict):
     @staticmethod
@@ -311,16 +307,16 @@
     def __init__(__self__, *,
                  duration: str,
                  plan_code: str,
                  pricing_mode: str,
                  catalog_name: Optional[str] = None,
                  configurations: Optional[Sequence['outputs.PrivateDatabasePlanOptionConfiguration']] = None):
         """
-        :param str duration: duration.
-        :param str plan_code: Plan code.
+        :param str duration: Service duration
+        :param str plan_code: Plan code
         :param str pricing_mode: Pricing model identifier
         :param str catalog_name: Catalog name
         :param Sequence['PrivateDatabasePlanOptionConfigurationArgs'] configurations: Representation of a configuration item for personalizing product
         """
         pulumi.set(__self__, "duration", duration)
         pulumi.set(__self__, "plan_code", plan_code)
         pulumi.set(__self__, "pricing_mode", pricing_mode)
@@ -329,23 +325,23 @@
         if configurations is not None:
             pulumi.set(__self__, "configurations", configurations)
 
     @property
     @pulumi.getter
     def duration(self) -> str:
         """
-        duration.
+        Service duration
         """
         return pulumi.get(self, "duration")
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> str:
         """
-        Plan code.
+        Plan code
         """
         return pulumi.get(self, "plan_code")
 
     @property
     @pulumi.getter(name="pricingMode")
     def pricing_mode(self) -> str:
         """
@@ -374,16 +370,14 @@
 class PrivateDatabasePlanOptionConfiguration(dict):
     def __init__(__self__, *,
                  label: str,
                  value: str):
         """
         :param str label: Identifier of the resource
         :param str value: Path to the resource in API.OVH.COM
-               
-               Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> str:
@@ -393,16 +387,14 @@
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
         Path to the resource in API.OVH.COM
-
-        Plan order valid values can be found on OVHcloud [APIv6](https://api.ovh.com/console/#/hosting/privateDatabase/availableOrderCapacities~GET)
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GetPrivateDatabaseDbUserResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 
 @pulumi.input_type
 class PrivateDatabaseArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['PrivateDatabasePlanArgs'],
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['PrivateDatabaseOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['PrivateDatabasePlanOptionArgs']]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PrivateDatabase resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['PrivateDatabasePlanArgs'] plan: Product Plan to order
         :param pulumi.Input[str] display_name: Name displayed in customer panel for your private database
+        :param pulumi.Input[Sequence[pulumi.Input['PrivateDatabaseOrderArgs']]] orders: Details about your Order
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['PrivateDatabasePlanOptionArgs']]] plan_options: Product Plan to order
         :param pulumi.Input[str] service_name: Service name
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -78,14 +82,26 @@
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['PrivateDatabaseOrderArgs']]]]:
+        """
+        Details about your Order
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['PrivateDatabaseOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -537,24 +553,24 @@
 
 class PrivateDatabase(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabaseOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['PrivateDatabasePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabasePlanOptionArgs']]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         database_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -577,27 +593,27 @@
                         label="engine",
                         value="postgresql_12",
                     ),
                 ],
             ))
         pulumi.export("privatedatabaseServiceName", database_private_database.service_name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Webhosting database can be imported using the `service_name`, E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabase:PrivateDatabase database service_name
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_name: Name displayed in customer panel for your private database
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabaseOrderArgs']]]] orders: Details about your Order
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['PrivateDatabasePlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabasePlanOptionArgs']]]] plan_options: Product Plan to order
         :param pulumi.Input[str] service_name: Service name
         """
         ...
@@ -605,15 +621,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: PrivateDatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         database_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -636,15 +651,14 @@
                         label="engine",
                         value="postgresql_12",
                     ),
                 ],
             ))
         pulumi.export("privatedatabaseServiceName", database_private_database.service_name)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Webhosting database can be imported using the `service_name`, E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabase:PrivateDatabase database service_name
@@ -662,14 +676,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabaseOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['PrivateDatabasePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PrivateDatabasePlanOptionArgs']]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -677,14 +692,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PrivateDatabaseArgs.__new__(PrivateDatabaseArgs)
 
             __props__.__dict__["display_name"] = display_name
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
@@ -693,15 +709,14 @@
             __props__.__dict__["database_urn"] = None
             __props__.__dict__["cpu"] = None
             __props__.__dict__["datacenter"] = None
             __props__.__dict__["hostname"] = None
             __props__.__dict__["hostname_ftp"] = None
             __props__.__dict__["infrastructure"] = None
             __props__.__dict__["offer"] = None
-            __props__.__dict__["orders"] = None
             __props__.__dict__["port"] = None
             __props__.__dict__["port_ftp"] = None
             __props__.__dict__["quota_size"] = None
             __props__.__dict__["quota_used"] = None
             __props__.__dict__["ram"] = None
             __props__.__dict__["server"] = None
             __props__.__dict__["state"] = None
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_allowlist.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_allowlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,26 +195,24 @@
                  sftp: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Create a new IP whitelist on your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         ip = ovh.hosting.PrivateDatabaseAllowlist("ip",
             ip="1.2.3.4",
             service=True,
             service_name="XXXXXX",
             sftp=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database whitelist can be imported using the `service_name` and the `ip`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseAllowlist:PrivateDatabaseAllowlist ip service_name/ip
@@ -235,26 +233,24 @@
                  args: PrivateDatabaseAllowlistArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a new IP whitelist on your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         ip = ovh.hosting.PrivateDatabaseAllowlist("ip",
             ip="1.2.3.4",
             service=True,
             service_name="XXXXXX",
             sftp=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database whitelist can be imported using the `service_name` and the `ip`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseAllowlist:PrivateDatabaseAllowlist ip service_name/ip
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_db.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,24 +98,22 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a new database on your private cloud database service.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         database = ovh.hosting.PrivateDatabaseDb("database",
             database_name="XXXXXX",
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Webhosting database can be imported using the `service_name` and the `database_name`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseDb:PrivateDatabaseDb database service_name/database_name
@@ -133,24 +131,22 @@
                  args: PrivateDatabaseDbArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a new database on your private cloud database service.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         database = ovh.hosting.PrivateDatabaseDb("database",
             database_name="XXXXXX",
             service_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud Webhosting database can be imported using the `service_name` and the `database_name`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseDb:PrivateDatabaseDb database service_name/database_name
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,25 +130,23 @@
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a new user on your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user = ovh.hosting.PrivateDatabaseUser("user",
             password="XXXXXX",
             service_name="XXXXXX",
             user_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database user can be imported using the `service_name` and the `user_name`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseUser:PrivateDatabaseUser user service_name/user_name
@@ -167,25 +165,23 @@
                  args: PrivateDatabaseUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Create a new user on your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user = ovh.hosting.PrivateDatabaseUser("user",
             password="XXXXXX",
             service_name="XXXXXX",
             user_name="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database user can be imported using the `service_name` and the `user_name`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseUser:PrivateDatabaseUser user service_name/user_name
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/hosting/private_database_user_grant.py` & `pulumi_ovh-0.44.0/pulumi_ovh/hosting/private_database_user_grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,24 @@
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Add grant on a database in your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user_grant = ovh.hosting.PrivateDatabaseUserGrant("userGrant",
             database_name="ovhcloud",
             grant="admin",
             service_name="XXXXXX",
             user_name="terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database user's grant can be imported using the `service_name`, the `user_name`, the `database_name` and the `grant`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseUserGrant:PrivateDatabaseUserGrant user service_name/user_name/database_name/grant
@@ -221,26 +219,24 @@
                  args: PrivateDatabaseUserGrantArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Add grant on a database in your private cloud database instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         user_grant = ovh.hosting.PrivateDatabaseUserGrant("userGrant",
             database_name="ovhcloud",
             grant="admin",
             service_name="XXXXXX",
             user_name="terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OVHcloud database user's grant can be imported using the `service_name`, the `user_name`, the `database_name` and the `grant`, separated by "/" E.g.,
 
         ```sh
         $ pulumi import ovh:Hosting/privateDatabaseUserGrant:PrivateDatabaseUserGrant user service_name/user_name/database_name/grant
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_permissions_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_permissions_groups.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_permissions_groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,22 +55,20 @@
 
 def get_permissions_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPermissionsGroupsResult:
     """
     Use this data source to retrieve an IAM permissions group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     website = ovh.Iam.get_permissions_group(urn="urn:v1:eu:permissionsGroup:ovh:controlPanelAccess")
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Iam/getPermissionsGroups:getPermissionsGroups', __args__, opts=opts, typ=GetPermissionsGroupsResult).value
 
     return AwaitableGetPermissionsGroupsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -80,17 +78,15 @@
 @_utilities.lift_output_func(get_permissions_groups)
 def get_permissions_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPermissionsGroupsResult]:
     """
     Use this data source to retrieve an IAM permissions group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     website = ovh.Iam.get_permissions_group(urn="urn:v1:eu:permissionsGroup:ovh:controlPanelAccess")
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_policies.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_policies.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_policies(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoliciesResult:
     """
     Use this data source to list the existing IAM policies of an account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_policies = ovh.Iam.get_policies()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Iam/getPolicies:getPolicies', __args__, opts=opts, typ=GetPoliciesResult).value
 
     return AwaitableGetPoliciesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_policies)
 def get_policies_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoliciesResult]:
     """
     Use this data source to list the existing IAM policies of an account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_policies = ovh.Iam.get_policies()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_policy.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -193,22 +193,20 @@
                permissions_groups: Optional[Sequence[str]] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPolicyResult:
     """
     Use this data source to retrieve am IAM policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_policy = ovh.Iam.get_policy(id="my_policy_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] allows: Set of actions allowed by the policy.
     :param Sequence[str] denies: Set of actions that will be denied no matter what policy exists.
     :param str description: Group description.
     :param Sequence[str] excepts: Set of actions that will be subtracted from the `allow` list.
     :param str id: UUID of the policy.
@@ -249,22 +247,20 @@
                       permissions_groups: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPolicyResult]:
     """
     Use this data source to retrieve am IAM policy.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_policy = ovh.Iam.get_policy(id="my_policy_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] allows: Set of actions allowed by the policy.
     :param Sequence[str] denies: Set of actions that will be denied no matter what policy exists.
     :param str description: Group description.
     :param Sequence[str] excepts: Set of actions that will be subtracted from the `allow` list.
     :param str id: UUID of the policy.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_reference_actions.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_reference_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_reference_resource_type.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_reference_resource_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_reference_resource_type(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetReferenceResourceTypeResult:
     """
     Use this data source to list all the IAM resource types.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     types = ovh.Iam.get_reference_resource_type()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Iam/getReferenceResourceType:getReferenceResourceType', __args__, opts=opts, typ=GetReferenceResourceTypeResult).value
 
     return AwaitableGetReferenceResourceTypeResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_reference_resource_type)
 def get_reference_resource_type_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReferenceResourceTypeResult]:
     """
     Use this data source to list all the IAM resource types.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     types = ovh.Iam.get_reference_resource_type()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_resource_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_resource_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,20 @@
 def get_resource_group(id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceGroupResult:
     """
     Use this data source get details about a resource group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_resource_group = ovh.Iam.get_resource_group(id="my_resource_group_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: Id of the resource group
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -164,20 +162,18 @@
 def get_resource_group_output(id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceGroupResult]:
     """
     Use this data source get details about a resource group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_resource_group = ovh.Iam.get_resource_group(id="my_resource_group_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: Id of the resource group
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/get_resource_groups.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/get_resource_groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_resource_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceGroupsResult:
     """
     Use this data source to list the existing IAM policies of an account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_groups = ovh.Iam.get_resource_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Iam/getResourceGroups:getResourceGroups', __args__, opts=opts, typ=GetResourceGroupsResult).value
 
     return AwaitableGetResourceGroupsResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_resource_groups)
 def get_resource_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceGroupsResult]:
     """
     Use this data source to list the existing IAM policies of an account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_groups = ovh.Iam.get_resource_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/permissions_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/policy.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,14 @@
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Creates an IAM policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         account = ovh.Me.get_me()
         my_group = ovh.me.IdentityGroup("myGroup", description="my_group created in Terraform")
         manager = ovh.iam.Policy("manager",
@@ -380,15 +379,14 @@
                 "account:apiovh:me/supportLevel/get",
                 "account:apiovh:me/certificates/get",
                 "account:apiovh:me/tag/get",
                 "account:apiovh:services/get",
                 "account:apiovh:*",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allows: List of actions allowed on resources by identities
         :param pulumi.Input[Sequence[pulumi.Input[str]]] denies: List of actions that will always be denied even if also allowed by this policy or another one.
         :param pulumi.Input[str] description: Description of the policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] excepts: List of overrides of action that must not be allowed even if they are caught by allow. Only makes sens if allow contains wildcards.
@@ -404,15 +402,14 @@
                  args: PolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an IAM policy.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         account = ovh.Me.get_me()
         my_group = ovh.me.IdentityGroup("myGroup", description="my_group created in Terraform")
         manager = ovh.iam.Policy("manager",
@@ -424,15 +421,14 @@
                 "account:apiovh:me/supportLevel/get",
                 "account:apiovh:me/certificates/get",
                 "account:apiovh:me/tag/get",
                 "account:apiovh:services/get",
                 "account:apiovh:*",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param PolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iam/resource_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iam/resource_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,25 +180,23 @@
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides an OVHcloud IAM resource group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_resource_group = ovh.iam.ResourceGroup("myResourceGroup", resources=[
             "urn:v1:eu:resource:service1:service1-id",
             "urn:v1:eu:resource:service2:service2-id",
         ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource groups can be imported by using their id.
 
         > Read only resource groups cannot be imported
 
@@ -214,25 +212,23 @@
                  args: Optional[ResourceGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an OVHcloud IAM resource group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_resource_group = ovh.iam.ResourceGroup("myResourceGroup", resources=[
             "urn:v1:eu:resource:service1:service1-id",
             "urn:v1:eu:resource:service2:service2-id",
         ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Resource groups can be imported by using their id.
 
         > Read only resource groups cannot be imported
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/firewall.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,24 +143,22 @@
                  ip_on_firewall: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to manage an IP firewall.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfirewall = ovh.ip.Firewall("myfirewall",
             ip="XXXXXX",
             ip_on_firewall="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ip: The IP or the CIDR
         :param pulumi.Input[str] ip_on_firewall: IPv4 address
                * `enabled ` - Whether firewall should be enabled
         """
@@ -171,24 +169,22 @@
                  args: FirewallArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to manage an IP firewall.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfirewall = ovh.ip.Firewall("myfirewall",
             ip="XXXXXX",
             ip_on_firewall="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/firewall_rule.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/firewall_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,27 +455,25 @@
                  tcp_option: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to manage a rule on an IP firewall.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfirewallrule = ovh.ip.FirewallRule("myfirewallrule",
             action="deny",
             ip="XXXXXX",
             ip_on_firewall="XXXXXX",
             protocol="tcp",
             sequence=0)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action: Possible values for action (deny|permit)
         :param pulumi.Input[float] destination_port: Destination port for your rule. Only with TCP/UDP protocol
         :param pulumi.Input[bool] fragments: Fragments option
         :param pulumi.Input[str] ip: The IP or the CIDR
@@ -493,27 +491,25 @@
                  args: FirewallRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to manage a rule on an IP firewall.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myfirewallrule = ovh.ip.FirewallRule("myfirewallrule",
             action="deny",
             ip="XXXXXX",
             ip_on_firewall="XXXXXX",
             protocol="tcp",
             sequence=0)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FirewallRuleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/get_firewall.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/get_firewall.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,23 +94,21 @@
                  ip_on_firewall: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFirewallResult:
     """
     Use this data source to retrieve information about an IP firewall.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfirewall = ovh.Ip.get_firewall(ip="XXXXXX",
         ip_on_firewall="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_firewall: IPv4 address
     """
     __args__ = dict()
     __args__['ip'] = ip
@@ -131,22 +129,20 @@
                         ip_on_firewall: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFirewallResult]:
     """
     Use this data source to retrieve information about an IP firewall.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfirewall = ovh.Ip.get_firewall(ip="XXXXXX",
         ip_on_firewall="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_firewall: IPv4 address
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/get_firewall_rule.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/get_firewall_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,24 +217,22 @@
                       sequence: Optional[float] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFirewallRuleResult:
     """
     Use this data source to retrieve information about a rule on an IP firewall.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfirewallrule = ovh.Ip.get_firewall_rule(ip="XXXXXX",
         ip_on_firewall="XXXXXX",
         sequence=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_firewall: IPv4 address
     :param float sequence: Rule position in the rules array
     """
     __args__ = dict()
@@ -268,24 +266,22 @@
                              sequence: Optional[pulumi.Input[float]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFirewallRuleResult]:
     """
     Use this data source to retrieve information about a rule on an IP firewall.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myfirewallrule = ovh.Ip.get_firewall_rule(ip="XXXXXX",
         ip_on_firewall="XXXXXX",
         sequence=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_firewall: IPv4 address
     :param float sequence: Rule position in the rules array
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/get_mitigation.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/get_mitigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,23 +106,21 @@
                    ip_on_mitigation: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMitigationResult:
     """
     Use this resource to retrieve information about an IP permanent mitigation.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mitigation_data = ovh.Ip.get_mitigation(ip="XXXXXX",
         ip_on_mitigation="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_mitigation: IPv4 address
     """
     __args__ = dict()
     __args__['ip'] = ip
@@ -144,22 +142,20 @@
                           ip_on_mitigation: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMitigationResult]:
     """
     Use this resource to retrieve information about an IP permanent mitigation.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mitigation_data = ovh.Ip.get_mitigation(ip="XXXXXX",
         ip_on_mitigation="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str ip: The IP or the CIDR
     :param str ip_on_mitigation: IPv4 address
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/get_service.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/get_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,20 @@
 def get_service(service_name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceResult:
     """
     Use this data source to retrieve information about an IP service.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myip = ovh.Ip.get_service(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -181,20 +179,18 @@
 def get_service_output(service_name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceResult]:
     """
     Use this data source to retrieve information about an IP service.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myip = ovh.Ip.get_service(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service name
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/ip_service.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/ip_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 
 @pulumi.input_type
 class IpServiceArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['IpServicePlanArgs'],
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['IpServiceOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['IpServicePlanOptionArgs']]]] = None):
         """
         The set of arguments for constructing a IpService resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['IpServicePlanArgs'] plan: Product Plan to order
         :param pulumi.Input[str] description: Custom description on your ip.
+        :param pulumi.Input[Sequence[pulumi.Input['IpServiceOrderArgs']]] orders: Details about an Order
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['IpServicePlanOptionArgs']]] plan_options: Product Plan to order
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -74,14 +78,26 @@
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IpServiceOrderArgs']]]]:
+        """
+        Details about an Order
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IpServiceOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -329,23 +345,23 @@
 
 class IpService(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServiceOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['IpServicePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServicePlanOptionArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary="fr")
         ipblock_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -361,34 +377,33 @@
                 pricing_mode=ipblock_cart_product_plan.selected_prices[0].pricing_mode,
                 configurations=[ovh.ip.IpServicePlanConfigurationArgs(
                     label="country",
                     value="FR",
                 )],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Custom description on your ip.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServiceOrderArgs']]]] orders: Details about an Order
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['IpServicePlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServicePlanOptionArgs']]]] plan_options: Product Plan to order
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IpServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary="fr")
         ipblock_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -404,15 +419,14 @@
                 pricing_mode=ipblock_cart_product_plan.selected_prices[0].pricing_mode,
                 configurations=[ovh.ip.IpServicePlanConfigurationArgs(
                     label="country",
                     value="FR",
                 )],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IpServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -422,40 +436,41 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServiceOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['IpServicePlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IpServicePlanOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = IpServiceArgs.__new__(IpServiceArgs)
 
             __props__.__dict__["description"] = description
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
             __props__.__dict__["plan_options"] = plan_options
             __props__.__dict__["can_be_terminated"] = None
             __props__.__dict__["country"] = None
             __props__.__dict__["ip"] = None
-            __props__.__dict__["orders"] = None
             __props__.__dict__["organisation_id"] = None
             __props__.__dict__["routed_tos"] = None
             __props__.__dict__["service_name"] = None
             __props__.__dict__["type"] = None
         super(IpService, __self__).__init__(
             'ovh:Ip/ipService:IpService',
             resource_name,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/mitigation.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/mitigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,24 +167,22 @@
                  permanent: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Use this resource to manage an IP permanent mitigation.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mitigation = ovh.ip.Mitigation("mitigation",
             ip="XXXXXX",
             ip_on_mitigation="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ip: The IP or the CIDR
         :param pulumi.Input[str] ip_on_mitigation: IPv4 address
                * `permanent ` - Set on true if the IP is on permanent mitigation
         :param pulumi.Input[bool] permanent: Set on true if your ip is on permanent mitigation
@@ -196,24 +194,22 @@
                  args: MitigationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to manage an IP permanent mitigation.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mitigation = ovh.ip.Mitigation("mitigation",
             ip="XXXXXX",
             ip_on_mitigation="XXXXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param MitigationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/move.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/move.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         :param pulumi.Input[bool] can_be_terminated: Whether IP service can be terminated
         :param pulumi.Input[str] country: Country
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
         :param pulumi.Input[str] organisation_id: IP block organisation Id
         :param pulumi.Input['MoveRoutedToArgs'] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
                instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
-        :param pulumi.Input[str] service_name: Name of the service to route the IP to. IP will be parked if this value is an empty string
+        :param pulumi.Input[str] service_name: Service name in the form of `ip-<part-1>.<part-2>.<part-3>.<part-4>`
         :param pulumi.Input[str] task_start_date: Starting date and time field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] task_status: Status field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] type: Possible values for ip type
         """
         if can_be_terminated is not None:
             pulumi.set(__self__, "can_be_terminated", can_be_terminated)
         if country is not None:
@@ -190,15 +190,15 @@
     def routed_to(self, value: Optional[pulumi.Input['MoveRoutedToArgs']]):
         pulumi.set(self, "routed_to", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the service to route the IP to. IP will be parked if this value is an empty string
+        Service name in the form of `ip-<part-1>.<part-2>.<part-3>.<part-4>`
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
@@ -249,41 +249,37 @@
                  routed_to: Optional[pulumi.Input[pulumi.InputType['MoveRoutedToArgs']]] = None,
                  __props__=None):
         """
         Moves a given IP to a different service, or inversely, parks it if empty service is given
 
         ## Move IP `1.2.3.4` to service loadbalancer-XXXXX
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         move_ip_to_load_balancer_xxxxx = ovh.ip.Move("moveIpToLoadBalancerXxxxx",
             ip="1.2.3.4",
             routed_to=ovh.ip.MoveRoutedToArgs(
                 service_name="loadbalancer-XXXXX",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Park IP/Detach IP `1.2.3.4` from any service
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         park_ip = ovh.ip.Move("parkIp",
             ip="1.2.3.4",
             routed_to=ovh.ip.MoveRoutedToArgs(
                 service_name="",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
         :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
                instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
@@ -295,41 +291,37 @@
                  args: MoveArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Moves a given IP to a different service, or inversely, parks it if empty service is given
 
         ## Move IP `1.2.3.4` to service loadbalancer-XXXXX
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         move_ip_to_load_balancer_xxxxx = ovh.ip.Move("moveIpToLoadBalancerXxxxx",
             ip="1.2.3.4",
             routed_to=ovh.ip.MoveRoutedToArgs(
                 service_name="loadbalancer-XXXXX",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Park IP/Detach IP `1.2.3.4` from any service
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         park_ip = ovh.ip.Move("parkIp",
             ip="1.2.3.4",
             routed_to=ovh.ip.MoveRoutedToArgs(
                 service_name="",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param MoveArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -398,15 +390,15 @@
         :param pulumi.Input[bool] can_be_terminated: Whether IP service can be terminated
         :param pulumi.Input[str] country: Country
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
         :param pulumi.Input[str] organisation_id: IP block organisation Id
         :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
                instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
-        :param pulumi.Input[str] service_name: Name of the service to route the IP to. IP will be parked if this value is an empty string
+        :param pulumi.Input[str] service_name: Service name in the form of `ip-<part-1>.<part-2>.<part-3>.<part-4>`
         :param pulumi.Input[str] task_start_date: Starting date and time field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] task_status: Status field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] type: Possible values for ip type
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MoveState.__new__(_MoveState)
@@ -472,15 +464,15 @@
         """
         return pulumi.get(self, "routed_to")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        Name of the service to route the IP to. IP will be parked if this value is an empty string
+        Service name in the form of `ip-<part-1>.<part-2>.<part-3>.<part-4>`
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter(name="taskStartDate")
     def task_start_date(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/ip/reverse.py` & `pulumi_ovh-0.44.0/pulumi_ovh/ip/reverse.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,26 +130,24 @@
                  ip: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a OVHcloud IP reverse.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Set the reverse of an IP
         test = ovh.ip.Reverse("test",
             ip="192.0.2.0/24",
             reverse_ip="192.0.2.1",
             reverse_value="example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `ip`, `ip_reverse` of the address, separated by "|" E.g.,
 
         bash
 
@@ -170,26 +168,24 @@
                  args: ReverseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a OVHcloud IP reverse.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         # Set the reverse of an IP
         test = ovh.ip.Reverse("test",
             ip="192.0.2.0/24",
             reverse_ip="192.0.2.1",
             reverse_value="example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `ip`, `ip_reverse` of the address, separated by "|" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,15 @@
 @pulumi.input_type
 class LoadBalancerOrderableZoneArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  plan_code: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: The zone three letter code
-        :param pulumi.Input[str] plan_code: Plan code
+        :param pulumi.Input[str] plan_code: The billing planCode for this zone
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if plan_code is not None:
             pulumi.set(__self__, "plan_code", plan_code)
 
     @property
@@ -500,15 +500,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> Optional[pulumi.Input[str]]:
         """
-        Plan code
+        The billing planCode for this zone
         """
         return pulumi.get(self, "plan_code")
 
     @plan_code.setter
     def plan_code(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plan_code", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,23 +194,21 @@
                           zones: Optional[Sequence[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIpLoadBalancingResult:
     """
     Use this data source to retrieve information about an IP Load Balancing product
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="XXXXXX",
         state="ok")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str display_name: the name displayed in ManagerV6 for your iplb (max 50 chars)
     :param str ip_loadbalancing: Your IP load balancing
     :param str ipv4: The IPV4 associated to your IP load balancing
     :param str ipv6: The IPV6 associated to your IP load balancing
     :param str offer: The offer of your IP load balancing
@@ -274,23 +272,21 @@
                                  zones: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIpLoadBalancingResult]:
     """
     Use this data source to retrieve information about an IP Load Balancing product
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="XXXXXX",
         state="ok")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str display_name: the name displayed in ManagerV6 for your iplb (max 50 chars)
     :param str ip_loadbalancing: Your IP load balancing
     :param str ipv4: The IPV4 associated to your IP load balancing
     :param str ipv6: The IPV6 associated to your IP load balancing
     :param str offer: The offer of your IP load balancing
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/get_vrack_network.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/get_vrack_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,23 +114,21 @@
                       vrack_network_id: Optional[int] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVrackNetworkResult:
     """
     Use this data source to get the details of Vrack network available for your IPLoadbalancer associated with your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb_network = ovh.IpLoadBalancing.get_vrack_network(service_name="XXXXXX",
         vrack_network_id="yyy")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your IP load balancing
     :param int vrack_network_id: Internal Load Balancer identifier of the vRack private network
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
@@ -153,22 +151,20 @@
                              vrack_network_id: Optional[pulumi.Input[int]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVrackNetworkResult]:
     """
     Use this data source to get the details of Vrack network available for your IPLoadbalancer associated with your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     lb_network = ovh.IpLoadBalancing.get_vrack_network(service_name="XXXXXX",
         vrack_network_id="yyy")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The internal name of your IP load balancing
     :param int vrack_network_id: Internal Load Balancer identifier of the vRack private network
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_farm.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_farm.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  vrack_network_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a HttpFarm resource.
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input['HttpFarmProbeArgs'] probe: define a backend healthcheck probe
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`, `cookie`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         """
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "zone", zone)
         if balance is not None:
@@ -98,15 +98,15 @@
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -158,15 +158,15 @@
                  stickiness: Optional[pulumi.Input[str]] = None,
                  vrack_network_id: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering HttpFarm resources.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input['HttpFarmProbeArgs'] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`, `cookie`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         if balance is not None:
@@ -210,15 +210,15 @@
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -298,37 +298,35 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a HTTP backend server group (farm) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.HttpFarm("farmname",
             display_name="ingress-8080-gra",
             service_name=lb.service_name,
             zone="GRA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP farm can be imported using the following format `service_name` and the `id` of the farm, separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input[pulumi.InputType['HttpFarmProbeArgs']] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`, `cookie`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         ...
@@ -338,27 +336,25 @@
                  args: HttpFarmArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a HTTP backend server group (farm) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.HttpFarm("farmname",
             display_name="ingress-8080-gra",
             service_name=lb.service_name,
             zone="GRA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP farm can be imported using the following format `service_name` and the `id` of the farm, separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param HttpFarmArgs args: The arguments to use to populate this resource's properties.
@@ -427,15 +423,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input[pulumi.InputType['HttpFarmProbeArgs']] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`, `cookie`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -468,15 +464,15 @@
         """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[Optional[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def probe(self) -> pulumi.Output[Optional['outputs.HttpFarmProbe']]:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_farm_server.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_farm_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,14 @@
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Creates a backend server entry linked to HTTP loadbalancing group (farm)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.HttpFarm("farmname",
@@ -491,15 +490,14 @@
             probe=True,
             proxy_protocol_version="v2",
             service_name=lb.service_name,
             ssl=False,
             status="active",
             weight=2)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP farm server can be imported using the following format `service_name`, the `id` of the farm and the `id` of the server separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -523,15 +521,14 @@
                  args: HttpFarmServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend server entry linked to HTTP loadbalancing group (farm)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.HttpFarm("farmname",
@@ -547,15 +544,14 @@
             probe=True,
             proxy_protocol_version="v2",
             service_name=lb.service_name,
             ssl=False,
             status="active",
             weight=2)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP farm server can be imported using the following format `service_name`, the `id` of the farm and the `id` of the server separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param HttpFarmServerArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_frontend.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,15 +468,14 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a backend HTTP server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.HttpFarm("farm80",
@@ -487,19 +486,17 @@
         testfrontend = ovh.ip_load_balancing.HttpFrontend("testfrontend",
             default_farm_id=farm80.id,
             display_name="ingress-8080-gra",
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With HTTP Header
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.HttpFarm("farm80",
@@ -514,15 +511,14 @@
                 "X-Ip-Header %%ci",
                 "X-Port-Header %%cp",
             ],
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP frontend can be imported using the following format `service_name` and the `id` of the frontend separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -549,15 +545,14 @@
                  args: HttpFrontendArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend HTTP server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.HttpFarm("farm80",
@@ -568,19 +563,17 @@
         testfrontend = ovh.ip_load_balancing.HttpFrontend("testfrontend",
             default_farm_id=farm80.id,
             display_name="ingress-8080-gra",
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With HTTP Header
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.HttpFarm("farm80",
@@ -595,15 +588,14 @@
                 "X-Ip-Header %%ci",
                 "X-Port-Header %%cp",
             ],
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP frontend can be imported using the following format `service_name` and the `id` of the frontend separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param HttpFrontendArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_route.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         """
         Input properties used for looking up and filtering HttpRoute resources.
         :param pulumi.Input['HttpRouteActionArgs'] action: Action triggered when all rules match
         :param pulumi.Input[str] display_name: Human readable name for your route, this field is for you
         :param pulumi.Input[int] frontend_id: Route traffic for this frontend
         :param pulumi.Input[Sequence[pulumi.Input['HttpRouteRuleArgs']]] rules: List of rules to match to trigger action
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] status: HTTP status code for "redirect" and "reject" actions
+        :param pulumi.Input[str] status: Route status. Routes in "ok" state are ready to operate
         :param pulumi.Input[int] weight: Route priority ([0..255]). 0 if null. Highest priority routes are evaluated first. Only the first matching route will trigger an action
         """
         if action is not None:
             pulumi.set(__self__, "action", action)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if frontend_id is not None:
@@ -194,15 +194,15 @@
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
-        HTTP status code for "redirect" and "reject" actions
+        Route status. Routes in "ok" state are ready to operate
         """
         return pulumi.get(self, "status")
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
@@ -233,30 +233,28 @@
         """
         Manage HTTP route for a loadbalancer service
 
         ## Example Usage
 
         Route which redirect all url to https.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         httpsredirect = ovh.ip_load_balancing.HttpRoute("httpsredirect",
             action=ovh.ip_load_balancing.HttpRouteActionArgs(
                 status=302,
                 target="https://${host}${path}${arguments}",
                 type="redirect",
             ),
             display_name="Redirect to HTTPS",
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP route can be imported using the following format `service_name` and the `id` of the route separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -275,30 +273,28 @@
         """
         Manage HTTP route for a loadbalancer service
 
         ## Example Usage
 
         Route which redirect all url to https.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         httpsredirect = ovh.ip_load_balancing.HttpRoute("httpsredirect",
             action=ovh.ip_load_balancing.HttpRouteActionArgs(
                 status=302,
                 target="https://${host}${path}${arguments}",
                 type="redirect",
             ),
             display_name="Redirect to HTTPS",
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP route can be imported using the following format `service_name` and the `id` of the route separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param HttpRouteArgs args: The arguments to use to populate this resource's properties.
@@ -365,15 +361,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['HttpRouteActionArgs']] action: Action triggered when all rules match
         :param pulumi.Input[str] display_name: Human readable name for your route, this field is for you
         :param pulumi.Input[int] frontend_id: Route traffic for this frontend
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['HttpRouteRuleArgs']]]] rules: List of rules to match to trigger action
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] status: HTTP status code for "redirect" and "reject" actions
+        :param pulumi.Input[str] status: Route status. Routes in "ok" state are ready to operate
         :param pulumi.Input[int] weight: Route priority ([0..255]). 0 if null. Highest priority routes are evaluated first. Only the first matching route will trigger an action
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HttpRouteState.__new__(_HttpRouteState)
 
         __props__.__dict__["action"] = action
@@ -425,15 +421,15 @@
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
-        HTTP status code for "redirect" and "reject" actions
+        Route status. Routes in "ok" state are ready to operate
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def weight(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/http_route_rule.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/http_route_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,15 +296,14 @@
         """
         Manage rules for HTTP route.
 
         ## Example Usage
 
         Route which redirect all URL to HTTPs for example.com (Vhost).
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         httpsredirect = ovh.ip_load_balancing.HttpRoute("httpsredirect",
             action=ovh.ip_load_balancing.HttpRouteActionArgs(
                 status=302,
@@ -320,34 +319,31 @@
             field="host",
             match="is",
             negate=False,
             pattern="example.com",
             route_id=httpsredirect.id,
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         Rule which match a specific header (same effect as the host match above).
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         examplerule = ovh.ip_load_balancing.HttpRouteRule("examplerule",
             display_name="Match example.com Host header",
             field="headers",
             match="is",
             negate=False,
             pattern="example.com",
             route_id=ovh_iploadbalancing_http_route["httpsredirect"]["id"],
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             sub_field="Host")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP route rule can be imported using the following format `service_name`, the `id` of the route and the `id` of the rule separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -369,15 +365,14 @@
         """
         Manage rules for HTTP route.
 
         ## Example Usage
 
         Route which redirect all URL to HTTPs for example.com (Vhost).
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         httpsredirect = ovh.ip_load_balancing.HttpRoute("httpsredirect",
             action=ovh.ip_load_balancing.HttpRouteActionArgs(
                 status=302,
@@ -393,34 +388,31 @@
             field="host",
             match="is",
             negate=False,
             pattern="example.com",
             route_id=httpsredirect.id,
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         Rule which match a specific header (same effect as the host match above).
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         examplerule = ovh.ip_load_balancing.HttpRouteRule("examplerule",
             display_name="Match example.com Host header",
             field="headers",
             match="is",
             negate=False,
             pattern="example.com",
             route_id=ovh_iploadbalancing_http_route["httpsredirect"]["id"],
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             sub_field="Host")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         HTTP route rule can be imported using the following format `service_name`, the `id` of the route and the `id` of the rule separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param HttpRouteRuleInitArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/load_balancer.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/load_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 
 @pulumi.input_type
 class LoadBalancerArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['LoadBalancerPlanArgs'],
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['LoadBalancerOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['LoadBalancerPlanOptionArgs']]]] = None,
                  ssl_configuration: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a LoadBalancer resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['LoadBalancerPlanArgs'] plan: Product Plan to order
         :param pulumi.Input[str] display_name: Set the name displayed in ManagerV6 for your iplb (max 50 chars)
+        :param pulumi.Input[Sequence[pulumi.Input['LoadBalancerOrderArgs']]] orders: Details about an Order
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['LoadBalancerPlanOptionArgs']]] plan_options: Product Plan to order
         :param pulumi.Input[str] ssl_configuration: Modern oldest compatible clients : Firefox 27, Chrome 30, IE 11 on Windows 7, Edge, Opera 17, Safari 9, Android 5.0, and Java 8. Intermediate oldest compatible clients : Firefox 1, Chrome 1, IE 7, Opera 5, Safari 1, Windows XP IE8, Android 2.3, Java 7. Intermediate if null. one of "intermediate", "modern".
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -78,14 +82,26 @@
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['LoadBalancerOrderArgs']]]]:
+        """
+        Details about an Order
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['LoadBalancerOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -441,24 +457,24 @@
 
 class LoadBalancer(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['LoadBalancerPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerPlanOptionArgs']]]]] = None,
                  ssl_configuration: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         iplb = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -480,19 +496,19 @@
             ),
             plan_options=[ovh.ip_load_balancing.LoadBalancerPlanOptionArgs(
                 duration=bhs.selected_prices[0].duration,
                 plan_code=bhs.plan_code,
                 pricing_mode=bhs.selected_prices[0].pricing_mode,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] display_name: Set the name displayed in ManagerV6 for your iplb (max 50 chars)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerOrderArgs']]]] orders: Details about an Order
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['LoadBalancerPlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerPlanOptionArgs']]]] plan_options: Product Plan to order
         :param pulumi.Input[str] ssl_configuration: Modern oldest compatible clients : Firefox 27, Chrome 30, IE 11 on Windows 7, Edge, Opera 17, Safari 9, Android 5.0, and Java 8. Intermediate oldest compatible clients : Firefox 1, Chrome 1, IE 7, Opera 5, Safari 1, Windows XP IE8, Android 2.3, Java 7. Intermediate if null. one of "intermediate", "modern".
         """
         ...
@@ -500,15 +516,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: LoadBalancerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         iplb = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -530,15 +545,14 @@
             ),
             plan_options=[ovh.ip_load_balancing.LoadBalancerPlanOptionArgs(
                 duration=bhs.selected_prices[0].duration,
                 plan_code=bhs.plan_code,
                 pricing_mode=bhs.selected_prices[0].pricing_mode,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param LoadBalancerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -548,14 +562,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['LoadBalancerPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['LoadBalancerPlanOptionArgs']]]]] = None,
                  ssl_configuration: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -563,14 +578,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LoadBalancerArgs.__new__(LoadBalancerArgs)
 
             __props__.__dict__["display_name"] = display_name
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
@@ -579,15 +595,14 @@
             __props__.__dict__["load_balancer_urn"] = None
             __props__.__dict__["ip_loadbalancing"] = None
             __props__.__dict__["ipv4"] = None
             __props__.__dict__["ipv6"] = None
             __props__.__dict__["metrics_token"] = None
             __props__.__dict__["offer"] = None
             __props__.__dict__["orderable_zones"] = None
-            __props__.__dict__["orders"] = None
             __props__.__dict__["service_name"] = None
             __props__.__dict__["state"] = None
             __props__.__dict__["vrack_eligibility"] = None
             __props__.__dict__["vrack_name"] = None
             __props__.__dict__["zones"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["metricsToken"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: Optional[str] = None,
                  plan_code: Optional[str] = None):
         """
         :param str name: The zone three letter code
-        :param str plan_code: Plan code
+        :param str plan_code: The billing planCode for this zone
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if plan_code is not None:
             pulumi.set(__self__, "plan_code", plan_code)
 
     @property
@@ -483,15 +483,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="planCode")
     def plan_code(self) -> Optional[str]:
         """
-        Plan code
+        The billing planCode for this zone
         """
         return pulumi.get(self, "plan_code")
 
 
 @pulumi.output_type
 class LoadBalancerPlan(dict):
     @staticmethod
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/refresh.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/dedicated_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,252 +5,225 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['RefreshArgs', 'Refresh']
+__all__ = ['DedicatedServerArgs', 'DedicatedServer']
 
 @pulumi.input_type
-class RefreshArgs:
+class DedicatedServerArgs:
     def __init__(__self__, *,
-                 keepers: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 server_id: pulumi.Input[str],
                  service_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a Refresh resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        The set of arguments for constructing a DedicatedServer resource.
+        :param pulumi.Input[str] server_id: The id of the dedicated server.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        pulumi.set(__self__, "keepers", keepers)
+        pulumi.set(__self__, "server_id", server_id)
         pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter
-    def keepers(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    @pulumi.getter(name="serverId")
+    def server_id(self) -> pulumi.Input[str]:
         """
-        List of values tracked to trigger refresh, used also to form implicit dependencies
+        The id of the dedicated server.
         """
-        return pulumi.get(self, "keepers")
+        return pulumi.get(self, "server_id")
 
-    @keepers.setter
-    def keepers(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "keepers", value)
+    @server_id.setter
+    def server_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "server_id", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The internal name of your IP load balancing
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
 
 @pulumi.input_type
-class _RefreshState:
+class _DedicatedServerState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 server_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Refresh resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        Input properties used for looking up and filtering DedicatedServer resources.
+        :param pulumi.Input[str] server_id: The id of the dedicated server.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        if keepers is not None:
-            pulumi.set(__self__, "keepers", keepers)
+        if server_id is not None:
+            pulumi.set(__self__, "server_id", server_id)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="serverId")
+    def server_id(self) -> Optional[pulumi.Input[str]]:
         """
-        List of values tracked to trigger refresh, used also to form implicit dependencies
+        The id of the dedicated server.
         """
-        return pulumi.get(self, "keepers")
+        return pulumi.get(self, "server_id")
 
-    @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "keepers", value)
+    @server_id.setter
+    def server_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "server_id", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The internal name of your IP load balancing
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
 
-class Refresh(pulumi.CustomResource):
+class DedicatedServer(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 server_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Applies changes from other `ovh_iploadbalancing_*` resources to the production configuration of loadbalancers.
+        Attach a legacy dedicated server to a vRack.
+
+        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
+        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
-            state="ok")
-        farmname = ovh.ip_load_balancing.TcpFarm("farmname",
-            port=8080,
-            service_name=lb.service_name,
-            zone="all")
-        backend = ovh.ip_load_balancing.TcpFarmServer("backend",
-            address="4.5.6.7",
-            backup=True,
-            display_name="mybackend",
-            farm_id=farmname.id,
-            port=80,
-            probe=True,
-            proxy_protocol_version="v2",
-            service_name=lb.service_name,
-            ssl=False,
-            status="active",
-            weight=2)
-        mylb = ovh.ip_load_balancing.Refresh("mylb",
-            keepers=[[__item.address for __item in [backend]]],
-            service_name=lb.service_name)
+        vds = ovh.vrack.DedicatedServer("vds",
+            server_id="67890",
+            service_name="XXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] server_id: The id of the dedicated server.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: RefreshArgs,
+                 args: DedicatedServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Applies changes from other `ovh_iploadbalancing_*` resources to the production configuration of loadbalancers.
+        Attach a legacy dedicated server to a vRack.
+
+        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
+        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
-            state="ok")
-        farmname = ovh.ip_load_balancing.TcpFarm("farmname",
-            port=8080,
-            service_name=lb.service_name,
-            zone="all")
-        backend = ovh.ip_load_balancing.TcpFarmServer("backend",
-            address="4.5.6.7",
-            backup=True,
-            display_name="mybackend",
-            farm_id=farmname.id,
-            port=80,
-            probe=True,
-            proxy_protocol_version="v2",
-            service_name=lb.service_name,
-            ssl=False,
-            status="active",
-            weight=2)
-        mylb = ovh.ip_load_balancing.Refresh("mylb",
-            keepers=[[__item.address for __item in [backend]]],
-            service_name=lb.service_name)
+        vds = ovh.vrack.DedicatedServer("vds",
+            server_id="67890",
+            service_name="XXXX")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
-        :param RefreshArgs args: The arguments to use to populate this resource's properties.
+        :param DedicatedServerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(RefreshArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DedicatedServerArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 server_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = RefreshArgs.__new__(RefreshArgs)
+            __props__ = DedicatedServerArgs.__new__(DedicatedServerArgs)
 
-            if keepers is None and not opts.urn:
-                raise TypeError("Missing required property 'keepers'")
-            __props__.__dict__["keepers"] = keepers
+            if server_id is None and not opts.urn:
+                raise TypeError("Missing required property 'server_id'")
+            __props__.__dict__["server_id"] = server_id
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
-        super(Refresh, __self__).__init__(
-            'ovh:IpLoadBalancing/refresh:Refresh',
+        super(DedicatedServer, __self__).__init__(
+            'ovh:Vrack/dedicatedServer:DedicatedServer',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            service_name: Optional[pulumi.Input[str]] = None) -> 'Refresh':
+            server_id: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'DedicatedServer':
         """
-        Get an existing Refresh resource's state with the given name, id, and optional extra
+        Get an existing DedicatedServer resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] keepers: List of values tracked to trigger refresh, used also to form implicit dependencies
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] server_id: The id of the dedicated server.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _RefreshState.__new__(_RefreshState)
+        __props__ = _DedicatedServerState.__new__(_DedicatedServerState)
 
-        __props__.__dict__["keepers"] = keepers
+        __props__.__dict__["server_id"] = server_id
         __props__.__dict__["service_name"] = service_name
-        return Refresh(resource_name, opts=opts, __props__=__props__)
+        return DedicatedServer(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def keepers(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="serverId")
+    def server_id(self) -> pulumi.Output[str]:
         """
-        List of values tracked to trigger refresh, used also to form implicit dependencies
+        The id of the dedicated server.
         """
-        return pulumi.get(self, "keepers")
+        return pulumi.get(self, "server_id")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The internal name of your IP load balancing
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_farm.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_farm.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  vrack_network_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a TcpFarm resource.
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input['TcpFarmProbeArgs'] probe: define a backend healthcheck probe
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         """
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "zone", zone)
         if balance is not None:
@@ -98,15 +98,15 @@
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -158,15 +158,15 @@
                  stickiness: Optional[pulumi.Input[str]] = None,
                  vrack_network_id: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TcpFarm resources.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input['TcpFarmProbeArgs'] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         if balance is not None:
@@ -210,15 +210,15 @@
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -298,37 +298,35 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a backend server group (farm) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.TcpFarm("farmname",
             display_name="ingress-8080-gra",
             service_name=lb.service_name,
             zone="GRA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP Farm can be imported using the following format `service_name` and the `id` of the farm, separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input[pulumi.InputType['TcpFarmProbeArgs']] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         ...
@@ -338,27 +336,25 @@
                  args: TcpFarmArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend server group (farm) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.TcpFarm("farmname",
             display_name="ingress-8080-gra",
             service_name=lb.service_name,
             zone="GRA")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP Farm can be imported using the following format `service_name` and the `id` of the farm, separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param TcpFarmArgs args: The arguments to use to populate this resource's properties.
@@ -427,15 +423,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] balance: Load balancing algorithm. `roundrobin` if null (`first`, `leastconn`, `roundrobin`, `source`)
         :param pulumi.Input[str] display_name: Readable label for loadbalancer farm
-        :param pulumi.Input[int] port: Port for backends to receive traffic on.
+        :param pulumi.Input[int] port: Port attached to your farm ([1..49151]). Inherited from frontend if null
         :param pulumi.Input[pulumi.InputType['TcpFarmProbeArgs']] probe: define a backend healthcheck probe
         :param pulumi.Input[str] service_name: The internal name of your IP load balancing
         :param pulumi.Input[str] stickiness: Stickiness type. No stickiness if null (`sourceIp`)
         :param pulumi.Input[int] vrack_network_id: Internal Load Balancer identifier of the vRack private network to attach to your farm, mandatory when your Load Balancer is attached to a vRack
         :param pulumi.Input[str] zone: Zone where the farm will be defined (ie. `GRA`, `BHS` also supports `ALL`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -468,15 +464,15 @@
         """
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter
     def port(self) -> pulumi.Output[Optional[int]]:
         """
-        Port for backends to receive traffic on.
+        Port attached to your farm ([1..49151]). Inherited from frontend if null
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter
     def probe(self) -> pulumi.Output[Optional['outputs.TcpFarmProbe']]:
         """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_farm_server.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,15 +451,14 @@
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Creates a backend server entry linked to loadbalancing group (farm)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.TcpFarm("farmname",
@@ -475,15 +474,14 @@
             probe=True,
             proxy_protocol_version="v2",
             service_name=lb.service_name,
             ssl=False,
             status="active",
             weight=2)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP farm server can be imported using the following format `service_name`, the `id` of the farm and the `id` of the server separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -507,15 +505,14 @@
                  args: TcpFarmServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend server entry linked to loadbalancing group (farm)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farmname = ovh.ip_load_balancing.TcpFarm("farmname",
@@ -531,15 +528,14 @@
             probe=True,
             proxy_protocol_version="v2",
             service_name=lb.service_name,
             ssl=False,
             status="active",
             weight=2)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP farm server can be imported using the following format `service_name`, the `id` of the farm and the `id` of the server separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param TcpFarmServerArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_frontend.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,14 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.TcpFarm("farm80",
@@ -388,15 +387,14 @@
         testfrontend = ovh.ip_load_balancing.TcpFrontend("testfrontend",
             default_farm_id=farm80.id,
             display_name="ingress-8080-gra",
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP frontend can be imported using the following format `service_name` and the `id` of the frontend separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -420,15 +418,14 @@
                  args: TcpFrontendArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         farm80 = ovh.ip_load_balancing.TcpFarm("farm80",
@@ -439,15 +436,14 @@
         testfrontend = ovh.ip_load_balancing.TcpFrontend("testfrontend",
             default_farm_id=farm80.id,
             display_name="ingress-8080-gra",
             port="80,443",
             service_name=lb.service_name,
             zone="all")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP frontend can be imported using the following format `service_name` and the `id` of the frontend separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param TcpFrontendArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_route.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,27 +231,25 @@
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manage TCP route for a loadbalancer service
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         tcpreject = ovh.ip_load_balancing.TcpRoute("tcpreject",
             action=ovh.ip_load_balancing.TcpRouteActionArgs(
                 type="reject",
             ),
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP route can be imported using the following format `service_name` and the `id` of the route separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -268,27 +266,25 @@
                  args: TcpRouteArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage TCP route for a loadbalancer service
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         tcpreject = ovh.ip_load_balancing.TcpRoute("tcpreject",
             action=ovh.ip_load_balancing.TcpRouteActionArgs(
                 type="reject",
             ),
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP route can be imported using the following format `service_name` and the `id` of the route separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param TcpRouteArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/tcp_route_rule.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,14 @@
                  sub_field: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage rules for TCP route.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         reject = ovh.ip_load_balancing.TcpRoute("reject",
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1,
@@ -315,15 +314,14 @@
             route_id=reject.id,
             display_name="Match example.com host",
             field="sni",
             match="is",
             negate=False,
             pattern="example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP route rule can be imported using the following format `service_name`, the `id` of the route and the `id` of the rule separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -343,15 +341,14 @@
                  args: TcpRouteRuleInitArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage rules for TCP route.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         reject = ovh.ip_load_balancing.TcpRoute("reject",
             service_name="loadbalancer-xxxxxxxxxxxxxxxxxx",
             weight=1,
@@ -364,15 +361,14 @@
             route_id=reject.id,
             display_name="Match example.com host",
             field="sni",
             match="is",
             negate=False,
             pattern="example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         TCP route rule can be imported using the following format `service_name`, the `id` of the route and the `id` of the rule separated by "/" e.g.
 
         :param str resource_name: The name of the resource.
         :param TcpRouteRuleInitArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/udp_frontend.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/udp_frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,28 +286,26 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
             service_name=lb.service_name,
             display_name="ingress-8080-gra",
             zone="all",
             port="10,11")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
         :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
         :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
         :param pulumi.Input[str] display_name: Human readable name for your frontend
@@ -324,28 +322,26 @@
                  args: UdpFrontendArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
             state="ok")
         testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
             service_name=lb.service_name,
             display_name="ingress-8080-gra",
             zone="all",
             port="10,11")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UdpFrontendArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/iploadbalancing/vrack_network.py` & `pulumi_ovh-0.44.0/pulumi_ovh/iploadbalancing/vrack_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 from .get_identity_user import *
 from .get_identity_users import *
 from .get_installation_template import *
 from .get_installation_templates import *
 from .get_me import *
 from .get_paymentmean_bank_account import *
 from .get_paymentmean_credit_card import *
-from .get_ssh_key import *
-from .get_ssh_keys import *
 from .identity_group import *
 from .identity_user import *
 from .installation_template import *
 from .installation_template_partition_scheme import *
 from .installation_template_partition_scheme_hardware_raid import *
 from .installation_template_partition_scheme_partition import *
-from .ssh_key import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/_inputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,40 +7,34 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'InstallationTemplateCustomizationArgs',
+    'InstallationTemplateInputArgs',
 ]
 
 @pulumi.input_type
 class InstallationTemplateCustomizationArgs:
     def __init__(__self__, *,
                  custom_hostname: Optional[pulumi.Input[str]] = None,
                  post_installation_script_link: Optional[pulumi.Input[str]] = None,
-                 post_installation_script_return: Optional[pulumi.Input[str]] = None,
-                 ssh_key_name: Optional[pulumi.Input[str]] = None):
+                 post_installation_script_return: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param pulumi.Input[str] post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param pulumi.Input[str] ssh_key_name: Deprecated.
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if ssh_key_name is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-            pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
-        if ssh_key_name is not None:
-            pulumi.set(__self__, "ssh_key_name", ssh_key_name)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[pulumi.Input[str]]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -70,23 +64,91 @@
         """
         return pulumi.get(self, "post_installation_script_return")
 
     @post_installation_script_return.setter
     def post_installation_script_return(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "post_installation_script_return", value)
 
+
+@pulumi.input_type
+class InstallationTemplateInputArgs:
+    def __init__(__self__, *,
+                 default: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 enums: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 mandatory: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] description: information about this template.
+        """
+        if default is not None:
+            pulumi.set(__self__, "default", default)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if enums is not None:
+            pulumi.set(__self__, "enums", enums)
+        if mandatory is not None:
+            pulumi.set(__self__, "mandatory", mandatory)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
     @property
-    @pulumi.getter(name="sshKeyName")
-    def ssh_key_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def default(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default")
+
+    @default.setter
+    def default(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Deprecated.
+        information about this template.
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
+        return pulumi.get(self, "description")
 
-        return pulumi.get(self, "ssh_key_name")
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
-    @ssh_key_name.setter
-    def ssh_key_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ssh_key_name", value)
+    @property
+    @pulumi.getter
+    def enums(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "enums")
+
+    @enums.setter
+    def enums(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "enums", value)
+
+    @property
+    @pulumi.getter
+    def mandatory(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "mandatory")
+
+    @mandatory.setter
+    def mandatory(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mandatory", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/apio_auth2_client.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/apio_auth2_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,38 +214,34 @@
         """
         Creates an OAuth2 service account.
 
         ## Example Usage
 
         An OAuth2 client for an app hosted at `my-app.com`, that uses the authorization code flow to authenticate.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oauth2_client_auth_code = ovh.me.APIOAuth2Client("myOauth2ClientAuthCode",
             callback_urls=["https://my-app.com/callback"],
             description="An OAuth2 client using the authorization code flow for my-app.com",
             flow="AUTHORIZATION_CODE")
         ```
-        <!--End PulumiCodeChooser -->
 
         An OAuth2 client for an app hosted at `my-app.com`, that uses the client credentials flow to authenticate.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oauth2_client_client_creds = ovh.me.APIOAuth2Client("myOauth2ClientClientCreds",
             description="An OAuth2 client using the client credentials flow for my app",
             flow="CLIENT_CREDENTIALS")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OAuth2 clients can be imported using their `client_id`:
 
         bash
 
@@ -277,38 +273,34 @@
         """
         Creates an OAuth2 service account.
 
         ## Example Usage
 
         An OAuth2 client for an app hosted at `my-app.com`, that uses the authorization code flow to authenticate.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oauth2_client_auth_code = ovh.me.APIOAuth2Client("myOauth2ClientAuthCode",
             callback_urls=["https://my-app.com/callback"],
             description="An OAuth2 client using the authorization code flow for my-app.com",
             flow="AUTHORIZATION_CODE")
         ```
-        <!--End PulumiCodeChooser -->
 
         An OAuth2 client for an app hosted at `my-app.com`, that uses the client credentials flow to authenticate.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_oauth2_client_client_creds = ovh.me.APIOAuth2Client("myOauth2ClientClientCreds",
             description="An OAuth2 client using the client credentials flow for my app",
             flow="CLIENT_CREDENTIALS")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         OAuth2 clients can be imported using their `client_id`:
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_apio_auth2_client.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_apio_auth2_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,22 +116,20 @@
 def get_apio_auth2_client(client_id: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAPIOAuth2ClientResult:
     """
     Use this data source to retrieve information about an existing OAuth2 service account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oauth2_client = ovh.Me.get_apio_auth2_client(client_id="5f8969a993ec8b4b")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: Client ID of an existing OAuth2 service account.
     """
     __args__ = dict()
     __args__['clientId'] = client_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -151,20 +149,18 @@
 def get_apio_auth2_client_output(client_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAPIOAuth2ClientResult]:
     """
     Use this data source to retrieve information about an existing OAuth2 service account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oauth2_client = ovh.Me.get_apio_auth2_client(client_id="5f8969a993ec8b4b")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str client_id: Client ID of an existing OAuth2 service account.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_apio_auth2_clients.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_apio_auth2_clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_apio_auth2_clients(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAPIOAuth2ClientsResult:
     """
     Use this data source to retrieve information the list of existing OAuth2 service account IDs.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oauth2_clients = ovh.Me.get_apio_auth2_client()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getAPIOAuth2Clients:getAPIOAuth2Clients', __args__, opts=opts, typ=GetAPIOAuth2ClientsResult).value
 
     return AwaitableGetAPIOAuth2ClientsResult(
         client_ids=pulumi.get(__ret__, 'client_ids'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_apio_auth2_clients)
 def get_apio_auth2_clients_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAPIOAuth2ClientsResult]:
     """
     Use this data source to retrieve information the list of existing OAuth2 service account IDs.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_oauth2_clients = ovh.Me.get_apio_auth2_client()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 ]
 
 @pulumi.output_type
 class GetIdentityGroupResult:
     """
     A collection of values returned by getIdentityGroup.
     """
-    def __init__(__self__, creation=None, default_group=None, description=None, id=None, last_update=None, name=None, role=None):
+    def __init__(__self__, group_urn=None, creation=None, default_group=None, description=None, id=None, last_update=None, name=None, role=None):
+        if group_urn and not isinstance(group_urn, str):
+            raise TypeError("Expected argument 'group_urn' to be a str")
+        pulumi.set(__self__, "group_urn", group_urn)
         if creation and not isinstance(creation, str):
             raise TypeError("Expected argument 'creation' to be a str")
         pulumi.set(__self__, "creation", creation)
         if default_group and not isinstance(default_group, bool):
             raise TypeError("Expected argument 'default_group' to be a bool")
         pulumi.set(__self__, "default_group", default_group)
         if description and not isinstance(description, str):
@@ -41,14 +44,22 @@
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if role and not isinstance(role, str):
             raise TypeError("Expected argument 'role' to be a str")
         pulumi.set(__self__, "role", role)
 
     @property
+    @pulumi.getter(name="GroupURN")
+    def group_urn(self) -> str:
+        """
+        Identity URN of the group.
+        """
+        return pulumi.get(self, "group_urn")
+
+    @property
     @pulumi.getter
     def creation(self) -> str:
         """
         Creation date of this group.
         """
         return pulumi.get(self, "creation")
 
@@ -100,14 +111,15 @@
 
 class AwaitableGetIdentityGroupResult(GetIdentityGroupResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetIdentityGroupResult(
+            group_urn=self.group_urn,
             creation=self.creation,
             default_group=self.default_group,
             description=self.description,
             id=self.id,
             last_update=self.last_update,
             name=self.name,
             role=self.role)
@@ -116,32 +128,31 @@
 def get_identity_group(name: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIdentityGroupResult:
     """
     Use this data source to retrieve information about an identity group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_group = ovh.Me.get_identity_group(name="my_group_name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Group name.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getIdentityGroup:getIdentityGroup', __args__, opts=opts, typ=GetIdentityGroupResult).value
 
     return AwaitableGetIdentityGroupResult(
+        group_urn=pulumi.get(__ret__, 'group_urn'),
         creation=pulumi.get(__ret__, 'creation'),
         default_group=pulumi.get(__ret__, 'default_group'),
         description=pulumi.get(__ret__, 'description'),
         id=pulumi.get(__ret__, 'id'),
         last_update=pulumi.get(__ret__, 'last_update'),
         name=pulumi.get(__ret__, 'name'),
         role=pulumi.get(__ret__, 'role'))
@@ -151,20 +162,18 @@
 def get_identity_group_output(name: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIdentityGroupResult]:
     """
     Use this data source to retrieve information about an identity group.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_group = ovh.Me.get_identity_group(name="my_group_name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Group name.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_groups.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_identity_groups(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIdentityGroupsResult:
     """
     Use this data source to retrieve the list of the account's identity groups
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     groups = ovh.Me.get_identity_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getIdentityGroups:getIdentityGroups', __args__, opts=opts, typ=GetIdentityGroupsResult).value
 
     return AwaitableGetIdentityGroupsResult(
         groups=pulumi.get(__ret__, 'groups'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_identity_groups)
 def get_identity_groups_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIdentityGroupsResult]:
     """
     Use this data source to retrieve the list of the account's identity groups
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     groups = ovh.Me.get_identity_groups()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,22 +164,20 @@
 def get_identity_user(user: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIdentityUserResult:
     """
     Use this data source to retrieve information about an identity user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_user = ovh.Me.get_identity_user(user="my_user_login")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user: User's login.
     """
     __args__ = dict()
     __args__['user'] = user
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -203,20 +201,18 @@
 def get_identity_user_output(user: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIdentityUserResult]:
     """
     Use this data source to retrieve information about an identity user.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     my_user = ovh.Me.get_identity_user(user="my_user_login")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str user: User's login.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_identity_users.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_identity_users.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_identity_users(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIdentityUsersResult:
     """
     Use this data source to retrieve list of user logins of the account's identity users.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     users = ovh.Me.get_identity_users()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getIdentityUsers:getIdentityUsers', __args__, opts=opts, typ=GetIdentityUsersResult).value
 
     return AwaitableGetIdentityUsersResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_identity_users)
 def get_identity_users_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIdentityUsersResult]:
     """
     Use this data source to retrieve list of user logins of the account's identity users.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     users = ovh.Me.get_identity_users()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_installation_template.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_installation_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,239 +18,277 @@
 ]
 
 @pulumi.output_type
 class GetInstallationTemplateResult:
     """
     A collection of values returned by getInstallationTemplate.
     """
-    def __init__(__self__, available_languages=None, bit_format=None, category=None, customizations=None, default_language=None, description=None, distribution=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, lvm_ready=None, partition_schemes=None, template_name=None):
-        if available_languages and not isinstance(available_languages, list):
-            raise TypeError("Expected argument 'available_languages' to be a list")
-        pulumi.set(__self__, "available_languages", available_languages)
+    def __init__(__self__, bit_format=None, category=None, customizations=None, description=None, distribution=None, end_of_install=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, inputs=None, lvm_ready=None, no_partitioning=None, partition_schemes=None, soft_raid_only_mirroring=None, subfamily=None, template_name=None):
         if bit_format and not isinstance(bit_format, int):
             raise TypeError("Expected argument 'bit_format' to be a int")
         pulumi.set(__self__, "bit_format", bit_format)
         if category and not isinstance(category, str):
             raise TypeError("Expected argument 'category' to be a str")
         pulumi.set(__self__, "category", category)
         if customizations and not isinstance(customizations, list):
             raise TypeError("Expected argument 'customizations' to be a list")
         pulumi.set(__self__, "customizations", customizations)
-        if default_language and not isinstance(default_language, str):
-            raise TypeError("Expected argument 'default_language' to be a str")
-        pulumi.set(__self__, "default_language", default_language)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if distribution and not isinstance(distribution, str):
             raise TypeError("Expected argument 'distribution' to be a str")
         pulumi.set(__self__, "distribution", distribution)
+        if end_of_install and not isinstance(end_of_install, str):
+            raise TypeError("Expected argument 'end_of_install' to be a str")
+        pulumi.set(__self__, "end_of_install", end_of_install)
         if family and not isinstance(family, str):
             raise TypeError("Expected argument 'family' to be a str")
         pulumi.set(__self__, "family", family)
         if filesystems and not isinstance(filesystems, list):
             raise TypeError("Expected argument 'filesystems' to be a list")
         pulumi.set(__self__, "filesystems", filesystems)
         if hard_raid_configuration and not isinstance(hard_raid_configuration, bool):
             raise TypeError("Expected argument 'hard_raid_configuration' to be a bool")
         pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if inputs and not isinstance(inputs, list):
+            raise TypeError("Expected argument 'inputs' to be a list")
+        pulumi.set(__self__, "inputs", inputs)
         if lvm_ready and not isinstance(lvm_ready, bool):
             raise TypeError("Expected argument 'lvm_ready' to be a bool")
         pulumi.set(__self__, "lvm_ready", lvm_ready)
+        if no_partitioning and not isinstance(no_partitioning, bool):
+            raise TypeError("Expected argument 'no_partitioning' to be a bool")
+        pulumi.set(__self__, "no_partitioning", no_partitioning)
         if partition_schemes and not isinstance(partition_schemes, list):
             raise TypeError("Expected argument 'partition_schemes' to be a list")
         pulumi.set(__self__, "partition_schemes", partition_schemes)
+        if soft_raid_only_mirroring and not isinstance(soft_raid_only_mirroring, bool):
+            raise TypeError("Expected argument 'soft_raid_only_mirroring' to be a bool")
+        pulumi.set(__self__, "soft_raid_only_mirroring", soft_raid_only_mirroring)
+        if subfamily and not isinstance(subfamily, str):
+            raise TypeError("Expected argument 'subfamily' to be a str")
+        pulumi.set(__self__, "subfamily", subfamily)
         if template_name and not isinstance(template_name, str):
             raise TypeError("Expected argument 'template_name' to be a str")
         pulumi.set(__self__, "template_name", template_name)
 
     @property
-    @pulumi.getter(name="availableLanguages")
-    def available_languages(self) -> Sequence[str]:
-        """
-        List of all language available for this template. Deprecated, will be removed in next release.
-        """
-        return pulumi.get(self, "available_languages")
-
-    @property
     @pulumi.getter(name="bitFormat")
     def bit_format(self) -> int:
         """
-        This template bit format (32 or 64).
+        Template bit format (32 or 64).
         """
         return pulumi.get(self, "bit_format")
 
     @property
     @pulumi.getter
     def category(self) -> str:
         """
-        Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
+        Category of this template (informative only).
         """
         return pulumi.get(self, "category")
 
     @property
     @pulumi.getter
     def customizations(self) -> Sequence['outputs.GetInstallationTemplateCustomizationResult']:
         return pulumi.get(self, "customizations")
 
     @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> str:
-        """
-        The default language of this template. Deprecated, will be removed in next release.
-        """
-        warnings.warn("""This field will be removed from the API, please use `userMetadata` instead.""", DeprecationWarning)
-        pulumi.log.warn("""default_language is deprecated: This field will be removed from the API, please use `userMetadata` instead.""")
-
-        return pulumi.get(self, "default_language")
-
-    @property
     @pulumi.getter
     def description(self) -> str:
         """
-        information about this template.
+        Information about this template.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def distribution(self) -> str:
         """
-        the distribution this template is based on.
+        Distribution this template is based on.
         """
         return pulumi.get(self, "distribution")
 
     @property
+    @pulumi.getter(name="endOfInstall")
+    def end_of_install(self) -> str:
+        """
+        End of install date of the template.
+        """
+        return pulumi.get(self, "end_of_install")
+
+    @property
     @pulumi.getter
     def family(self) -> str:
         """
-        this template family type (bsd,linux,solaris,windows).
+        Template family type (bsd,linux,solaris,windows).
         """
         return pulumi.get(self, "family")
 
     @property
     @pulumi.getter
     def filesystems(self) -> Sequence[str]:
         """
-        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        Filesystems available.
         """
         return pulumi.get(self, "filesystems")
 
     @property
     @pulumi.getter(name="hardRaidConfiguration")
     def hard_raid_configuration(self) -> bool:
         """
-        This distribution supports hardware raid configuration through the OVHcloud API.
+        Distribution supports hardware raid configuration through the OVHcloud API.
         """
+        warnings.warn("""This will be deprecated in the next release""", DeprecationWarning)
+        pulumi.log.warn("""hard_raid_configuration is deprecated: This will be deprecated in the next release""")
+
         return pulumi.get(self, "hard_raid_configuration")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter
+    def inputs(self) -> Sequence['outputs.GetInstallationTemplateInputResult']:
+        """
+        Represents the questions of the expected answers in the userMetadata field.
+        """
+        return pulumi.get(self, "inputs")
+
+    @property
     @pulumi.getter(name="lvmReady")
     def lvm_ready(self) -> bool:
+        """
+        Whether this template supports LVM.
+        """
         return pulumi.get(self, "lvm_ready")
 
     @property
+    @pulumi.getter(name="noPartitioning")
+    def no_partitioning(self) -> bool:
+        """
+        Partitioning customization is not available for this OS template.
+        """
+        return pulumi.get(self, "no_partitioning")
+
+    @property
     @pulumi.getter(name="partitionSchemes")
     def partition_schemes(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemeResult']:
         return pulumi.get(self, "partition_schemes")
 
     @property
+    @pulumi.getter(name="softRaidOnlyMirroring")
+    def soft_raid_only_mirroring(self) -> bool:
+        """
+        Template supports RAID0 and RAID1 on 2 disks.
+        """
+        return pulumi.get(self, "soft_raid_only_mirroring")
+
+    @property
+    @pulumi.getter
+    def subfamily(self) -> str:
+        """
+        Subfamily of the template.
+        """
+        return pulumi.get(self, "subfamily")
+
+    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> str:
         return pulumi.get(self, "template_name")
 
 
 class AwaitableGetInstallationTemplateResult(GetInstallationTemplateResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetInstallationTemplateResult(
-            available_languages=self.available_languages,
             bit_format=self.bit_format,
             category=self.category,
             customizations=self.customizations,
-            default_language=self.default_language,
             description=self.description,
             distribution=self.distribution,
+            end_of_install=self.end_of_install,
             family=self.family,
             filesystems=self.filesystems,
             hard_raid_configuration=self.hard_raid_configuration,
             id=self.id,
+            inputs=self.inputs,
             lvm_ready=self.lvm_ready,
+            no_partitioning=self.no_partitioning,
             partition_schemes=self.partition_schemes,
+            soft_raid_only_mirroring=self.soft_raid_only_mirroring,
+            subfamily=self.subfamily,
             template_name=self.template_name)
 
 
 def get_installation_template(template_name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstallationTemplateResult:
     """
     Use this data source to get a custom installation template available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mytemplate = ovh.Me.get_installation_template(template_name="mytemplate")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str template_name: This template name
+    :param str template_name: Template name.
     """
     __args__ = dict()
     __args__['templateName'] = template_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getInstallationTemplate:getInstallationTemplate', __args__, opts=opts, typ=GetInstallationTemplateResult).value
 
     return AwaitableGetInstallationTemplateResult(
-        available_languages=pulumi.get(__ret__, 'available_languages'),
         bit_format=pulumi.get(__ret__, 'bit_format'),
         category=pulumi.get(__ret__, 'category'),
         customizations=pulumi.get(__ret__, 'customizations'),
-        default_language=pulumi.get(__ret__, 'default_language'),
         description=pulumi.get(__ret__, 'description'),
         distribution=pulumi.get(__ret__, 'distribution'),
+        end_of_install=pulumi.get(__ret__, 'end_of_install'),
         family=pulumi.get(__ret__, 'family'),
         filesystems=pulumi.get(__ret__, 'filesystems'),
         hard_raid_configuration=pulumi.get(__ret__, 'hard_raid_configuration'),
         id=pulumi.get(__ret__, 'id'),
+        inputs=pulumi.get(__ret__, 'inputs'),
         lvm_ready=pulumi.get(__ret__, 'lvm_ready'),
+        no_partitioning=pulumi.get(__ret__, 'no_partitioning'),
         partition_schemes=pulumi.get(__ret__, 'partition_schemes'),
+        soft_raid_only_mirroring=pulumi.get(__ret__, 'soft_raid_only_mirroring'),
+        subfamily=pulumi.get(__ret__, 'subfamily'),
         template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_installation_template)
 def get_installation_template_output(template_name: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstallationTemplateResult]:
     """
     Use this data source to get a custom installation template available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     mytemplate = ovh.Me.get_installation_template(template_name="mytemplate")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str template_name: This template name
+    :param str template_name: Template name.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_installation_templates.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_installation_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 
 def get_installation_templates(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstallationTemplatesResult:
     """
     Use this data source to get the list of custom installation templates available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     templates = ovh.Me.get_installation_templates()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getInstallationTemplates:getInstallationTemplates', __args__, opts=opts, typ=GetInstallationTemplatesResult).value
 
     return AwaitableGetInstallationTemplatesResult(
         id=pulumi.get(__ret__, 'id'),
@@ -83,17 +81,15 @@
 @_utilities.lift_output_func(get_installation_templates)
 def get_installation_templates_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstallationTemplatesResult]:
     """
     Use this data source to get the list of custom installation templates available for dedicated servers.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     templates = ovh.Me.get_installation_templates()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_me.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_me.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,22 +404,20 @@
 
 def get_me(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMeResult:
     """
     Use this data source to get information about the current OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getMe:getMe', __args__, opts=opts, typ=GetMeResult).value
 
     return AwaitableGetMeResult(
         account_urn=pulumi.get(__ret__, 'account_urn'),
@@ -458,17 +456,15 @@
 @_utilities.lift_output_func(get_me)
 def get_me_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMeResult]:
     """
     Use this data source to get information about the current OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_paymentmean_bank_account.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_paymentmean_bank_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,22 +112,20 @@
                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPaymentmeanBankAccountResult:
     """
     Use this data source to retrieve information about a bank account
     payment mean associated with an OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     ba = ovh.Me.get_paymentmean_bank_account(use_default=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description_regexp: a regexp used to filter bank accounts 
            on their `description` attributes.
     :param str state: Filter bank accounts on their `state` attribute.
            Can be "blockedForIncidents", "valid", "pendingValidation"
     :param bool use_default: Retrieve bank account marked as default payment mean.
@@ -160,22 +158,20 @@
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPaymentmeanBankAccountResult]:
     """
     Use this data source to retrieve information about a bank account
     payment mean associated with an OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     ba = ovh.Me.get_paymentmean_bank_account(use_default=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description_regexp: a regexp used to filter bank accounts 
            on their `description` attributes.
     :param str state: Filter bank accounts on their `state` attribute.
            Can be "blockedForIncidents", "valid", "pendingValidation"
     :param bool use_default: Retrieve bank account marked as default payment mean.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_paymentmean_credit_card.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/get_paymentmean_credit_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,22 +124,20 @@
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPaymentmeanCreditCardResult:
     """
     Use this data source to retrieve information about a credit card
     payment mean associated with an OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     cc = ovh.Me.get_paymentmean_credit_card(use_default=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description_regexp: a regexp used to filter credit cards 
            on their `description` attributes.
     :param Sequence[str] states: Filter credit cards on their `state` attribute.
            Can be "expired", "valid", "tooManyFailures"
     :param bool use_default: Retrieve credit card marked as default payment mean.
@@ -173,22 +171,20 @@
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPaymentmeanCreditCardResult]:
     """
     Use this data source to retrieve information about a credit card
     payment mean associated with an OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     cc = ovh.Me.get_paymentmean_credit_card(use_default=True)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description_regexp: a regexp used to filter credit cards 
            on their `description` attributes.
     :param Sequence[str] states: Filter credit cards on their `state` attribute.
            Can be "expired", "valid", "tooManyFailures"
     :param bool use_default: Retrieve credit card marked as default payment mean.
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/get_ssh_keys.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vps/get_vpss.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,94 +6,90 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetSshKeysResult',
-    'AwaitableGetSshKeysResult',
-    'get_ssh_keys',
-    'get_ssh_keys_output',
+    'GetVpssResult',
+    'AwaitableGetVpssResult',
+    'get_vpss',
+    'get_vpss_output',
 ]
 
 @pulumi.output_type
-class GetSshKeysResult:
+class GetVpssResult:
     """
-    A collection of values returned by getSshKeys.
+    A collection of values returned by getVpss.
     """
-    def __init__(__self__, id=None, names=None):
+    def __init__(__self__, id=None, results=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if names and not isinstance(names, list):
-            raise TypeError("Expected argument 'names' to be a list")
-        pulumi.set(__self__, "names", names)
+        if results and not isinstance(results, list):
+            raise TypeError("Expected argument 'results' to be a list")
+        pulumi.set(__self__, "results", results)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def names(self) -> Sequence[str]:
+    def results(self) -> Sequence[str]:
         """
-        The list of the names of all the SSH keys.
+        The list of VPS IDs associated with your OVH Account.
         """
-        return pulumi.get(self, "names")
+        return pulumi.get(self, "results")
 
 
-class AwaitableGetSshKeysResult(GetSshKeysResult):
+class AwaitableGetVpssResult(GetVpssResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetSshKeysResult(
+        return GetVpssResult(
             id=self.id,
-            names=self.names)
+            results=self.results)
 
 
-def get_ssh_keys(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSshKeysResult:
+def get_vpss(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVpssResult:
     """
-    Use this data source to retrieve list of names of the account's SSH keys.
+    Use this data source to get the list of VPS associated with your OVH Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    mykeys = ovh.Me.get_ssh_keys()
+    servers = ovh.Vps.get_vpss()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('ovh:Me/getSshKeys:getSshKeys', __args__, opts=opts, typ=GetSshKeysResult).value
+    __ret__ = pulumi.runtime.invoke('ovh:Vps/getVpss:getVpss', __args__, opts=opts, typ=GetVpssResult).value
 
-    return AwaitableGetSshKeysResult(
+    return AwaitableGetVpssResult(
         id=pulumi.get(__ret__, 'id'),
-        names=pulumi.get(__ret__, 'names'))
+        results=pulumi.get(__ret__, 'results'))
 
 
-@_utilities.lift_output_func(get_ssh_keys)
-def get_ssh_keys_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshKeysResult]:
+@_utilities.lift_output_func(get_vpss)
+def get_vpss_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVpssResult]:
     """
-    Use this data source to retrieve list of names of the account's SSH keys.
+    Use this data source to get the list of VPS associated with your OVH Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    mykeys = ovh.Me.get_ssh_keys()
+    servers = ovh.Vps.get_vpss()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/identity_group.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/identity_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,24 +197,22 @@
                  role: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an identity group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_group = ovh.me.IdentityGroup("myGroup",
             description="Some custom description",
             role="NONE")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Group description.
         :param pulumi.Input[str] name: Group name.
         :param pulumi.Input[str] role: Role associated with the group. Valid roles are ADMIN, REGULAR, UNPRIVILEGED, and NONE.
         """
@@ -225,24 +223,22 @@
                  args: Optional[IdentityGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an identity group.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_group = ovh.me.IdentityGroup("myGroup",
             description="Some custom description",
             role="NONE")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IdentityGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/identity_user.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/identity_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,27 +276,25 @@
                  password: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Creates an identity user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_user = ovh.me.IdentityUser("myUser",
             description="Some custom description",
             email="my_login@example.com",
             group="DEFAULT",
             login="my_login",
             password="super-s3cr3t!password")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: User description.
         :param pulumi.Input[str] email: User's email.
         :param pulumi.Input[str] group: User's group.
         :param pulumi.Input[str] login: User's login suffix.
@@ -309,27 +307,25 @@
                  args: IdentityUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Creates an identity user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         my_user = ovh.me.IdentityUser("myUser",
             description="Some custom description",
             email="my_login@example.com",
             group="DEFAULT",
             login="my_login",
             password="super-s3cr3t!password")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IdentityUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,32 +15,25 @@
 
 @pulumi.input_type
 class InstallationTemplateArgs:
     def __init__(__self__, *,
                  base_template_name: pulumi.Input[str],
                  template_name: pulumi.Input[str],
                  customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
                  remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a InstallationTemplate resource.
         :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         :param pulumi.Input[str] template_name: This template name.
-        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
         """
         pulumi.set(__self__, "base_template_name", base_template_name)
         pulumi.set(__self__, "template_name", template_name)
         if customization is not None:
             pulumi.set(__self__, "customization", customization)
-        if default_language is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-            pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
-        if default_language is not None:
-            pulumi.set(__self__, "default_language", default_language)
         if remove_default_partition_schemes is not None:
             pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
 
     @property
     @pulumi.getter(name="baseTemplateName")
     def base_template_name(self) -> pulumi.Input[str]:
         """
@@ -70,29 +63,14 @@
         return pulumi.get(self, "customization")
 
     @customization.setter
     def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
         pulumi.set(self, "customization", value)
 
     @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> Optional[pulumi.Input[str]]:
-        """
-        Deprecated, use language in userMetadata instead.
-        """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
-
-        return pulumi.get(self, "default_language")
-
-    @default_language.setter
-    def default_language(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_language", value)
-
-    @property
     @pulumi.getter(name="removeDefaultPartitionSchemes")
     def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
         """
         Remove default partition schemes at creation.
         """
         return pulumi.get(self, "remove_default_partition_schemes")
 
@@ -100,92 +78,88 @@
     def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "remove_default_partition_schemes", value)
 
 
 @pulumi.input_type
 class _InstallationTemplateState:
     def __init__(__self__, *,
-                 available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  base_template_name: Optional[pulumi.Input[str]] = None,
                  bit_format: Optional[pulumi.Input[int]] = None,
                  category: Optional[pulumi.Input[str]] = None,
                  customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  distribution: Optional[pulumi.Input[str]] = None,
+                 end_of_install: Optional[pulumi.Input[str]] = None,
                  family: Optional[pulumi.Input[str]] = None,
                  filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
+                 inputs: Optional[pulumi.Input[Sequence[pulumi.Input['InstallationTemplateInputArgs']]]] = None,
                  lvm_ready: Optional[pulumi.Input[bool]] = None,
+                 no_partitioning: Optional[pulumi.Input[bool]] = None,
                  remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 soft_raid_only_mirroring: Optional[pulumi.Input[bool]] = None,
+                 subfamily: Optional[pulumi.Input[str]] = None,
                  template_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering InstallationTemplate resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: Deprecated.
         :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
         :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
-        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
         :param pulumi.Input[str] description: information about this template.
         :param pulumi.Input[str] distribution: the distribution this template is based on.
-        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
-        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
-        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[str] end_of_install: after this date, install of this template will not be possible at OVH
+        :param pulumi.Input[str] family: this template family type.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available.
+        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API. Deprecated, will be removed in next release.
+        :param pulumi.Input[bool] lvm_ready: Whether this distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[bool] no_partitioning: Partitioning customization is not available for this OS template
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
+        :param pulumi.Input[bool] soft_raid_only_mirroring: Partitioning customization is available but limited to mirroring for this OS template
+        :param pulumi.Input[str] subfamily: this template subfamily type
         :param pulumi.Input[str] template_name: This template name.
         """
-        if available_languages is not None:
-            pulumi.set(__self__, "available_languages", available_languages)
         if base_template_name is not None:
             pulumi.set(__self__, "base_template_name", base_template_name)
         if bit_format is not None:
             pulumi.set(__self__, "bit_format", bit_format)
         if category is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-            pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
-        if category is not None:
             pulumi.set(__self__, "category", category)
         if customization is not None:
             pulumi.set(__self__, "customization", customization)
-        if default_language is not None:
-            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-            pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
-        if default_language is not None:
-            pulumi.set(__self__, "default_language", default_language)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if distribution is not None:
             pulumi.set(__self__, "distribution", distribution)
+        if end_of_install is not None:
+            pulumi.set(__self__, "end_of_install", end_of_install)
         if family is not None:
             pulumi.set(__self__, "family", family)
         if filesystems is not None:
             pulumi.set(__self__, "filesystems", filesystems)
         if hard_raid_configuration is not None:
+            warnings.warn("""This will be deprecated in the next release""", DeprecationWarning)
+            pulumi.log.warn("""hard_raid_configuration is deprecated: This will be deprecated in the next release""")
+        if hard_raid_configuration is not None:
             pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
+        if inputs is not None:
+            pulumi.set(__self__, "inputs", inputs)
         if lvm_ready is not None:
             pulumi.set(__self__, "lvm_ready", lvm_ready)
+        if no_partitioning is not None:
+            pulumi.set(__self__, "no_partitioning", no_partitioning)
         if remove_default_partition_schemes is not None:
             pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
+        if soft_raid_only_mirroring is not None:
+            pulumi.set(__self__, "soft_raid_only_mirroring", soft_raid_only_mirroring)
+        if subfamily is not None:
+            pulumi.set(__self__, "subfamily", subfamily)
         if template_name is not None:
             pulumi.set(__self__, "template_name", template_name)
 
     @property
-    @pulumi.getter(name="availableLanguages")
-    def available_languages(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Deprecated.
-        """
-        return pulumi.get(self, "available_languages")
-
-    @available_languages.setter
-    def available_languages(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "available_languages", value)
-
-    @property
     @pulumi.getter(name="baseTemplateName")
     def base_template_name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         """
         return pulumi.get(self, "base_template_name")
 
@@ -207,17 +181,14 @@
 
     @property
     @pulumi.getter
     def category(self) -> Optional[pulumi.Input[str]]:
         """
         Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
-
         return pulumi.get(self, "category")
 
     @category.setter
     def category(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "category", value)
 
     @property
@@ -226,29 +197,14 @@
         return pulumi.get(self, "customization")
 
     @customization.setter
     def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
         pulumi.set(self, "customization", value)
 
     @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> Optional[pulumi.Input[str]]:
-        """
-        Deprecated, use language in userMetadata instead.
-        """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
-
-        return pulumi.get(self, "default_language")
-
-    @default_language.setter
-    def default_language(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_language", value)
-
-    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         information about this template.
         """
         return pulumi.get(self, "description")
 
@@ -265,74 +221,134 @@
         return pulumi.get(self, "distribution")
 
     @distribution.setter
     def distribution(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "distribution", value)
 
     @property
+    @pulumi.getter(name="endOfInstall")
+    def end_of_install(self) -> Optional[pulumi.Input[str]]:
+        """
+        after this date, install of this template will not be possible at OVH
+        """
+        return pulumi.get(self, "end_of_install")
+
+    @end_of_install.setter
+    def end_of_install(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "end_of_install", value)
+
+    @property
     @pulumi.getter
     def family(self) -> Optional[pulumi.Input[str]]:
         """
-        this template family type (bsd,linux,solaris,windows).
+        this template family type.
         """
         return pulumi.get(self, "family")
 
     @family.setter
     def family(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "family", value)
 
     @property
     @pulumi.getter
     def filesystems(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        Filesystems available.
         """
         return pulumi.get(self, "filesystems")
 
     @filesystems.setter
     def filesystems(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "filesystems", value)
 
     @property
     @pulumi.getter(name="hardRaidConfiguration")
     def hard_raid_configuration(self) -> Optional[pulumi.Input[bool]]:
         """
-        This distribution supports hardware raid configuration through the OVHcloud API.
+        This distribution supports hardware raid configuration through the OVHcloud API. Deprecated, will be removed in next release.
         """
+        warnings.warn("""This will be deprecated in the next release""", DeprecationWarning)
+        pulumi.log.warn("""hard_raid_configuration is deprecated: This will be deprecated in the next release""")
+
         return pulumi.get(self, "hard_raid_configuration")
 
     @hard_raid_configuration.setter
     def hard_raid_configuration(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "hard_raid_configuration", value)
 
     @property
+    @pulumi.getter
+    def inputs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['InstallationTemplateInputArgs']]]]:
+        return pulumi.get(self, "inputs")
+
+    @inputs.setter
+    def inputs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['InstallationTemplateInputArgs']]]]):
+        pulumi.set(self, "inputs", value)
+
+    @property
     @pulumi.getter(name="lvmReady")
     def lvm_ready(self) -> Optional[pulumi.Input[bool]]:
         """
-        This distribution supports Logical Volumes (Linux LVM)
+        Whether this distribution supports Logical Volumes (Linux LVM)
         """
         return pulumi.get(self, "lvm_ready")
 
     @lvm_ready.setter
     def lvm_ready(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lvm_ready", value)
 
     @property
+    @pulumi.getter(name="noPartitioning")
+    def no_partitioning(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Partitioning customization is not available for this OS template
+        """
+        return pulumi.get(self, "no_partitioning")
+
+    @no_partitioning.setter
+    def no_partitioning(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_partitioning", value)
+
+    @property
     @pulumi.getter(name="removeDefaultPartitionSchemes")
     def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
         """
         Remove default partition schemes at creation.
         """
         return pulumi.get(self, "remove_default_partition_schemes")
 
     @remove_default_partition_schemes.setter
     def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "remove_default_partition_schemes", value)
 
     @property
+    @pulumi.getter(name="softRaidOnlyMirroring")
+    def soft_raid_only_mirroring(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Partitioning customization is available but limited to mirroring for this OS template
+        """
+        return pulumi.get(self, "soft_raid_only_mirroring")
+
+    @soft_raid_only_mirroring.setter
+    def soft_raid_only_mirroring(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "soft_raid_only_mirroring", value)
+
+    @property
+    @pulumi.getter
+    def subfamily(self) -> Optional[pulumi.Input[str]]:
+        """
+        this template subfamily type
+        """
+        return pulumi.get(self, "subfamily")
+
+    @subfamily.setter
+    def subfamily(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subfamily", value)
+
+    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> Optional[pulumi.Input[str]]:
         """
         This template name.
         """
         return pulumi.get(self, "template_name")
 
@@ -344,15 +360,14 @@
 class InstallationTemplate(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  base_template_name: Optional[pulumi.Input[str]] = None,
                  customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
                  remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to create a custom installation template available for dedicated servers.
 
         ## Import
@@ -364,15 +379,14 @@
         ```sh
         $ pulumi import ovh:Me/installationTemplate:InstallationTemplate mytemplate base_template_name/template_name
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
         :param pulumi.Input[str] template_name: This template name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -404,15 +418,14 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  base_template_name: Optional[pulumi.Input[str]] = None,
                  customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
                  remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -420,102 +433,105 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstallationTemplateArgs.__new__(InstallationTemplateArgs)
 
             if base_template_name is None and not opts.urn:
                 raise TypeError("Missing required property 'base_template_name'")
             __props__.__dict__["base_template_name"] = base_template_name
             __props__.__dict__["customization"] = customization
-            __props__.__dict__["default_language"] = default_language
             __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
             if template_name is None and not opts.urn:
                 raise TypeError("Missing required property 'template_name'")
             __props__.__dict__["template_name"] = template_name
-            __props__.__dict__["available_languages"] = None
             __props__.__dict__["bit_format"] = None
             __props__.__dict__["category"] = None
             __props__.__dict__["description"] = None
             __props__.__dict__["distribution"] = None
+            __props__.__dict__["end_of_install"] = None
             __props__.__dict__["family"] = None
             __props__.__dict__["filesystems"] = None
             __props__.__dict__["hard_raid_configuration"] = None
+            __props__.__dict__["inputs"] = None
             __props__.__dict__["lvm_ready"] = None
+            __props__.__dict__["no_partitioning"] = None
+            __props__.__dict__["soft_raid_only_mirroring"] = None
+            __props__.__dict__["subfamily"] = None
         super(InstallationTemplate, __self__).__init__(
             'ovh:Me/installationTemplate:InstallationTemplate',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             base_template_name: Optional[pulumi.Input[str]] = None,
             bit_format: Optional[pulumi.Input[int]] = None,
             category: Optional[pulumi.Input[str]] = None,
             customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-            default_language: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             distribution: Optional[pulumi.Input[str]] = None,
+            end_of_install: Optional[pulumi.Input[str]] = None,
             family: Optional[pulumi.Input[str]] = None,
             filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
+            inputs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InstallationTemplateInputArgs']]]]] = None,
             lvm_ready: Optional[pulumi.Input[bool]] = None,
+            no_partitioning: Optional[pulumi.Input[bool]] = None,
             remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+            soft_raid_only_mirroring: Optional[pulumi.Input[bool]] = None,
+            subfamily: Optional[pulumi.Input[str]] = None,
             template_name: Optional[pulumi.Input[str]] = None) -> 'InstallationTemplate':
         """
         Get an existing InstallationTemplate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: Deprecated.
         :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
         :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
-        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
         :param pulumi.Input[str] description: information about this template.
         :param pulumi.Input[str] distribution: the distribution this template is based on.
-        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
-        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
-        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[str] end_of_install: after this date, install of this template will not be possible at OVH
+        :param pulumi.Input[str] family: this template family type.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available.
+        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API. Deprecated, will be removed in next release.
+        :param pulumi.Input[bool] lvm_ready: Whether this distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[bool] no_partitioning: Partitioning customization is not available for this OS template
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
+        :param pulumi.Input[bool] soft_raid_only_mirroring: Partitioning customization is available but limited to mirroring for this OS template
+        :param pulumi.Input[str] subfamily: this template subfamily type
         :param pulumi.Input[str] template_name: This template name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstallationTemplateState.__new__(_InstallationTemplateState)
 
-        __props__.__dict__["available_languages"] = available_languages
         __props__.__dict__["base_template_name"] = base_template_name
         __props__.__dict__["bit_format"] = bit_format
         __props__.__dict__["category"] = category
         __props__.__dict__["customization"] = customization
-        __props__.__dict__["default_language"] = default_language
         __props__.__dict__["description"] = description
         __props__.__dict__["distribution"] = distribution
+        __props__.__dict__["end_of_install"] = end_of_install
         __props__.__dict__["family"] = family
         __props__.__dict__["filesystems"] = filesystems
         __props__.__dict__["hard_raid_configuration"] = hard_raid_configuration
+        __props__.__dict__["inputs"] = inputs
         __props__.__dict__["lvm_ready"] = lvm_ready
+        __props__.__dict__["no_partitioning"] = no_partitioning
         __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
+        __props__.__dict__["soft_raid_only_mirroring"] = soft_raid_only_mirroring
+        __props__.__dict__["subfamily"] = subfamily
         __props__.__dict__["template_name"] = template_name
         return InstallationTemplate(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="availableLanguages")
-    def available_languages(self) -> pulumi.Output[Sequence[str]]:
-        """
-        Deprecated.
-        """
-        return pulumi.get(self, "available_languages")
-
-    @property
     @pulumi.getter(name="baseTemplateName")
     def base_template_name(self) -> pulumi.Output[str]:
         """
         The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         """
         return pulumi.get(self, "base_template_name")
 
@@ -529,36 +545,22 @@
 
     @property
     @pulumi.getter
     def category(self) -> pulumi.Output[str]:
         """
         Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
-
         return pulumi.get(self, "category")
 
     @property
     @pulumi.getter
     def customization(self) -> pulumi.Output[Optional['outputs.InstallationTemplateCustomization']]:
         return pulumi.get(self, "customization")
 
     @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> pulumi.Output[Optional[str]]:
-        """
-        Deprecated, use language in userMetadata instead.
-        """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
-
-        return pulumi.get(self, "default_language")
-
-    @property
     @pulumi.getter
     def description(self) -> pulumi.Output[str]:
         """
         information about this template.
         """
         return pulumi.get(self, "description")
 
@@ -567,54 +569,94 @@
     def distribution(self) -> pulumi.Output[str]:
         """
         the distribution this template is based on.
         """
         return pulumi.get(self, "distribution")
 
     @property
+    @pulumi.getter(name="endOfInstall")
+    def end_of_install(self) -> pulumi.Output[str]:
+        """
+        after this date, install of this template will not be possible at OVH
+        """
+        return pulumi.get(self, "end_of_install")
+
+    @property
     @pulumi.getter
     def family(self) -> pulumi.Output[str]:
         """
-        this template family type (bsd,linux,solaris,windows).
+        this template family type.
         """
         return pulumi.get(self, "family")
 
     @property
     @pulumi.getter
     def filesystems(self) -> pulumi.Output[Sequence[str]]:
         """
-        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        Filesystems available.
         """
         return pulumi.get(self, "filesystems")
 
     @property
     @pulumi.getter(name="hardRaidConfiguration")
     def hard_raid_configuration(self) -> pulumi.Output[bool]:
         """
-        This distribution supports hardware raid configuration through the OVHcloud API.
+        This distribution supports hardware raid configuration through the OVHcloud API. Deprecated, will be removed in next release.
         """
+        warnings.warn("""This will be deprecated in the next release""", DeprecationWarning)
+        pulumi.log.warn("""hard_raid_configuration is deprecated: This will be deprecated in the next release""")
+
         return pulumi.get(self, "hard_raid_configuration")
 
     @property
+    @pulumi.getter
+    def inputs(self) -> pulumi.Output[Sequence['outputs.InstallationTemplateInput']]:
+        return pulumi.get(self, "inputs")
+
+    @property
     @pulumi.getter(name="lvmReady")
     def lvm_ready(self) -> pulumi.Output[bool]:
         """
-        This distribution supports Logical Volumes (Linux LVM)
+        Whether this distribution supports Logical Volumes (Linux LVM)
         """
         return pulumi.get(self, "lvm_ready")
 
     @property
+    @pulumi.getter(name="noPartitioning")
+    def no_partitioning(self) -> pulumi.Output[bool]:
+        """
+        Partitioning customization is not available for this OS template
+        """
+        return pulumi.get(self, "no_partitioning")
+
+    @property
     @pulumi.getter(name="removeDefaultPartitionSchemes")
     def remove_default_partition_schemes(self) -> pulumi.Output[bool]:
         """
         Remove default partition schemes at creation.
         """
         return pulumi.get(self, "remove_default_partition_schemes")
 
     @property
+    @pulumi.getter(name="softRaidOnlyMirroring")
+    def soft_raid_only_mirroring(self) -> pulumi.Output[bool]:
+        """
+        Partitioning customization is available but limited to mirroring for this OS template
+        """
+        return pulumi.get(self, "soft_raid_only_mirroring")
+
+    @property
+    @pulumi.getter
+    def subfamily(self) -> pulumi.Output[str]:
+        """
+        this template subfamily type
+        """
+        return pulumi.get(self, "subfamily")
+
+    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> pulumi.Output[str]:
         """
         This template name.
         """
         return pulumi.get(self, "template_name")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,27 +131,25 @@
                  template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to create partition scheme for a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `name` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -172,27 +170,25 @@
                  args: InstallationTemplatePartitionSchemeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to create partition scheme for a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `name` of the cluster, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,14 @@
                  template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to create a hardware raid group in the partition scheme of a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
@@ -248,15 +247,14 @@
             disks=[
                 "[c1:d1,c1:d2,c1:d3]",
                 "[c1:d10,c1:d20,c1:d30]",
             ],
             mode="raid50",
             step=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `scheme_name`, `name` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -280,15 +278,14 @@
                  args: InstallationTemplatePartitionSchemeHardwareRaidArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to create a hardware raid group in the partition scheme of a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
@@ -301,15 +298,14 @@
             disks=[
                 "[c1:d1,c1:d2,c1:d3]",
                 "[c1:d10,c1:d20,c1:d30]",
             ],
             mode="raid50",
             step=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `scheme_name`, `name` of the cluster, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/installation_template_partition_scheme_partition.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,14 @@
                  volume_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to create a partition in the partition scheme of a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
@@ -412,15 +411,14 @@
             scheme_name=scheme.name,
             mountpoint="/",
             filesystem="ext4",
             size=400,
             order=1,
             type="primary")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `scheme_name`, `mountpoint` of the cluster, separated by "/" E.g.,
 
         bash
 
@@ -464,15 +462,14 @@
                  args: InstallationTemplatePartitionSchemePartitionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to create a partition in the partition scheme of a custom installation template available for dedicated servers.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
             base_template_name="debian12_64",
             template_name="mytemplate")
@@ -484,15 +481,14 @@
             scheme_name=scheme.name,
             mountpoint="/",
             filesystem="ext4",
             size=400,
             order=1,
             type="primary")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         The resource can be imported using the `template_name`, `scheme_name`, `mountpoint` of the cluster, separated by "/" E.g.,
 
         bash
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/me/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/me/outputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
     'InstallationTemplateCustomization',
+    'InstallationTemplateInput',
     'GetInstallationTemplateCustomizationResult',
+    'GetInstallationTemplateInputResult',
     'GetInstallationTemplatePartitionSchemeResult',
     'GetInstallationTemplatePartitionSchemeHardwareRaidResult',
     'GetInstallationTemplatePartitionSchemePartitionResult',
     'GetMeCurrencyResult',
 ]
 
 @pulumi.output_type
@@ -26,16 +28,14 @@
         suggest = None
         if key == "customHostname":
             suggest = "custom_hostname"
         elif key == "postInstallationScriptLink":
             suggest = "post_installation_script_link"
         elif key == "postInstallationScriptReturn":
             suggest = "post_installation_script_return"
-        elif key == "sshKeyName":
-            suggest = "ssh_key_name"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstallationTemplateCustomization. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstallationTemplateCustomization.__key_warning(key)
         return super().__getitem__(key)
@@ -43,30 +43,26 @@
     def get(self, key: str, default = None) -> Any:
         InstallationTemplateCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  custom_hostname: Optional[str] = None,
                  post_installation_script_link: Optional[str] = None,
-                 post_installation_script_return: Optional[str] = None,
-                 ssh_key_name: Optional[str] = None):
+                 post_installation_script_return: Optional[str] = None):
         """
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param str ssh_key_name: Deprecated.
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if ssh_key_name is not None:
-            pulumi.set(__self__, "ssh_key_name", ssh_key_name)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[str]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -84,43 +80,88 @@
     @pulumi.getter(name="postInstallationScriptReturn")
     def post_installation_script_return(self) -> Optional[str]:
         """
         indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
         return pulumi.get(self, "post_installation_script_return")
 
+
+@pulumi.output_type
+class InstallationTemplateInput(dict):
+    def __init__(__self__, *,
+                 default: Optional[str] = None,
+                 description: Optional[str] = None,
+                 enums: Optional[Sequence[str]] = None,
+                 mandatory: Optional[bool] = None,
+                 name: Optional[str] = None,
+                 type: Optional[str] = None):
+        """
+        :param str description: information about this template.
+        """
+        if default is not None:
+            pulumi.set(__self__, "default", default)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if enums is not None:
+            pulumi.set(__self__, "enums", enums)
+        if mandatory is not None:
+            pulumi.set(__self__, "mandatory", mandatory)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
     @property
-    @pulumi.getter(name="sshKeyName")
-    def ssh_key_name(self) -> Optional[str]:
+    @pulumi.getter
+    def default(self) -> Optional[str]:
+        return pulumi.get(self, "default")
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[str]:
         """
-        Deprecated.
+        information about this template.
         """
-        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
-        pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def enums(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "enums")
+
+    @property
+    @pulumi.getter
+    def mandatory(self) -> Optional[bool]:
+        return pulumi.get(self, "mandatory")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        return pulumi.get(self, "name")
 
-        return pulumi.get(self, "ssh_key_name")
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[str]:
+        return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class GetInstallationTemplateCustomizationResult(dict):
     def __init__(__self__, *,
                  custom_hostname: str,
                  post_installation_script_link: str,
-                 post_installation_script_return: str,
-                 ssh_key_name: str):
+                 post_installation_script_return: str):
         """
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
-        :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled. Deprecated, will be removed in next release, use userMetada instead.
+        :param str post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
         pulumi.set(__self__, "custom_hostname", custom_hostname)
         pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        pulumi.set(__self__, "ssh_key_name", ssh_key_name)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> str:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -134,40 +175,90 @@
         """
         return pulumi.get(self, "post_installation_script_link")
 
     @property
     @pulumi.getter(name="postInstallationScriptReturn")
     def post_installation_script_return(self) -> str:
         """
-        indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
+        Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
         return pulumi.get(self, "post_installation_script_return")
 
+
+@pulumi.output_type
+class GetInstallationTemplateInputResult(dict):
+    def __init__(__self__, *,
+                 default: str,
+                 description: str,
+                 enums: Sequence[str],
+                 mandatory: bool,
+                 name: str,
+                 type: str):
+        """
+        :param str description: Information about this template.
+        :param str name: Hardware RAID name.
+        :param str type: Partition type.
+        """
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "enums", enums)
+        pulumi.set(__self__, "mandatory", mandatory)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def default(self) -> str:
+        return pulumi.get(self, "default")
+
     @property
-    @pulumi.getter(name="sshKeyName")
-    def ssh_key_name(self) -> str:
+    @pulumi.getter
+    def description(self) -> str:
         """
-        Name of the ssh key that should be installed. Password login will be disabled. Deprecated, will be removed in next release, use userMetada instead.
+        Information about this template.
         """
-        warnings.warn("""This field will be removed from the API, please use `userMetadata` instead.""", DeprecationWarning)
-        pulumi.log.warn("""ssh_key_name is deprecated: This field will be removed from the API, please use `userMetadata` instead.""")
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def enums(self) -> Sequence[str]:
+        return pulumi.get(self, "enums")
+
+    @property
+    @pulumi.getter
+    def mandatory(self) -> bool:
+        return pulumi.get(self, "mandatory")
 
-        return pulumi.get(self, "ssh_key_name")
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Hardware RAID name.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Partition type.
+        """
+        return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class GetInstallationTemplatePartitionSchemeResult(dict):
     def __init__(__self__, *,
                  hardware_raids: Sequence['outputs.GetInstallationTemplatePartitionSchemeHardwareRaidResult'],
                  name: str,
                  partitions: Sequence['outputs.GetInstallationTemplatePartitionSchemePartitionResult'],
                  priority: int):
         """
         :param str name: Hardware RAID name.
-        :param int priority: on a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
+        :param int priority: On a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
         """
         pulumi.set(__self__, "hardware_raids", hardware_raids)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "partitions", partitions)
         pulumi.set(__self__, "priority", priority)
 
     @property
@@ -188,15 +279,15 @@
     def partitions(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemePartitionResult']:
         return pulumi.get(self, "partitions")
 
     @property
     @pulumi.getter
     def priority(self) -> int:
         """
-        on a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
+        On a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
         """
         return pulumi.get(self, "priority")
 
 
 @pulumi.output_type
 class GetInstallationTemplatePartitionSchemeHardwareRaidResult(dict):
     def __init__(__self__, *,
@@ -256,20 +347,20 @@
                  order: int,
                  raid: str,
                  size: int,
                  type: str,
                  volume_name: str):
         """
         :param str filesystem: Partition filesystem.
-        :param str mountpoint: partition mount point.
-        :param int order: step or order. specifies the creation order of the partition on the disk
-        :param str raid: raid partition type.
-        :param int size: size of partition in MB, 0 => rest of the space.
-        :param str type: partition type.
-        :param str volume_name: The volume name needed for proxmox distribution
+        :param str mountpoint: Partition mount point.
+        :param int order: Step or order. Specifies the creation order of the partition on the disk.
+        :param str raid: Raid partition type.
+        :param int size: Size of partition in MB, 0 => rest of the space.
+        :param str type: Partition type.
+        :param str volume_name: Volume name needed for proxmox distribution.
         """
         pulumi.set(__self__, "filesystem", filesystem)
         pulumi.set(__self__, "mountpoint", mountpoint)
         pulumi.set(__self__, "order", order)
         pulumi.set(__self__, "raid", raid)
         pulumi.set(__self__, "size", size)
         pulumi.set(__self__, "type", type)
@@ -283,55 +374,55 @@
         """
         return pulumi.get(self, "filesystem")
 
     @property
     @pulumi.getter
     def mountpoint(self) -> str:
         """
-        partition mount point.
+        Partition mount point.
         """
         return pulumi.get(self, "mountpoint")
 
     @property
     @pulumi.getter
     def order(self) -> int:
         """
-        step or order. specifies the creation order of the partition on the disk
+        Step or order. Specifies the creation order of the partition on the disk.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def raid(self) -> str:
         """
-        raid partition type.
+        Raid partition type.
         """
         return pulumi.get(self, "raid")
 
     @property
     @pulumi.getter
     def size(self) -> int:
         """
-        size of partition in MB, 0 => rest of the space.
+        Size of partition in MB, 0 => rest of the space.
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        partition type.
+        Partition type.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="volumeName")
     def volume_name(self) -> str:
         """
-        The volume name needed for proxmox distribution
+        Volume name needed for proxmox distribution.
         """
         return pulumi.get(self, "volume_name")
 
 
 @pulumi.output_type
 class GetMeCurrencyResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,23 +122,21 @@
              ovh_subsidiary: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCartResult:
     """
     Use this data source to create a temporary order cart to retrieve information order cart products.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool assign: Assign a shopping cart to a logged in client. Values can be `true` or `false`.
     :param str description: Description of your cart
     :param str expire: Expiration time (format: 2006-01-02T15:04:05+00:00)
     :param str ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
     """
@@ -168,23 +166,21 @@
                     ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCartResult]:
     """
     Use this data source to create a temporary order cart to retrieve information order cart products.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param bool assign: Assign a shopping cart to a logged in client. Values can be `true` or `false`.
     :param str description: Description of your cart
     :param str expire: Expiration time (format: 2006-01-02T15:04:05+00:00)
     :param str ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,25 +79,23 @@
                      product: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCartProductResult:
     """
     Use this data source to retrieve information of order cart product products.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plans = ovh.Order.get_cart_product(cart_id=mycart.id,
         product="...")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str product: product
     """
     __args__ = dict()
     __args__['cartId'] = cart_id
@@ -117,24 +115,22 @@
                             product: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCartProductResult]:
     """
     Use this data source to retrieve information of order cart product products.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plans = ovh.Order.get_cart_product(cart_id=mycart.id,
         product="...")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str product: product
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_options.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,26 +102,24 @@
                              product: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCartProductOptionsResult:
     """
     Use this data source to retrieve information of order cart product options.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     options = ovh.Order.get_cart_product_options(cart_id=mycart.id,
         product="cloud",
         plan_code="project")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str plan_code: Product offer identifier
     :param str product: Product
     """
@@ -149,26 +147,24 @@
                                     product: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCartProductOptionsResult]:
     """
     Use this data source to retrieve information of order cart product options.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     options = ovh.Order.get_cart_product_options(cart_id=mycart.id,
         product="cloud",
         plan_code="project")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str plan_code: Product offer identifier
     :param str product: Product
     """
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_options_plan.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_options_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,28 +194,26 @@
                                   product: Optional[str] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCartProductOptionsPlanResult:
     """
     Use this data source to retrieve information of order cart product options plan.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plan = ovh.Order.get_cart_product_options_plan(cart_id=mycart.id,
         price_capacity="renew",
         product="cloud",
         plan_code="project",
         options_plan_code="vrack")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str options_plan_code: options plan code.
     :param str plan_code: Product offer identifier
     :param str price_capacity: Capacity of the pricing (type of pricing)
@@ -257,28 +255,26 @@
                                          product: Optional[pulumi.Input[str]] = None,
                                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCartProductOptionsPlanResult]:
     """
     Use this data source to retrieve information of order cart product options plan.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plan = ovh.Order.get_cart_product_options_plan(cart_id=mycart.id,
         price_capacity="renew",
         product="cloud",
         plan_code="project",
         options_plan_code="vrack")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str options_plan_code: options plan code.
     :param str plan_code: Product offer identifier
     :param str price_capacity: Capacity of the pricing (type of pricing)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/get_cart_product_plan.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/get_cart_product_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,27 +148,25 @@
                           product: Optional[str] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCartProductPlanResult:
     """
     Use this data source to retrieve information of order cart product plan.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
         price_capacity="renew",
         product="cloud",
         plan_code="project")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str plan_code: Product offer identifier
     :param str price_capacity: Capacity of the pricing (type of pricing)
     :param str product: Product
@@ -203,27 +201,25 @@
                                  product: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCartProductPlanResult]:
     """
     Use this data source to retrieve information of order cart product plan.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     myaccount = ovh.Me.get_me()
     mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
     plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
         price_capacity="renew",
         product="cloud",
         plan_code="project")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str cart_id: Cart identifier
     :param str catalog_name: Catalog name
     :param str plan_code: Product offer identifier
     :param str price_capacity: Capacity of the pricing (type of pricing)
     :param str product: Product
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/order/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/order/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/provider.py` & `pulumi_ovh-0.44.0/pulumi_ovh/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vps/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vps/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -468,37 +468,37 @@
 
 @pulumi.input_type
 class VpsPlanConfigurationArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] label: Identifier of the resource
-        :param pulumi.Input[str] value: Path to the resource in api.ovh.com
+        :param pulumi.Input[str] label: Label for your configuration item
+        :param pulumi.Input[str] value: Value or resource URL on API.OVH.COM of your configuration item
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
         """
-        Identifier of the resource
+        Label for your configuration item
         """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
-        Path to the resource in api.ovh.com
+        Value or resource URL on API.OVH.COM of your configuration item
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
@@ -603,37 +603,37 @@
 
 @pulumi.input_type
 class VpsPlanOptionConfigurationArgs:
     def __init__(__self__, *,
                  label: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] label: Identifier of the resource
-        :param pulumi.Input[str] value: Path to the resource in api.ovh.com
+        :param pulumi.Input[str] label: Label for your configuration item
+        :param pulumi.Input[str] value: Value or resource URL on API.OVH.COM of your configuration item
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
         """
-        Identifier of the resource
+        Label for your configuration item
         """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
         """
-        Path to the resource in api.ovh.com
+        Value or resource URL on API.OVH.COM of your configuration item
         """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vps/get_vps.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vps/get_vps.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,22 +245,20 @@
 def get_vps(service_name: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVpsResult:
     """
     Use this data source to retrieve information about a vps associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     server = ovh.Vps.get_vps(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated server.
     """
     __args__ = dict()
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -291,20 +289,18 @@
 def get_vps_output(service_name: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVpsResult]:
     """
     Use this data source to retrieve information about a vps associated with your OVHcloud Account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
     server = ovh.Vps.get_vps(service_name="XXXXXX")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str service_name: The service_name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vps/get_vpss.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/get_vracks.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetVpssResult',
-    'AwaitableGetVpssResult',
-    'get_vpss',
-    'get_vpss_output',
+    'GetVracksResult',
+    'AwaitableGetVracksResult',
+    'get_vracks',
+    'get_vracks_output',
 ]
 
 @pulumi.output_type
-class GetVpssResult:
+class GetVracksResult:
     """
-    A collection of values returned by getVpss.
+    A collection of values returned by getVracks.
     """
     def __init__(__self__, id=None, results=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if results and not isinstance(results, list):
             raise TypeError("Expected argument 'results' to be a list")
@@ -37,63 +37,59 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence[str]:
         """
-        The list of VPS IDs associated with your OVH Account.
+        The list of vrack service name available for your OVHcloud account.
         """
         return pulumi.get(self, "results")
 
 
-class AwaitableGetVpssResult(GetVpssResult):
+class AwaitableGetVracksResult(GetVracksResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetVpssResult(
+        return GetVracksResult(
             id=self.id,
             results=self.results)
 
 
-def get_vpss(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVpssResult:
+def get_vracks(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVracksResult:
     """
-    Use this data source to get the list of VPS associated with your OVH Account.
+    Use this data source to get the list of Vrack IDs available for your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    servers = ovh.Vps.get_vpss()
+    vracks = ovh.Vrack.get_vracks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('ovh:Vps/getVpss:getVpss', __args__, opts=opts, typ=GetVpssResult).value
+    __ret__ = pulumi.runtime.invoke('ovh:Vrack/getVracks:getVracks', __args__, opts=opts, typ=GetVracksResult).value
 
-    return AwaitableGetVpssResult(
+    return AwaitableGetVracksResult(
         id=pulumi.get(__ret__, 'id'),
         results=pulumi.get(__ret__, 'results'))
 
 
-@_utilities.lift_output_func(get_vpss)
-def get_vpss_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVpssResult]:
+@_utilities.lift_output_func(get_vracks)
+def get_vracks_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVracksResult]:
     """
-    Use this data source to get the list of VPS associated with your OVH Account.
+    Use this data source to get the list of Vrack IDs available for your OVHcloud account.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    servers = ovh.Vps.get_vpss()
+    vracks = ovh.Vrack.get_vracks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vps/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vps/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,33 +452,33 @@
 
 @pulumi.output_type
 class VpsPlanConfiguration(dict):
     def __init__(__self__, *,
                  label: str,
                  value: str):
         """
-        :param str label: Identifier of the resource
-        :param str value: Path to the resource in api.ovh.com
+        :param str label: Label for your configuration item
+        :param str value: Value or resource URL on API.OVH.COM of your configuration item
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> str:
         """
-        Identifier of the resource
+        Label for your configuration item
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
-        Path to the resource in api.ovh.com
+        Value or resource URL on API.OVH.COM of your configuration item
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class VpsPlanOption(dict):
     @staticmethod
@@ -576,30 +576,30 @@
 
 @pulumi.output_type
 class VpsPlanOptionConfiguration(dict):
     def __init__(__self__, *,
                  label: str,
                  value: str):
         """
-        :param str label: Identifier of the resource
-        :param str value: Path to the resource in api.ovh.com
+        :param str label: Label for your configuration item
+        :param str value: Value or resource URL on API.OVH.COM of your configuration item
         """
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def label(self) -> str:
         """
-        Identifier of the resource
+        Label for your configuration item
         """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def value(self) -> str:
         """
-        Path to the resource in api.ovh.com
+        Value or resource URL on API.OVH.COM of your configuration item
         """
         return pulumi.get(self, "value")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vps/vps.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vps/vps.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/__init__.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/_inputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/cloud_project.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/cloud_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,33 +106,31 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Attach a Public Cloud Project to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         vcp = ovh.vrack.CloudProject("vcp",
             project_id="67890",
             service_name="12345")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Attachment of a public cloud project and a VRack can be imported using the `project_id`, the `service_name` (vRackID) and the `attach_id`, separated by "/" E.g.,
+        Attachment of a public cloud project and a VRack can be imported using the `service_name` (vRack identifier) and the `project_id` (Cloud Project identifier), separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/vrack_pn-12345678-cloudproject_ookie9mee8Shaeghaeleeju7Xeghohv6e-attach
+        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach service_name/project_id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] project_id: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
@@ -145,33 +143,31 @@
                  args: CloudProjectArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Attach a Public Cloud Project to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         vcp = ovh.vrack.CloudProject("vcp",
             project_id="67890",
             service_name="12345")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Attachment of a public cloud project and a VRack can be imported using the `project_id`, the `service_name` (vRackID) and the `attach_id`, separated by "/" E.g.,
+        Attachment of a public cloud project and a VRack can be imported using the `service_name` (vRack identifier) and the `project_id` (Cloud Project identifier), separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/vrack_pn-12345678-cloudproject_ookie9mee8Shaeghaeleeju7Xeghohv6e-attach
+        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach service_name/project_id
         ```
 
         :param str resource_name: The name of the resource.
         :param CloudProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/dedicated_server.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/dedicated_server_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,229 +5,227 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['DedicatedServerArgs', 'DedicatedServer']
+__all__ = ['DedicatedServerInterfaceArgs', 'DedicatedServerInterface']
 
 @pulumi.input_type
-class DedicatedServerArgs:
+class DedicatedServerInterfaceArgs:
     def __init__(__self__, *,
-                 server_id: pulumi.Input[str],
+                 interface_id: pulumi.Input[str],
                  service_name: pulumi.Input[str]):
         """
-        The set of arguments for constructing a DedicatedServer resource.
-        :param pulumi.Input[str] server_id: The id of the dedicated server.
-        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+        The set of arguments for constructing a DedicatedServerInterface resource.
+        :param pulumi.Input[str] interface_id: The id of dedicated server network interface.
+        :param pulumi.Input[str] service_name: The id of the vrack. If omitted,
                the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        pulumi.set(__self__, "server_id", server_id)
+        pulumi.set(__self__, "interface_id", interface_id)
         pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter(name="serverId")
-    def server_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="interfaceId")
+    def interface_id(self) -> pulumi.Input[str]:
         """
-        The id of the dedicated server.
+        The id of dedicated server network interface.
         """
-        return pulumi.get(self, "server_id")
+        return pulumi.get(self, "interface_id")
 
-    @server_id.setter
-    def server_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "server_id", value)
+    @interface_id.setter
+    def interface_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "interface_id", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The service name of the vrack. If omitted,
+        The id of the vrack. If omitted,
         the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
 
 @pulumi.input_type
-class _DedicatedServerState:
+class _DedicatedServerInterfaceState:
     def __init__(__self__, *,
-                 server_id: Optional[pulumi.Input[str]] = None,
+                 interface_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering DedicatedServer resources.
-        :param pulumi.Input[str] server_id: The id of the dedicated server.
-        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+        Input properties used for looking up and filtering DedicatedServerInterface resources.
+        :param pulumi.Input[str] interface_id: The id of dedicated server network interface.
+        :param pulumi.Input[str] service_name: The id of the vrack. If omitted,
                the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        if server_id is not None:
-            pulumi.set(__self__, "server_id", server_id)
+        if interface_id is not None:
+            pulumi.set(__self__, "interface_id", interface_id)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter(name="serverId")
-    def server_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="interfaceId")
+    def interface_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the dedicated server.
+        The id of dedicated server network interface.
         """
-        return pulumi.get(self, "server_id")
+        return pulumi.get(self, "interface_id")
 
-    @server_id.setter
-    def server_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "server_id", value)
+    @interface_id.setter
+    def interface_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "interface_id", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The service name of the vrack. If omitted,
+        The id of the vrack. If omitted,
         the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
 
-class DedicatedServer(pulumi.CustomResource):
+class DedicatedServerInterface(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 server_id: Optional[pulumi.Input[str]] = None,
+                 interface_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Attach a legacy dedicated server to a vRack.
+        Attach a Dedicated Server Network Interface to a vRack.
 
-        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
-        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
+        > **NOTE:** The resource `Vrack.DedicatedServerInterface` is intended to be used for dedicated servers that have configurable network interfaces.<br />
+        Legacy Dedicated servers that do not have configurable network interfaces MUST use the resource `Vrack.DedicatedServer` instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        vds = ovh.vrack.DedicatedServer("vds",
-            server_id="67890",
-            service_name="XXXX")
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        vdsi = ovh.vrack.DedicatedServerInterface("vdsi",
+            service_name="pn-xxxxxxx",
+            interface_id=server.enabled_vrack_vnis[0])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] server_id: The id of the dedicated server.
-        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+        :param pulumi.Input[str] interface_id: The id of dedicated server network interface.
+        :param pulumi.Input[str] service_name: The id of the vrack. If omitted,
                the `OVH_VRACK_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DedicatedServerArgs,
+                 args: DedicatedServerInterfaceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Attach a legacy dedicated server to a vRack.
+        Attach a Dedicated Server Network Interface to a vRack.
 
-        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
-        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
+        > **NOTE:** The resource `Vrack.DedicatedServerInterface` is intended to be used for dedicated servers that have configurable network interfaces.<br />
+        Legacy Dedicated servers that do not have configurable network interfaces MUST use the resource `Vrack.DedicatedServer` instead.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        vds = ovh.vrack.DedicatedServer("vds",
-            server_id="67890",
-            service_name="XXXX")
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        vdsi = ovh.vrack.DedicatedServerInterface("vdsi",
+            service_name="pn-xxxxxxx",
+            interface_id=server.enabled_vrack_vnis[0])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
-        :param DedicatedServerArgs args: The arguments to use to populate this resource's properties.
+        :param DedicatedServerInterfaceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DedicatedServerArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DedicatedServerInterfaceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 server_id: Optional[pulumi.Input[str]] = None,
+                 interface_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DedicatedServerArgs.__new__(DedicatedServerArgs)
+            __props__ = DedicatedServerInterfaceArgs.__new__(DedicatedServerInterfaceArgs)
 
-            if server_id is None and not opts.urn:
-                raise TypeError("Missing required property 'server_id'")
-            __props__.__dict__["server_id"] = server_id
+            if interface_id is None and not opts.urn:
+                raise TypeError("Missing required property 'interface_id'")
+            __props__.__dict__["interface_id"] = interface_id
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
-        super(DedicatedServer, __self__).__init__(
-            'ovh:Vrack/dedicatedServer:DedicatedServer',
+        super(DedicatedServerInterface, __self__).__init__(
+            'ovh:Vrack/dedicatedServerInterface:DedicatedServerInterface',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            server_id: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None) -> 'DedicatedServer':
+            interface_id: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'DedicatedServerInterface':
         """
-        Get an existing DedicatedServer resource's state with the given name, id, and optional extra
+        Get an existing DedicatedServerInterface resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] server_id: The id of the dedicated server.
-        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+        :param pulumi.Input[str] interface_id: The id of dedicated server network interface.
+        :param pulumi.Input[str] service_name: The id of the vrack. If omitted,
                the `OVH_VRACK_SERVICE` environment variable is used.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _DedicatedServerState.__new__(_DedicatedServerState)
+        __props__ = _DedicatedServerInterfaceState.__new__(_DedicatedServerInterfaceState)
 
-        __props__.__dict__["server_id"] = server_id
+        __props__.__dict__["interface_id"] = interface_id
         __props__.__dict__["service_name"] = service_name
-        return DedicatedServer(resource_name, opts=opts, __props__=__props__)
+        return DedicatedServerInterface(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="serverId")
-    def server_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="interfaceId")
+    def interface_id(self) -> pulumi.Output[str]:
         """
-        The id of the dedicated server.
+        The id of dedicated server network interface.
         """
-        return pulumi.get(self, "server_id")
+        return pulumi.get(self, "interface_id")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The service name of the vrack. If omitted,
+        The id of the vrack. If omitted,
         the `OVH_VRACK_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/ip_address.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/ip_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,14 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Attach an IP block to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -185,15 +184,14 @@
                     value="FR",
                 )],
             ))
         vrackblock = ovh.vrack.IpAddress("vrackblock",
             service_name=vrack_vrack.service_name,
             block=ipblock_ip_service.ip)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] block: Your IP block.
         :param pulumi.Input[str] service_name: The internal name of your vrack
         """
         ...
@@ -203,15 +201,14 @@
                  args: IpAddressArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Attach an IP block to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -242,15 +239,14 @@
                     value="FR",
                 )],
             ))
         vrackblock = ovh.vrack.IpAddress("vrackblock",
             service_name=vrack_vrack.service_name,
             block=ipblock_ip_service.ip)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IpAddressArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/ip_loadbalancing.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/ip_loadbalancing.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,24 +98,22 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Attach an IP Load Balancing to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         viplb = ovh.vrack.IpLoadbalancing("viplb",
             loadbalancing_id="yyy",
             service_name="xxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] loadbalancing_id: The id of the IP Load Balancing.
         :param pulumi.Input[str] service_name: The id of the vrack.
         """
         ...
@@ -125,24 +123,22 @@
                  args: IpLoadbalancingArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Attach an IP Load Balancing to a VRack.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         viplb = ovh.vrack.IpLoadbalancing("viplb",
             loadbalancing_id="yyy",
             service_name="xxx")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IpLoadbalancingArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/outputs.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh/vrack/vrack.py` & `pulumi_ovh-0.44.0/pulumi_ovh/vrack/vrack.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,35 @@
 @pulumi.input_type
 class VrackArgs:
     def __init__(__self__, *,
                  ovh_subsidiary: pulumi.Input[str],
                  plan: pulumi.Input['VrackPlanArgs'],
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]] = None):
         """
         The set of arguments for constructing a Vrack resource.
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input['VrackPlanArgs'] plan: Product Plan to order
         :param pulumi.Input[str] description: yourvrackdescription
         :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]] orders: Details about an Order
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]] plan_options: Product Plan to order
         """
         pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
         pulumi.set(__self__, "plan", plan)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
         if payment_mean is not None:
             warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
             pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
         if payment_mean is not None:
             pulumi.set(__self__, "payment_mean", payment_mean)
         if plan_options is not None:
             pulumi.set(__self__, "plan_options", plan_options)
@@ -90,14 +94,26 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]]:
+        """
+        Details about an Order
+        """
+        return pulumi.get(self, "orders")
+
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
+
+    @property
     @pulumi.getter(name="paymentMean")
     def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
         Ovh payment mode
         """
         warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
         pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
@@ -282,23 +298,23 @@
 class Vrack(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['VrackPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -310,45 +326,44 @@
             description="my vrack",
             plan=ovh.vrack.VrackPlanArgs(
                 duration=vrack_cart_product_plan.selected_prices[0].duration,
                 plan_code=vrack_cart_product_plan.plan_code,
                 pricing_mode=vrack_cart_product_plan.selected_prices[0].pricing_mode,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
-        vRack can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders).
+        vRack can be imported using the `service_name`.
 
         bash
 
         ```sh
-        $ pulumi import ovh:Vrack/vrack:Vrack vrack order_id
+        $ pulumi import ovh:Vrack/vrack:Vrack vrack service_name
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: yourvrackdescription
         :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackOrderArgs']]]] orders: Details about an Order
         :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         :param pulumi.Input[str] payment_mean: Ovh payment mode
         :param pulumi.Input[pulumi.InputType['VrackPlanArgs']] plan: Product Plan to order
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]] plan_options: Product Plan to order
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VrackArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         myaccount = ovh.Me.get_me()
         mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
         vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
@@ -360,24 +375,23 @@
             description="my vrack",
             plan=ovh.vrack.VrackPlanArgs(
                 duration=vrack_cart_product_plan.selected_prices[0].duration,
                 plan_code=vrack_cart_product_plan.plan_code,
                 pricing_mode=vrack_cart_product_plan.selected_prices[0].pricing_mode,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
-        vRack can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders).
+        vRack can be imported using the `service_name`.
 
         bash
 
         ```sh
-        $ pulumi import ovh:Vrack/vrack:Vrack vrack order_id
+        $ pulumi import ovh:Vrack/vrack:Vrack vrack service_name
         ```
 
         :param str resource_name: The name of the resource.
         :param VrackArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -389,14 +403,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackOrderArgs']]]]] = None,
                  ovh_subsidiary: Optional[pulumi.Input[str]] = None,
                  payment_mean: Optional[pulumi.Input[str]] = None,
                  plan: Optional[pulumi.Input[pulumi.InputType['VrackPlanArgs']]] = None,
                  plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -404,24 +419,24 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VrackArgs.__new__(VrackArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
+            __props__.__dict__["orders"] = orders
             if ovh_subsidiary is None and not opts.urn:
                 raise TypeError("Missing required property 'ovh_subsidiary'")
             __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
             __props__.__dict__["payment_mean"] = payment_mean
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
             __props__.__dict__["plan_options"] = plan_options
             __props__.__dict__["vrack_urn"] = None
-            __props__.__dict__["orders"] = None
             __props__.__dict__["service_name"] = None
         super(Vrack, __self__).__init__(
             'ovh:Vrack/vrack:Vrack',
             resource_name,
             __props__,
             opts)
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh.egg-info/PKG-INFO` & `pulumi_ovh-0.44.0/pulumi_ovh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-ovh
-Version: 0.43.1
+Version: 0.44.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.43.1 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.44.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.43.1/pulumi_ovh.egg-info/SOURCES.txt` & `pulumi_ovh-0.44.0/pulumi_ovh.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 pulumi_ovh/__init__.py
 pulumi_ovh/_utilities.py
+pulumi_ovh/get_installation_template.py
 pulumi_ovh/get_installation_templates.py
 pulumi_ovh/get_server.py
 pulumi_ovh/get_servers.py
 pulumi_ovh/get_vrack_networks.py
 pulumi_ovh/outputs.py
 pulumi_ovh/provider.py
 pulumi_ovh/pulumi-plugin.json
@@ -222,24 +223,21 @@
 pulumi_ovh/me/get_identity_user.py
 pulumi_ovh/me/get_identity_users.py
 pulumi_ovh/me/get_installation_template.py
 pulumi_ovh/me/get_installation_templates.py
 pulumi_ovh/me/get_me.py
 pulumi_ovh/me/get_paymentmean_bank_account.py
 pulumi_ovh/me/get_paymentmean_credit_card.py
-pulumi_ovh/me/get_ssh_key.py
-pulumi_ovh/me/get_ssh_keys.py
 pulumi_ovh/me/identity_group.py
 pulumi_ovh/me/identity_user.py
 pulumi_ovh/me/installation_template.py
 pulumi_ovh/me/installation_template_partition_scheme.py
 pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
 pulumi_ovh/me/installation_template_partition_scheme_partition.py
 pulumi_ovh/me/outputs.py
-pulumi_ovh/me/ssh_key.py
 pulumi_ovh/order/__init__.py
 pulumi_ovh/order/get_cart.py
 pulumi_ovh/order/get_cart_product.py
 pulumi_ovh/order/get_cart_product_options.py
 pulumi_ovh/order/get_cart_product_options_plan.py
 pulumi_ovh/order/get_cart_product_plan.py
 pulumi_ovh/order/outputs.py
```

### Comparing `pulumi_ovh-0.43.1/setup.py` & `pulumi_ovh-0.44.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.43.1"
+VERSION = "0.44.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ovh Pulumi Package - Development Version"
```

