# Comparing `tmp/cartography-0.90.0rc2.tar.gz` & `tmp/cartography-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartography-0.90.0rc2.tar", last modified: Thu Feb 22 23:52:51 2024, max compression
+gzip compressed data, was "cartography-0.91.0.tar", last modified: Wed May 15 18:44:57 2024, max compression
```

## Comparing `cartography-0.90.0rc2.tar` & `cartography-0.91.0.tar`

### file list

```diff
@@ -1,389 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.398251 cartography-0.90.0rc2/cartography/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30059 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.398251 cartography-0.90.0rc2/cartography/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.398251 cartography-0.90.0rc2/cartography/client/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/client/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/client/aws/iam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.398251 cartography-0.90.0rc2/cartography/client/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/client/core/tx.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.402251 cartography-0.90.0rc2/cartography/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27804 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/indexes.cypher
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.402251 cartography-0.90.0rc2/cartography/data/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.402251 cartography-0.90.0rc2/cartography/data/jobs/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_iaminstance.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_iaminstanceprofile.json
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_keypair_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_eks_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_foreign_accounts.json
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_lambda_ecr.json
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_s3acl_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_gke_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_gke_basic_auth.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/analysis/gsuite_human_link.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.418251 cartography-0.90.0rc2/cartography/data/jobs/cleanup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_apigateway_details.json
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_dns_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_config_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ec2_launch_configurations_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_elasticache_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_internet_gateways_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_kms_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_lambda_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_redshift_clusters_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_secrets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_securityhub_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_tags_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_tgw_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_kms_details.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_s3_details.json
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_cors_details.json
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_mongodb_database_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_sql_database_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_table_resources_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_database_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_disks_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_virtual_machines_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_sql_server_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_storage_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_subscriptions_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_tenant_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/crowdstrike_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/digitalocean_project_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_forwarding_rules_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_dns_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_gke_cluster_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_storage_bucket_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/github_repos_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/github_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gsuite_ingest_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/gsuite_ingest_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/jamf_import_computers_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/kubernetes_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_compartments_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_groups_membership_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_policies_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_tenancy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/okta_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/okta_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/cleanup/pagerduty_import_cleanup.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.418251 cartography-0.90.0rc2/cartography/data/jobs/scoped_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/scoped_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/jobs/scoped_analysis/semgrep_sca_risk_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/data/permission_relationships.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.422251 cartography-0.90.0rc2/cartography/driftdetect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/add_shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/detect_deviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/get_states.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/driftdetect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.422251 cartography-0.90.0rc2/cartography/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/cleanupbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20108 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/querybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/graph/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.422251 cartography-0.90.0rc2/cartography/intel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.426252 cartography-0.90.0rc2/cartography/intel/aws/
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.430251 cartography-0.90.0rc2/cartography/intel/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/auto_scaling_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/load_balancer_v2s.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/tgw.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ec2/vpc_peerings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/eks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/emr.py
--rw-r--r--   0 runner    (1001) docker     (127)    32347 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/kms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/permission_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/rds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/resourcegroupstaggingapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/route53.py
--rw-r--r--   0 runner    (1001) docker     (127)    27034 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/securityhub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.430251 cartography-0.90.0rc2/cartography/intel/aws/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/util/arns.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/aws/util/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/azure/
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    41275 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/cosmosdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    32865 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    27393 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/azure/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/azure/util/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/bigfix/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/bigfix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/bigfix/computers.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/create_indexes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/crowdstrike/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crowdstrike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crowdstrike/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crowdstrike/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crowdstrike/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/crxcavator/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crxcavator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/crxcavator/crxcavator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.434251 cartography-0.90.0rc2/cartography/intel/cve/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/cve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/cve/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.438251 cartography-0.90.0rc2/cartography/intel/digitalocean/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/digitalocean/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/digitalocean/management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/digitalocean/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.438251 cartography-0.90.0rc2/cartography/intel/duo/
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/api_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/phones.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/duo/web_authn_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.438251 cartography-0.90.0rc2/cartography/intel/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48333 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/crm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/gke.py
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/github/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21766 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/github/repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/github/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/github/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/github/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/gsuite/
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/gsuite/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/jamf/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/jamf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/jamf/computers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/jamf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/kubernetes/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/lastpass/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/lastpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/lastpass/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.442252 cartography-0.90.0rc2/cartography/intel/oci/
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/oci/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/oci/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.446251 cartography-0.90.0rc2/cartography/intel/okta/
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/awssaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/factors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/sync_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/okta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.446251 cartography-0.90.0rc2/cartography/intel/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/escalation_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/pagerduty/vendors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.446251 cartography-0.90.0rc2/cartography/intel/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/semgrep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/intel/semgrep/findings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.446251 cartography-0.90.0rc2/cartography/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.446251 cartography-0.90.0rc2/cartography/models/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.450251 cartography-0.90.0rc2/cartography/models/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/dynamodb/gsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/dynamodb/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.450251 cartography-0.90.0rc2/cartography/models/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/loadbalancerv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/networkinterface_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/networkinterfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/privateip_networkinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/reservations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/securitygroup_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/securitygroup_networkinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/subnet_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/subnet_networkinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ec2/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.450251 cartography-0.90.0rc2/cartography/models/aws/eks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/eks/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/emr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.454251 cartography-0.90.0rc2/cartography/models/aws/inspector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/inspector/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/inspector/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.454251 cartography-0.90.0rc2/cartography/models/aws/ssm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ssm/instance_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/aws/ssm/instance_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.454251 cartography-0.90.0rc2/cartography/models/bigfix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/bigfix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/bigfix/bigfix_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/bigfix/bigfix_root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.454251 cartography-0.90.0rc2/cartography/models/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/core/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/core/relationships.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.454251 cartography-0.90.0rc2/cartography/models/cve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/cve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/cve/cve.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/cve/cve_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/cartography/models/duo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/api_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/phone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/duo/web_authn_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/cartography/models/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/github/teams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/cartography/models/lastpass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/lastpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/lastpass/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/lastpass/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/cartography/models/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/semgrep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/semgrep/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/semgrep/findings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/models/semgrep/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/cartography/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 23:52:51.458251 cartography-0.90.0rc2/cartography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 23:52:51.000000 cartography-0.90.0rc2/cartography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-22 23:52:51.462252 cartography-0.90.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-22 23:52:43.000000 cartography-0.90.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-15 18:44:46.000000 cartography-0.91.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 18:44:46.000000 cartography-0.91.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 18:44:57.450284 cartography-0.91.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-15 18:44:46.000000 cartography-0.91.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.390283 cartography-0.91.0/cartography/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31787 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/client/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/client/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/client/aws/iam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/client/core/tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27804 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/indexes.cypher
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/data/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.394283 cartography-0.91.0/cartography/data/jobs/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_iaminstance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_iaminstanceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_keypair_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_eks_asset_exposure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_foreign_accounts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_lambda_ecr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/gcp_gke_asset_exposure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/gcp_gke_basic_auth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/analysis/gsuite_human_link.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.410284 cartography-0.91.0/cartography/data/jobs/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_account_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_apigateway_details.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_config_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_configurations_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_elasticache_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_internet_gateways_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_kms_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_lambda_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_redshift_clusters_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_secrets_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_securityhub_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_snapshots_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_tags_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_tgw_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_kms_details.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/aws_s3_details.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_cors_details.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_mongodb_database_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_sql_database_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_table_resources_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_database_account_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_disks_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_snapshots_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_virtual_machines_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_sql_server_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_storage_account_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_subscriptions_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/azure_tenant_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/crowdstrike_import_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/digitalocean_project_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_forwarding_rules_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_dns_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_gke_cluster_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gcp_storage_bucket_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/github_repos_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/github_users_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gsuite_ingest_groups_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/gsuite_ingest_users_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/jamf_import_computers_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/kubernetes_import_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_compartments_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_groups_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_groups_membership_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_policies_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_users_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/oci_tenancy_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/okta_groups_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/okta_import_cleanup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/cleanup/pagerduty_import_cleanup.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.410284 cartography-0.91.0/cartography/data/jobs/scoped_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/scoped_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/jobs/scoped_analysis/semgrep_sca_risk_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/data/permission_relationships.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.414284 cartography-0.91.0/cartography/driftdetect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/add_shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/detect_deviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/get_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/shortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/driftdetect/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.414284 cartography-0.91.0/cartography/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/cleanupbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20108 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/querybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/graph/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.414284 cartography-0.91.0/cartography/intel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.422284 cartography-0.91.0/cartography/intel/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/auto_scaling_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/load_balancer_v2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/tgw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ec2/vpc_peerings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/eks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/emr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32347 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/kms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/permission_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25252 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/resourcegroupstaggingapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27034 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/securityhub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/aws/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/util/arns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/aws/util/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41275 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/cosmosdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32865 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27393 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/azure/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/azure/util/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/bigfix/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/bigfix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/bigfix/computers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/create_indexes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.426284 cartography-0.91.0/cartography/intel/crowdstrike/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crowdstrike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crowdstrike/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crowdstrike/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crowdstrike/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.430284 cartography-0.91.0/cartography/intel/crxcavator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crxcavator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13797 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/crxcavator/crxcavator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.430284 cartography-0.91.0/cartography/intel/cve/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/cve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/cve/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.430284 cartography-0.91.0/cartography/intel/digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/digitalocean/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/digitalocean/management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/digitalocean/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.430284 cartography-0.91.0/cartography/intel/duo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/api_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/phones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/duo/web_authn_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.430284 cartography-0.91.0/cartography/intel/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48333 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/crm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/gke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21766 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/github/repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/github/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/github/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/github/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/gsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/gsuite/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/jamf/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/jamf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/jamf/computers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/jamf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/kandji/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kandji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kandji/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/kubernetes/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.434284 cartography-0.91.0/cartography/intel/lastpass/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/lastpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/lastpass/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.438284 cartography-0.91.0/cartography/intel/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/oci/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/oci/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.438284 cartography-0.91.0/cartography/intel/okta/
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/awssaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/sync_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/okta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.438284 cartography-0.91.0/cartography/intel/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/escalation_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/pagerduty/vendors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.438284 cartography-0.91.0/cartography/intel/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/semgrep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/intel/semgrep/findings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.438284 cartography-0.91.0/cartography/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.442284 cartography-0.91.0/cartography/models/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.442284 cartography-0.91.0/cartography/models/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/dynamodb/gsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/dynamodb/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.442284 cartography-0.91.0/cartography/models/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/loadbalancerv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/networkinterface_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/networkinterfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/privateip_networkinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/reservations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/securitygroup_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/securitygroup_networkinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/subnet_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/subnet_networkinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ec2/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.442284 cartography-0.91.0/cartography/models/aws/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/eks/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/emr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/aws/inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/inspector/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/inspector/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/aws/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ssm/instance_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/aws/ssm/instance_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/bigfix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/bigfix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/bigfix/bigfix_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/bigfix/bigfix_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/core/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/core/relationships.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/cve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/cve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/cve/cve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/cve/cve_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.446284 cartography-0.91.0/cartography/models/duo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/api_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/phone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/duo/web_authn_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/cartography/models/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/github/teams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/cartography/models/kandji/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/kandji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/kandji/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/kandji/tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/cartography/models/lastpass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/lastpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/lastpass/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/lastpass/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/cartography/models/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/semgrep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/semgrep/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/semgrep/findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/models/semgrep/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14474 2024-05-15 18:44:46.000000 cartography-0.91.0/cartography/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:44:57.450284 cartography-0.91.0/cartography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 18:44:57.000000 cartography-0.91.0/cartography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 18:44:57.450284 cartography-0.91.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-15 18:44:46.000000 cartography-0.91.0/setup.py
```

### Comparing `cartography-0.90.0rc2/LICENSE` & `cartography-0.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/PKG-INFO` & `cartography-0.91.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartography
-Version: 0.90.0rc2
+Version: 0.91.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cartography-0.90.0rc2/README.md` & `cartography-0.91.0/README.md`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/cli.py` & `cartography-0.91.0/cartography/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -322,14 +322,38 @@
         parser.add_argument(
             '--jamf-password-env-var',
             type=str,
             default=None,
             help='The name of an environment variable containing a password with which to authenticate to Jamf.',
         )
         parser.add_argument(
+            '--kandji-base-uri',
+            type=str,
+            default=None,
+            help=(
+                'Your Kandji base URI, e.g. https://company.api.kandji.io.'
+                'Required if you are using the Kandji intel module. Ignored otherwise.'
+            ),
+        )
+        parser.add_argument(
+            '--kandji-tenant-id',
+            type=str,
+            default=None,
+            help=(
+                'Your Kandji tenant id e.g. company.'
+                'Required using the Kandji intel module. Ignored otherwise.'
+            ),
+        )
+        parser.add_argument(
+            '--kandji-token-env-var',
+            type=str,
+            default=None,
+            help='The name of an environment variable containing token with which to authenticate to Kandji.',
+        )
+        parser.add_argument(
             '--k8s-kubeconfig',
             default=None,
             type=str,
             help=(
                 'The path to kubeconfig file specifying context to access K8s cluster(s).'
             ),
         )
@@ -616,14 +640,34 @@
                 logger.warning("A Jamf base URI was provided but a user was not.")
             if not config.jamf_password:
                 logger.warning("A Jamf password could not be found.")
         else:
             config.jamf_user = None
             config.jamf_password = None
 
+        # Kandji config
+        if config.kandji_base_uri:
+            if config.kandji_token_env_var:
+                logger.debug(
+                    "Reading Kandji API token from environment variable '%s'.",
+                    config.kandji_token_env_var,
+                )
+                config.kandji_token = os.environ.get(config.kandji_token_env_var)
+            elif os.environ.get('KANDJI_TOKEN'):
+                logger.debug(
+                    "Reading Kandji API token from environment variable 'KANDJI_TOKEN'.",
+                )
+                config.kandji_token = os.environ.get('KANDJI_TOKEN')
+            else:
+                logger.warning("A Kandji base URI was provided but a token was not.")
+                config.kandji_token = None
+        else:
+            logger.warning("A Kandji base URI was not provided.")
+            config.kandji_base_uri = None
+
         if config.statsd_enabled:
             logger.debug(
                 f'statsd enabled. Sending metrics to server {config.statsd_host}:{config.statsd_port}. '
                 f'Metrics have prefix "{config.statsd_prefix}".',
             )
 
         # Pagerduty config
```

### Comparing `cartography-0.90.0rc2/cartography/client/aws/iam.py` & `cartography-0.91.0/cartography/client/aws/iam.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/client/core/tx.py` & `cartography-0.91.0/cartography/client/core/tx.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/config.py` & `cartography-0.91.0/cartography/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,20 @@
     :param permission_relationships_file: File path for the resource permission relationships file. Optional.
     :type jamf_base_uri: string
     :param jamf_base_uri: Jamf data provider base URI, e.g. https://example.com/JSSResource. Optional.
     :type jamf_user: string
     :param jamf_user: User name used to authenticate to the Jamf data provider. Optional.
     :type jamf_password: string
     :param jamf_password: Password used to authenticate to the Jamf data provider. Optional.
+    :type kandji_base_uri: string
+    :param kandji_base_uri: Kandji data provider base URI, e.g. https://company.api.kandji.io. Optional.
+    :type kandji_tenant_id: string
+    :param kandji_tenant_id: Kandji tenant id. e.g. company Optional.
+    :type kandji_token: string
+    :param kandji_token: Token used to authenticate to the Kandji data provider. Optional.
     :type statsd_enabled: bool
     :param statsd_enabled: Whether to collect statsd metrics such as sync execution times. Optional.
     :type statsd_host: str
     :param statsd_host: If statsd_enabled is True, send metrics to this host. Optional.
     :type: statsd_port: int
     :param statsd_port: If statsd_enabled is True, send metrics to this port on statsd_host. Optional.
     :type: k8s_kubeconfig: str
@@ -133,14 +139,17 @@
         okta_saml_role_regex=None,
         github_config=None,
         digitalocean_token=None,
         permission_relationships_file=None,
         jamf_base_uri=None,
         jamf_user=None,
         jamf_password=None,
+        kandji_base_uri=None,
+        kandji_tenant_id=None,
+        kandji_token=None,
         k8s_kubeconfig=None,
         statsd_enabled=False,
         statsd_prefix=None,
         statsd_host=None,
         statsd_port=None,
         pagerduty_api_key=None,
         pagerduty_request_timeout=None,
@@ -186,14 +195,17 @@
         self.okta_saml_role_regex = okta_saml_role_regex
         self.github_config = github_config
         self.digitalocean_token = digitalocean_token
         self.permission_relationships_file = permission_relationships_file
         self.jamf_base_uri = jamf_base_uri
         self.jamf_user = jamf_user
         self.jamf_password = jamf_password
+        self.kandji_base_uri = kandji_base_uri
+        self.kandji_tenant_id = kandji_tenant_id
+        self.kandji_token = kandji_token
         self.k8s_kubeconfig = k8s_kubeconfig
         self.statsd_enabled = statsd_enabled
         self.statsd_prefix = statsd_prefix
         self.statsd_host = statsd_host
         self.statsd_port = statsd_port
         self.pagerduty_api_key = pagerduty_api_key
         self.pagerduty_request_timeout = pagerduty_request_timeout
```

### Comparing `cartography-0.90.0rc2/cartography/data/indexes.cypher` & `cartography-0.91.0/cartography/data/indexes.cypher`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_iaminstanceprofile.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_iaminstanceprofile.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_ec2_keypair_analysis.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_ec2_keypair_analysis.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_eks_asset_exposure.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_eks_asset_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_foreign_accounts.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_foreign_accounts.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_lambda_ecr.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_lambda_ecr.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/aws_s3acl_analysis.json` & `cartography-0.91.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json` & `cartography-0.91.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_gke_asset_exposure.json` & `cartography-0.91.0/cartography/data/jobs/analysis/gcp_gke_asset_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/gcp_gke_basic_auth.json` & `cartography-0.91.0/cartography/data/jobs/analysis/gcp_gke_basic_auth.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/analysis/gsuite_human_link.json` & `cartography-0.91.0/cartography/data/jobs/analysis/gsuite_human_link.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_dns_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_config_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_config_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_elasticache_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_elasticache_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_es_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_kms_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_kms_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_lambda_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_lambda_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_redshift_clusters_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_redshift_clusters_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_snapshots_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_snapshots_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_tags_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_tags_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_tgw_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_tgw_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_cors_details.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_cors_details.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_mongodb_database_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_mongodb_database_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_sql_database_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_sql_database_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_cosmosdb_table_resources_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_cosmosdb_table_resources_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_database_account_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_database_account_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_disks_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_disks_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_snapshots_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_snapshots_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_import_virtual_machines_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_import_virtual_machines_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_sql_server_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_sql_server_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/azure_storage_account_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/azure_storage_account_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/crowdstrike_import_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/crowdstrike_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/digitalocean_project_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/digitalocean_project_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_forwarding_rules_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_forwarding_rules_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_dns_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_dns_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_gke_cluster_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_gke_cluster_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gcp_storage_bucket_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gcp_storage_bucket_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/github_repos_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/github_repos_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/github_users_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/github_users_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/gsuite_ingest_groups_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/gsuite_ingest_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/kubernetes_import_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/kubernetes_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_groups_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/oci_import_policies_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/oci_import_policies_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/okta_groups_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/okta_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/okta_import_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/okta_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/cleanup/pagerduty_import_cleanup.json` & `cartography-0.91.0/cartography/data/jobs/cleanup/pagerduty_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/jobs/scoped_analysis/semgrep_sca_risk_analysis.json` & `cartography-0.91.0/cartography/data/jobs/scoped_analysis/semgrep_sca_risk_analysis.json`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/data/permission_relationships.yaml` & `cartography-0.91.0/cartography/data/permission_relationships.yaml`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/add_shortcut.py` & `cartography-0.91.0/cartography/driftdetect/add_shortcut.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/cli.py` & `cartography-0.91.0/cartography/driftdetect/cli.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/config.py` & `cartography-0.91.0/cartography/driftdetect/config.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/detect_deviations.py` & `cartography-0.91.0/cartography/driftdetect/detect_deviations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/get_states.py` & `cartography-0.91.0/cartography/driftdetect/get_states.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/model.py` & `cartography-0.91.0/cartography/driftdetect/model.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/reporter.py` & `cartography-0.91.0/cartography/driftdetect/reporter.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/serializers.py` & `cartography-0.91.0/cartography/driftdetect/serializers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/storage.py` & `cartography-0.91.0/cartography/driftdetect/storage.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/driftdetect/util.py` & `cartography-0.91.0/cartography/driftdetect/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/graph/cleanupbuilder.py` & `cartography-0.91.0/cartography/graph/cleanupbuilder.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/graph/context.py` & `cartography-0.91.0/cartography/graph/context.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/graph/job.py` & `cartography-0.91.0/cartography/graph/job.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/graph/querybuilder.py` & `cartography-0.91.0/cartography/graph/querybuilder.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/graph/statement.py` & `cartography-0.91.0/cartography/graph/statement.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/analysis.py` & `cartography-0.91.0/cartography/intel/analysis.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/__init__.py` & `cartography-0.91.0/cartography/intel/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/apigateway.py` & `cartography-0.91.0/cartography/intel/aws/apigateway.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/config.py` & `cartography-0.91.0/cartography/intel/aws/config.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/dynamodb.py` & `cartography-0.91.0/cartography/intel/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/auto_scaling_groups.py` & `cartography-0.91.0/cartography/intel/aws/ec2/auto_scaling_groups.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/elastic_ip_addresses.py` & `cartography-0.91.0/cartography/intel/aws/ec2/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/images.py` & `cartography-0.91.0/cartography/intel/aws/ec2/images.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from cartography.util import timeit
 
 logger = logging.getLogger(__name__)
 
 
 @timeit
 def get_images_in_use(neo4j_session: neo4j.Session, region: str, current_aws_account_id: str) -> List[str]:
-    # We use OPTIONAL here to allow query chaining with queries that may not match.
     get_images_query = """
-    OPTIONAL MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(i:EC2Instance)
+    MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(i:EC2Instance)
     WHERE i.region = $Region
-    WITH collect(DISTINCT i.imageid) AS images
-    OPTIONAL MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(lc:LaunchConfiguration)
+    RETURN DISTINCT(i.imageid) as image
+    UNION
+    MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(lc:LaunchConfiguration)
     WHERE lc.region = $Region
-    WITH collect(DISTINCT lc.image_id)+images AS images
-    OPTIONAL MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(ltv:LaunchTemplateVersion)
+    RETURN DISTINCT(lc.image_id) as image
+    UNION
+    MATCH (:AWSAccount{id: $AWS_ACCOUNT_ID})-[:RESOURCE]->(ltv:LaunchTemplateVersion)
     WHERE ltv.region = $Region
-    WITH collect(DISTINCT ltv.image_id)+images AS images
-    RETURN images
+    RETURN DISTINCT(ltv.image_id) as image
     """
     results = neo4j_session.run(get_images_query, AWS_ACCOUNT_ID=current_aws_account_id, Region=region)
     images = []
     for r in results:
-        images.extend(r['images'])
+        images.append(r['image'])
     return images
 
 
 @timeit
 @aws_handle_regions
 def get_images(boto3_session: boto3.session.Session, region: str, image_ids: List[str]) -> List[Dict]:
     client = boto3_session.client('ec2', region_name=region, config=get_botocore_config())
```

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/instances.py` & `cartography-0.91.0/cartography/intel/aws/ec2/instances.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/internet_gateways.py` & `cartography-0.91.0/cartography/intel/aws/ec2/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/key_pairs.py` & `cartography-0.91.0/cartography/intel/aws/ec2/key_pairs.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/launch_templates.py` & `cartography-0.91.0/cartography/intel/aws/ec2/launch_templates.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/load_balancer_v2s.py` & `cartography-0.91.0/cartography/intel/aws/ec2/load_balancer_v2s.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/load_balancers.py` & `cartography-0.91.0/cartography/intel/aws/ec2/load_balancers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/network_interfaces.py` & `cartography-0.91.0/cartography/intel/aws/ec2/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/reserved_instances.py` & `cartography-0.91.0/cartography/intel/aws/ec2/reserved_instances.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/security_groups.py` & `cartography-0.91.0/cartography/intel/aws/ec2/security_groups.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/snapshots.py` & `cartography-0.91.0/cartography/intel/aws/ec2/snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,18 @@
     other_snapshot_ids = set(in_use_snapshot_ids) - self_owned_snapshot_ids
     if other_snapshot_ids:
         try:
             for page in paginator.paginate(SnapshotIds=list(other_snapshot_ids)):
                 snapshots.extend(page['Snapshots'])
         except ClientError as e:
             if e.response['Error']['Code'] == 'InvalidSnapshot.NotFound':
-                logger.warning(f"Failed to retrieve page of in-use, \
-                    not owned snapshots. Continuing anyway. Error - {e}")
+                logger.warning(
+                    f"Failed to retrieve page of in-use, \
+                    not owned snapshots. Continuing anyway. Error - {e}",
+                )
             else:
                 raise
 
     return snapshots
 
 
 @timeit
```

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/subnets.py` & `cartography-0.91.0/cartography/intel/aws/ec2/subnets.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/tgw.py` & `cartography-0.91.0/cartography/intel/aws/ec2/tgw.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/volumes.py` & `cartography-0.91.0/cartography/intel/aws/ec2/volumes.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/vpc.py` & `cartography-0.91.0/cartography/intel/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ec2/vpc_peerings.py` & `cartography-0.91.0/cartography/intel/aws/ec2/vpc_peerings.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ecr.py` & `cartography-0.91.0/cartography/intel/aws/ecr.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ecs.py` & `cartography-0.91.0/cartography/intel/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/eks.py` & `cartography-0.91.0/cartography/intel/aws/eks.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/elasticache.py` & `cartography-0.91.0/cartography/intel/aws/elasticache.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/elasticsearch.py` & `cartography-0.91.0/cartography/intel/aws/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/emr.py` & `cartography-0.91.0/cartography/intel/aws/emr.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/iam.py` & `cartography-0.91.0/cartography/intel/aws/iam.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/inspector.py` & `cartography-0.91.0/cartography/intel/aws/inspector.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/kms.py` & `cartography-0.91.0/cartography/intel/aws/kms.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/lambda_function.py` & `cartography-0.91.0/cartography/intel/aws/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/organizations.py` & `cartography-0.91.0/cartography/intel/aws/organizations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/permission_relationships.py` & `cartography-0.91.0/cartography/intel/aws/permission_relationships.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/rds.py` & `cartography-0.91.0/cartography/intel/aws/rds.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/redshift.py` & `cartography-0.91.0/cartography/intel/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/resourcegroupstaggingapi.py` & `cartography-0.91.0/cartography/intel/aws/resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/resources.py` & `cartography-0.91.0/cartography/intel/aws/resources.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/route53.py` & `cartography-0.91.0/cartography/intel/aws/route53.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/s3.py` & `cartography-0.91.0/cartography/intel/aws/s3.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/secretsmanager.py` & `cartography-0.91.0/cartography/intel/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/securityhub.py` & `cartography-0.91.0/cartography/intel/aws/securityhub.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/sqs.py` & `cartography-0.91.0/cartography/intel/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/ssm.py` & `cartography-0.91.0/cartography/intel/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/util/arns.py` & `cartography-0.91.0/cartography/intel/aws/util/arns.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/aws/util/common.py` & `cartography-0.91.0/cartography/intel/aws/util/common.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/__init__.py` & `cartography-0.91.0/cartography/intel/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/compute.py` & `cartography-0.91.0/cartography/intel/azure/compute.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/cosmosdb.py` & `cartography-0.91.0/cartography/intel/azure/cosmosdb.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/sql.py` & `cartography-0.91.0/cartography/intel/azure/sql.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/storage.py` & `cartography-0.91.0/cartography/intel/azure/storage.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/subscription.py` & `cartography-0.91.0/cartography/intel/azure/subscription.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/tenant.py` & `cartography-0.91.0/cartography/intel/azure/tenant.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/azure/util/credentials.py` & `cartography-0.91.0/cartography/intel/azure/util/credentials.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/bigfix/__init__.py` & `cartography-0.91.0/cartography/intel/bigfix/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/bigfix/computers.py` & `cartography-0.91.0/cartography/intel/bigfix/computers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/create_indexes.py` & `cartography-0.91.0/cartography/intel/create_indexes.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/crowdstrike/__init__.py` & `cartography-0.91.0/cartography/intel/crowdstrike/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/crowdstrike/endpoints.py` & `cartography-0.91.0/cartography/intel/crowdstrike/endpoints.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/crowdstrike/spotlight.py` & `cartography-0.91.0/cartography/intel/crowdstrike/spotlight.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/crxcavator/__init__.py` & `cartography-0.91.0/cartography/intel/crxcavator/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/crxcavator/crxcavator.py` & `cartography-0.91.0/cartography/intel/crxcavator/crxcavator.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/cve/__init__.py` & `cartography-0.91.0/cartography/intel/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/cve/feed.py` & `cartography-0.91.0/cartography/intel/cve/feed.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/digitalocean/__init__.py` & `cartography-0.91.0/cartography/intel/digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/digitalocean/compute.py` & `cartography-0.91.0/cartography/intel/digitalocean/compute.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/digitalocean/management.py` & `cartography-0.91.0/cartography/intel/digitalocean/management.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/digitalocean/platform.py` & `cartography-0.91.0/cartography/intel/digitalocean/platform.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/dns.py` & `cartography-0.91.0/cartography/intel/dns.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/__init__.py` & `cartography-0.91.0/cartography/intel/duo/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/api_host.py` & `cartography-0.91.0/cartography/intel/duo/api_host.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/endpoints.py` & `cartography-0.91.0/cartography/intel/duo/endpoints.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/groups.py` & `cartography-0.91.0/cartography/intel/duo/groups.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/phones.py` & `cartography-0.91.0/cartography/intel/duo/phones.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/tokens.py` & `cartography-0.91.0/cartography/intel/duo/tokens.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/users.py` & `cartography-0.91.0/cartography/intel/duo/users.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/duo/web_authn_credentials.py` & `cartography-0.91.0/cartography/intel/duo/web_authn_credentials.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/__init__.py` & `cartography-0.91.0/cartography/intel/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/compute.py` & `cartography-0.91.0/cartography/intel/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/crm.py` & `cartography-0.91.0/cartography/intel/gcp/crm.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/dns.py` & `cartography-0.91.0/cartography/intel/gcp/dns.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/gke.py` & `cartography-0.91.0/cartography/intel/gcp/gke.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gcp/storage.py` & `cartography-0.91.0/cartography/intel/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/github/__init__.py` & `cartography-0.91.0/cartography/intel/github/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/github/repos.py` & `cartography-0.91.0/cartography/intel/github/repos.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/github/teams.py` & `cartography-0.91.0/cartography/intel/github/teams.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,18 +53,21 @@
     result = {}
     for team in team_raw_data:
         team_name = team['slug']
         repo_count = team['repositories']['totalCount']
 
         team_repos = _get_team_repos(org, api_url, token, team_name) if repo_count > 0 else None
 
-        # Shape = [(repo_url, 'WRITE'), ...]]
-        repo_urls = [t['url'] for t in team_repos.nodes] if team_repos else []
-        repo_permissions = [t['permission'] for t in team_repos.edges] if team_repos else []
+        repo_urls = []
+        repo_permissions = []
+        if team_repos:
+            repo_urls = [t['url'] for t in team_repos.nodes] if team_repos.nodes else []
+            repo_permissions = [t['permission'] for t in team_repos.edges] if team_repos.edges else []
 
+        # Shape = [(repo_url, 'WRITE'), ...]]
         result[team_name] = list(zip(repo_urls, repo_permissions))
     return result
 
 
 @timeit
 def _get_team_repos(org: str, api_url: str, token: str, team: str) -> PaginatedGraphqlData:
     team_repos_gql = """
```

### Comparing `cartography-0.90.0rc2/cartography/intel/github/users.py` & `cartography-0.91.0/cartography/intel/github/users.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/github/util.py` & `cartography-0.91.0/cartography/intel/github/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,20 +77,20 @@
             f'call_github_api() response has errors, please investigate. Raw response: {response_json["errors"]}; '
             f'continuing sync.',
         )
     return response_json  # type: ignore
 
 
 def fetch_page(
-        token: str,
-        api_url: str,
-        organization: str,
-        query: str,
-        cursor: Optional[str] = None,
-        **kwargs: Any,
+    token: str,
+    api_url: str,
+    organization: str,
+    query: str,
+    cursor: Optional[str] = None,
+    **kwargs: Any,
 ) -> Dict[str, Any]:
     """
     Return a single page of max size 100 elements from the Github api_url using the given `query` and `cursor` params.
     :param token: The API token as string. Must have permission for the object being paginated.
     :param api_url: The Github API endpoint as string.
     :param organization: The name of the target Github organization as string.
     :param query: The GraphQL query, e.g. `GITHUB_ORG_USERS_PAGINATED_GRAPHQL`
@@ -135,14 +135,15 @@
     `resource_inner_type`.
     :param kwargs: Additional key-value args (other than `login` and `cursor`) to pass to the GraphQL query variables.
     :return: A 2-tuple containing 1. A list of data items of the given `resource_type` and `field_name`,  and 2. a dict
     containing the `url` and the `login` fields of the organization that the items belong to.
     """
     cursor = None
     has_next_page = True
+    org_data: Dict[str, Any] = {}
     data: PaginatedGraphqlData = PaginatedGraphqlData(nodes=[], edges=[])
     retry = 0
 
     while has_next_page:
         exc: Any = None
         try:
             # In the future, we may use also use the rateLimit object from the graphql response.
@@ -166,20 +167,37 @@
                 exc_info=True,
             )
             raise exc
         elif retry > 0:
             time.sleep(2 ** retry)
             continue
 
+        if 'data' not in resp:
+            logger.warning(
+                f'Got no "data" attribute in response: {resp}. '
+                f'Stopping requests for organization: {organization} and '
+                f'resource_type: {resource_type}',
+            )
+            has_next_page = False
+            continue
+
         resource = resp['data']['organization'][resource_type]
         if resource_inner_type:
             resource = resp['data']['organization'][resource_type][resource_inner_type]
 
         # Allow for paginating both nodes and edges fields of the GitHub GQL structure.
         data.nodes.extend(resource.get('nodes', []))
         data.edges.extend(resource.get('edges', []))
 
         cursor = resource['pageInfo']['endCursor']
         has_next_page = resource['pageInfo']['hasNextPage']
-
-    org_data = {'url': resp['data']['organization']['url'], 'login': resp['data']['organization']['login']}
+        if not org_data:
+            org_data = {
+                'url': resp['data']['organization']['url'],
+                'login': resp['data']['organization']['login'],
+            }
+
+    if not org_data:
+        raise ValueError(
+            f"Didn't get any organization data for organization: {organization} and resource_type: {resource_type}",
+        )
     return data, org_data
```

### Comparing `cartography-0.90.0rc2/cartography/intel/gsuite/__init__.py` & `cartography-0.91.0/cartography/intel/gsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/gsuite/api.py` & `cartography-0.91.0/cartography/intel/gsuite/api.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/jamf/computers.py` & `cartography-0.91.0/cartography/intel/jamf/computers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/jamf/util.py` & `cartography-0.91.0/cartography/intel/jamf/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/__init__.py` & `cartography-0.91.0/cartography/intel/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/namespaces.py` & `cartography-0.91.0/cartography/intel/kubernetes/namespaces.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/pods.py` & `cartography-0.91.0/cartography/intel/kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/secrets.py` & `cartography-0.91.0/cartography/intel/kubernetes/secrets.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/services.py` & `cartography-0.91.0/cartography/intel/kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/kubernetes/util.py` & `cartography-0.91.0/cartography/intel/kubernetes/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/lastpass/__init__.py` & `cartography-0.91.0/cartography/intel/lastpass/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/lastpass/users.py` & `cartography-0.91.0/cartography/intel/lastpass/users.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/oci/__init__.py` & `cartography-0.91.0/cartography/intel/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/oci/iam.py` & `cartography-0.91.0/cartography/intel/oci/iam.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/oci/organizations.py` & `cartography-0.91.0/cartography/intel/oci/organizations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/oci/utils.py` & `cartography-0.91.0/cartography/intel/oci/utils.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/__init__.py` & `cartography-0.91.0/cartography/intel/okta/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/applications.py` & `cartography-0.91.0/cartography/intel/okta/applications.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/awssaml.py` & `cartography-0.91.0/cartography/intel/okta/awssaml.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/factors.py` & `cartography-0.91.0/cartography/intel/okta/factors.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/groups.py` & `cartography-0.91.0/cartography/intel/okta/groups.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/organization.py` & `cartography-0.91.0/cartography/intel/okta/organization.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/origins.py` & `cartography-0.91.0/cartography/intel/okta/origins.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/roles.py` & `cartography-0.91.0/cartography/intel/okta/roles.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/sync_state.py` & `cartography-0.91.0/cartography/intel/okta/sync_state.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/users.py` & `cartography-0.91.0/cartography/intel/okta/users.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/okta/utils.py` & `cartography-0.91.0/cartography/intel/okta/utils.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/__init__.py` & `cartography-0.91.0/cartography/intel/pagerduty/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/escalation_policies.py` & `cartography-0.91.0/cartography/intel/pagerduty/escalation_policies.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/schedules.py` & `cartography-0.91.0/cartography/intel/pagerduty/schedules.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/services.py` & `cartography-0.91.0/cartography/intel/pagerduty/services.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/teams.py` & `cartography-0.91.0/cartography/intel/pagerduty/teams.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/users.py` & `cartography-0.91.0/cartography/intel/pagerduty/users.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/pagerduty/vendors.py` & `cartography-0.91.0/cartography/intel/pagerduty/vendors.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/semgrep/__init__.py` & `cartography-0.91.0/cartography/intel/semgrep/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/intel/semgrep/findings.py` & `cartography-0.91.0/cartography/intel/semgrep/findings.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/dynamodb/gsi.py` & `cartography-0.91.0/cartography/models/aws/dynamodb/gsi.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/dynamodb/tables.py` & `cartography-0.91.0/cartography/models/aws/dynamodb/tables.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/images.py` & `cartography-0.91.0/cartography/models/aws/ec2/images.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/instances.py` & `cartography-0.91.0/cartography/models/aws/ec2/instances.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/keypairs.py` & `cartography-0.91.0/cartography/models/aws/ec2/keypairs.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/networkinterface_instance.py` & `cartography-0.91.0/cartography/models/aws/ec2/networkinterface_instance.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/networkinterfaces.py` & `cartography-0.91.0/cartography/models/aws/ec2/networkinterfaces.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/privateip_networkinterface.py` & `cartography-0.91.0/cartography/models/aws/ec2/privateip_networkinterface.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/reservations.py` & `cartography-0.91.0/cartography/models/aws/ec2/reservations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/securitygroup_instance.py` & `cartography-0.91.0/cartography/models/aws/ec2/securitygroup_instance.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/securitygroup_networkinterface.py` & `cartography-0.91.0/cartography/models/aws/ec2/securitygroup_networkinterface.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/subnet_instance.py` & `cartography-0.91.0/cartography/models/aws/ec2/subnet_instance.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/subnet_networkinterface.py` & `cartography-0.91.0/cartography/models/aws/ec2/subnet_networkinterface.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ec2/volumes.py` & `cartography-0.91.0/cartography/models/aws/ec2/volumes.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/eks/clusters.py` & `cartography-0.91.0/cartography/models/aws/eks/clusters.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/emr.py` & `cartography-0.91.0/cartography/models/aws/emr.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/inspector/findings.py` & `cartography-0.91.0/cartography/models/aws/inspector/findings.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/inspector/packages.py` & `cartography-0.91.0/cartography/models/aws/inspector/packages.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ssm/instance_information.py` & `cartography-0.91.0/cartography/models/aws/ssm/instance_information.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/aws/ssm/instance_patch.py` & `cartography-0.91.0/cartography/models/aws/ssm/instance_patch.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/bigfix/bigfix_computer.py` & `cartography-0.91.0/cartography/models/bigfix/bigfix_computer.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/bigfix/bigfix_root.py` & `cartography-0.91.0/cartography/models/bigfix/bigfix_root.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/core/common.py` & `cartography-0.91.0/cartography/models/core/common.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/core/nodes.py` & `cartography-0.91.0/cartography/models/core/nodes.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/core/relationships.py` & `cartography-0.91.0/cartography/models/core/relationships.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/cve/cve.py` & `cartography-0.91.0/cartography/models/cve/cve.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/cve/cve_feed.py` & `cartography-0.91.0/cartography/models/cve/cve_feed.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/api_host.py` & `cartography-0.91.0/cartography/models/duo/api_host.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/endpoint.py` & `cartography-0.91.0/cartography/models/duo/endpoint.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/group.py` & `cartography-0.91.0/cartography/models/duo/group.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/phone.py` & `cartography-0.91.0/cartography/models/duo/phone.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/token.py` & `cartography-0.91.0/cartography/models/duo/token.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/user.py` & `cartography-0.91.0/cartography/models/duo/user.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/duo/web_authn_credential.py` & `cartography-0.91.0/cartography/models/duo/web_authn_credential.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/github/teams.py` & `cartography-0.91.0/cartography/models/github/teams.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/lastpass/tenant.py` & `cartography-0.91.0/cartography/models/lastpass/tenant.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/lastpass/user.py` & `cartography-0.91.0/cartography/models/lastpass/user.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/semgrep/deployment.py` & `cartography-0.91.0/cartography/models/semgrep/deployment.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/semgrep/findings.py` & `cartography-0.91.0/cartography/models/semgrep/findings.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/models/semgrep/locations.py` & `cartography-0.91.0/cartography/models/semgrep/locations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/stats.py` & `cartography-0.91.0/cartography/stats.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography/sync.py` & `cartography-0.91.0/cartography/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import cartography.intel.crxcavator.crxcavator
 import cartography.intel.cve
 import cartography.intel.digitalocean
 import cartography.intel.duo
 import cartography.intel.gcp
 import cartography.intel.github
 import cartography.intel.gsuite
+import cartography.intel.kandji
 import cartography.intel.kubernetes
 import cartography.intel.lastpass
 import cartography.intel.oci
 import cartography.intel.okta
 import cartography.intel.semgrep
 from cartography.config import Config
 from cartography.stats import set_stats_client
@@ -46,14 +47,15 @@
     'gsuite': cartography.intel.gsuite.start_gsuite_ingestion,
     'crxcavator': cartography.intel.crxcavator.start_extension_ingestion,
     'cve': cartography.intel.cve.start_cve_ingestion,
     'oci': cartography.intel.oci.start_oci_ingestion,
     'okta': cartography.intel.okta.start_okta_ingestion,
     'github': cartography.intel.github.start_github_ingestion,
     'digitalocean': cartography.intel.digitalocean.start_digitalocean_ingestion,
+    'kandji': cartography.intel.kandji.start_kandji_ingestion,
     'kubernetes': cartography.intel.kubernetes.start_k8s_ingestion,
     'lastpass': cartography.intel.lastpass.start_lastpass_ingestion,
     'bigfix': cartography.intel.bigfix.start_bigfix_ingestion,
     'duo': cartography.intel.duo.start_duo_ingestion,
     'semgrep': cartography.intel.semgrep.start_semgrep_ingestion,
     'analysis': cartography.intel.analysis.run,
 })
```

### Comparing `cartography-0.90.0rc2/cartography/util.py` & `cartography-0.91.0/cartography/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/cartography.egg-info/PKG-INFO` & `cartography-0.91.0/cartography.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartography
-Version: 0.90.0rc2
+Version: 0.91.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cartography-0.90.0rc2/cartography.egg-info/SOURCES.txt` & `cartography-0.91.0/cartography.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,16 @@
 cartography/intel/github/users.py
 cartography/intel/github/util.py
 cartography/intel/gsuite/__init__.py
 cartography/intel/gsuite/api.py
 cartography/intel/jamf/__init__.py
 cartography/intel/jamf/computers.py
 cartography/intel/jamf/util.py
+cartography/intel/kandji/__init__.py
+cartography/intel/kandji/devices.py
 cartography/intel/kubernetes/__init__.py
 cartography/intel/kubernetes/namespaces.py
 cartography/intel/kubernetes/pods.py
 cartography/intel/kubernetes/secrets.py
 cartography/intel/kubernetes/services.py
 cartography/intel/kubernetes/util.py
 cartography/intel/lastpass/__init__.py
@@ -326,14 +328,17 @@
 cartography/models/duo/group.py
 cartography/models/duo/phone.py
 cartography/models/duo/token.py
 cartography/models/duo/user.py
 cartography/models/duo/web_authn_credential.py
 cartography/models/github/__init__.py
 cartography/models/github/teams.py
+cartography/models/kandji/__init__.py
+cartography/models/kandji/device.py
+cartography/models/kandji/tenant.py
 cartography/models/lastpass/__init__.py
 cartography/models/lastpass/tenant.py
 cartography/models/lastpass/user.py
 cartography/models/semgrep/__init__.py
 cartography/models/semgrep/deployment.py
 cartography/models/semgrep/findings.py
 cartography/models/semgrep/locations.py
```

### Comparing `cartography-0.90.0rc2/cartography.egg-info/requires.txt` & `cartography-0.91.0/cartography.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/setup.cfg` & `cartography-0.91.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cartography-0.90.0rc2/setup.py` & `cartography-0.91.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = '0.90.0rc2'
+__version__ = '0.91.0'
 
 
 setup(
     name='cartography',
     version=__version__,
     description='Explore assets and their relationships across your technical infrastructure.',
     long_description='file: README.md',
```

