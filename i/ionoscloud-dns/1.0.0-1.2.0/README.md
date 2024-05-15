# Comparing `tmp/ionoscloud-dns-1.0.0.tar.gz` & `tmp/ionoscloud-dns-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionoscloud-dns-1.0.0.tar", last modified: Tue Oct 24 13:01:10 2023, max compression
+gzip compressed data, was "ionoscloud-dns-1.2.0.tar", last modified: Wed May 15 14:31:44 2024, max compression
```

## Comparing `ionoscloud-dns-1.0.0.tar` & `ionoscloud-dns-1.2.0.tar`

### file list

```diff
@@ -1,83 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:01:10.814158 ionoscloud-dns-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-24 13:00:06.000000 ionoscloud-dns-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2023-10-24 13:01:10.814158 ionoscloud-dns-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:01:10.806158 ionoscloud-dns-1.0.0/ionoscloud_dns/
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:01:10.806158 ionoscloud-dns-1.0.0/ionoscloud_dns/api/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20022 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/dnssec_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53302 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    50002 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/secondary_zones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/zone_files_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34570 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api/zones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32633 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16749 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:01:10.814158 ionoscloud-dns-1.0.0/ionoscloud_dns/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_read_list_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/key_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/key_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/ksk_bits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_for_secondary_zone_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_nameservers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_nameservers_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/nsec_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/provisioning_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/quota_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read_list_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_transfer_primary_ip_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_transfer_primary_ips_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/models/zsk_bits.py
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/rest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3518 2023-10-24 13:00:06.000000 ionoscloud-dns-1.0.0/ionoscloud_dns/test-driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:01:10.806158 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2023-10-24 13:01:10.000000 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-10-24 13:01:10.000000 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 13:01:10.000000 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-24 13:01:10.000000 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-24 13:01:10.000000 ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-24 13:01:10.814158 ionoscloud-dns-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-10-24 13:00:32.000000 ionoscloud-dns-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:31:44.318520 ionoscloud-dns-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 14:30:46.000000 ionoscloud-dns-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-15 14:31:44.318520 ionoscloud-dns-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:31:44.294520 ionoscloud-dns-1.2.0/ionoscloud_dns/
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:31:44.298520 ionoscloud-dns-1.2.0/ionoscloud_dns/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20067 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/dnssec_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53126 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35981 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/reverse_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49826 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/secondary_zones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/zone_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34392 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api/zones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32639 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:31:44.318520 ionoscloud-dns-1.2.0/ionoscloud_dns/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_properties_key_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_properties_nsec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/key_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/key_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/ksk_bits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_for_secondary_zone_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_nameservers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_nameservers_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/nsec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/nsec_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/provisioning_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/quota_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_record_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_record_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_records_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read_list_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_transfer_primary_ip_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_transfer_primary_ips_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-15 14:31:09.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/models/zsk_bits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/rest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3518 2024-05-15 14:30:46.000000 ionoscloud-dns-1.2.0/ionoscloud_dns/test-driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:31:44.298520 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-15 14:31:44.000000 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-15 14:31:44.000000 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:31:44.000000 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 14:31:44.000000 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 14:31:44.000000 ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 14:31:44.318520 ionoscloud-dns-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-15 14:31:10.000000 ionoscloud-dns-1.2.0/setup.py
```

### Comparing `ionoscloud-dns-1.0.0/LICENSE` & `ionoscloud-dns-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ionoscloud-dns-1.0.0/PKG-INFO` & `ionoscloud-dns-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: ionoscloud-dns
-Version: 1.0.0
-Summary: Python SDK for the ionoscloud-dns API
-Home-page: https://github.com/ionos-cloud/sdk-python-dns
-Author: Ionos Cloud
-Author-email: sdk@cloud.ionos.com
-Keywords: OpenAPI,OpenAPI-Generator,IONOS Cloud - DNS API
-Classifier: Natural Language :: English
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Internet :: WWW/HTTP
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Gitter](https://img.shields.io/gitter/room/ionos-cloud/sdk-general)](https://gitter.im/ionos-cloud/sdk-general)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=alert_status)](https://sonarcloud.io/summary?id=sdk-python-dns)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=bugs)](https://sonarcloud.io/summary/new_code?id=sdk-python-dns)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=sdk-python-dns)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=sdk-python-dns)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=sdk-python-dns)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=sdk-python-dns&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=sdk-python-dns)
@@ -118,14 +97,22 @@
 
 ### HTTP proxies
 
 You can use http proxies by setting the following environment variables:
 - `IONOS_HTTP_PROXY` - proxy URL
 - `IONOS_HTTP_PROXY_HEADERS` - proxy headers
 
+Each line in `IONOS_HTTP_PROXY_HEADERS` represents one header, where the header name and value is separated by a colon. Newline characters within a value need to be escaped. See this example:
+```
+Connection: Keep-Alive
+User-Info: MyID
+User-Group: my long\nheader value
+```
+
+
 ### Changing the base URL
 
 Base URL for the HTTP operation can be changed in the following way:
 
 ```python
 import os
 
@@ -163,29 +150,34 @@
 | QuotaApi | [**quota_get**](docs/api/QuotaApi.md#quota_get) | **GET** /quota | Retrieve resources quota |
 | RecordsApi | [**records_get**](docs/api/RecordsApi.md#records_get) | **GET** /records | Retrieve all records from primary zones |
 | RecordsApi | [**secondaryzones_records_get**](docs/api/RecordsApi.md#secondaryzones_records_get) | **GET** /secondaryzones/{secondaryZoneId}/records | Retrieve records for a secondary zone |
 | RecordsApi | [**zones_records_delete**](docs/api/RecordsApi.md#zones_records_delete) | **DELETE** /zones/{zoneId}/records/{recordId} | Delete a record |
 | RecordsApi | [**zones_records_find_by_id**](docs/api/RecordsApi.md#zones_records_find_by_id) | **GET** /zones/{zoneId}/records/{recordId} | Retrieve a record |
 | RecordsApi | [**zones_records_get**](docs/api/RecordsApi.md#zones_records_get) | **GET** /zones/{zoneId}/records | Retrieve records |
 | RecordsApi | [**zones_records_post**](docs/api/RecordsApi.md#zones_records_post) | **POST** /zones/{zoneId}/records | Create a record |
-| RecordsApi | [**zones_records_put**](docs/api/RecordsApi.md#zones_records_put) | **PUT** /zones/{zoneId}/records/{recordId} | Ensure a record |
+| RecordsApi | [**zones_records_put**](docs/api/RecordsApi.md#zones_records_put) | **PUT** /zones/{zoneId}/records/{recordId} | Update a record |
+| ReverseRecordsApi | [**reverserecords_delete**](docs/api/ReverseRecordsApi.md#reverserecords_delete) | **DELETE** /reverserecords/{reverserecordId} | Delete a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_find_by_id**](docs/api/ReverseRecordsApi.md#reverserecords_find_by_id) | **GET** /reverserecords/{reverserecordId} | Retrieve a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_get**](docs/api/ReverseRecordsApi.md#reverserecords_get) | **GET** /reverserecords | Retrieves existing reverse DNS records |
+| ReverseRecordsApi | [**reverserecords_post**](docs/api/ReverseRecordsApi.md#reverserecords_post) | **POST** /reverserecords | Create a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_put**](docs/api/ReverseRecordsApi.md#reverserecords_put) | **PUT** /reverserecords/{reverserecordId} | Update a reverse DNS record |
 | SecondaryZonesApi | [**secondaryzones_axfr_get**](docs/api/SecondaryZonesApi.md#secondaryzones_axfr_get) | **GET** /secondaryzones/{secondaryZoneId}/axfr | Get status of zone transfer |
 | SecondaryZonesApi | [**secondaryzones_axfr_put**](docs/api/SecondaryZonesApi.md#secondaryzones_axfr_put) | **PUT** /secondaryzones/{secondaryZoneId}/axfr | Start zone transfer |
 | SecondaryZonesApi | [**secondaryzones_delete**](docs/api/SecondaryZonesApi.md#secondaryzones_delete) | **DELETE** /secondaryzones/{secondaryZoneId} | Delete a secondary zone |
 | SecondaryZonesApi | [**secondaryzones_find_by_id**](docs/api/SecondaryZonesApi.md#secondaryzones_find_by_id) | **GET** /secondaryzones/{secondaryZoneId} | Retrieve a secondary zone |
 | SecondaryZonesApi | [**secondaryzones_get**](docs/api/SecondaryZonesApi.md#secondaryzones_get) | **GET** /secondaryzones | Retrieve secondary zones |
 | SecondaryZonesApi | [**secondaryzones_post**](docs/api/SecondaryZonesApi.md#secondaryzones_post) | **POST** /secondaryzones | Create a secondary zone |
-| SecondaryZonesApi | [**secondaryzones_put**](docs/api/SecondaryZonesApi.md#secondaryzones_put) | **PUT** /secondaryzones/{secondaryZoneId} | Ensure a secondary zone |
+| SecondaryZonesApi | [**secondaryzones_put**](docs/api/SecondaryZonesApi.md#secondaryzones_put) | **PUT** /secondaryzones/{secondaryZoneId} | Update a secondary zone |
 | ZoneFilesApi | [**zones_zonefile_get**](docs/api/ZoneFilesApi.md#zones_zonefile_get) | **GET** /zones/{zoneId}/zonefile | Retrieve a zone file |
 | ZoneFilesApi | [**zones_zonefile_put**](docs/api/ZoneFilesApi.md#zones_zonefile_put) | **PUT** /zones/{zoneId}/zonefile | Updates a zone with a file |
 | ZonesApi | [**zones_delete**](docs/api/ZonesApi.md#zones_delete) | **DELETE** /zones/{zoneId} | Delete a zone |
 | ZonesApi | [**zones_find_by_id**](docs/api/ZonesApi.md#zones_find_by_id) | **GET** /zones/{zoneId} | Retrieve a zone |
 | ZonesApi | [**zones_get**](docs/api/ZonesApi.md#zones_get) | **GET** /zones | Retrieve zones |
 | ZonesApi | [**zones_post**](docs/api/ZonesApi.md#zones_post) | **POST** /zones | Create a zone |
-| ZonesApi | [**zones_put**](docs/api/ZonesApi.md#zones_put) | **PUT** /zones/{zoneId} | Ensure a zone |
+| ZonesApi | [**zones_put**](docs/api/ZonesApi.md#zones_put) | **PUT** /zones/{zoneId} | Update a zone |
 
 </details>
 
 ## Documentation For Models
 
 All URIs are relative to *https://dns.de-fra.ionos.com*
 <details >
@@ -194,37 +186,47 @@
  - [Algorithm](docs/models/Algorithm)
  - [CommonZone](docs/models/CommonZone)
  - [CommonZoneRead](docs/models/CommonZoneRead)
  - [CommonZoneReadList](docs/models/CommonZoneReadList)
  - [DnssecKey](docs/models/DnssecKey)
  - [DnssecKeyCreate](docs/models/DnssecKeyCreate)
  - [DnssecKeyParameters](docs/models/DnssecKeyParameters)
+ - [DnssecKeyReadCreation](docs/models/DnssecKeyReadCreation)
  - [DnssecKeyReadList](docs/models/DnssecKeyReadList)
  - [DnssecKeyReadListMetadata](docs/models/DnssecKeyReadListMetadata)
+ - [DnssecKeyReadListProperties](docs/models/DnssecKeyReadListProperties)
+ - [DnssecKeyReadListPropertiesKeyParameters](docs/models/DnssecKeyReadListPropertiesKeyParameters)
+ - [DnssecKeyReadListPropertiesNsecParameters](docs/models/DnssecKeyReadListPropertiesNsecParameters)
  - [Error](docs/models/Error)
  - [ErrorMessages](docs/models/ErrorMessages)
  - [KeyData](docs/models/KeyData)
  - [KeyParameters](docs/models/KeyParameters)
  - [KskBits](docs/models/KskBits)
  - [Links](docs/models/Links)
  - [Metadata](docs/models/Metadata)
  - [MetadataForSecondaryZoneRecords](docs/models/MetadataForSecondaryZoneRecords)
  - [MetadataWithStateFqdnZoneId](docs/models/MetadataWithStateFqdnZoneId)
  - [MetadataWithStateFqdnZoneIdAllOf](docs/models/MetadataWithStateFqdnZoneIdAllOf)
  - [MetadataWithStateNameservers](docs/models/MetadataWithStateNameservers)
  - [MetadataWithStateNameserversAllOf](docs/models/MetadataWithStateNameserversAllOf)
+ - [NsecMode](docs/models/NsecMode)
  - [NsecParameters](docs/models/NsecParameters)
  - [ProvisioningState](docs/models/ProvisioningState)
  - [Quota](docs/models/Quota)
  - [QuotaDetail](docs/models/QuotaDetail)
  - [Record](docs/models/Record)
  - [RecordCreate](docs/models/RecordCreate)
  - [RecordEnsure](docs/models/RecordEnsure)
  - [RecordRead](docs/models/RecordRead)
  - [RecordReadList](docs/models/RecordReadList)
+ - [ReverseRecord](docs/models/ReverseRecord)
+ - [ReverseRecordCreate](docs/models/ReverseRecordCreate)
+ - [ReverseRecordEnsure](docs/models/ReverseRecordEnsure)
+ - [ReverseRecordRead](docs/models/ReverseRecordRead)
+ - [ReverseRecordsReadList](docs/models/ReverseRecordsReadList)
  - [SecondaryZone](docs/models/SecondaryZone)
  - [SecondaryZoneAllOf](docs/models/SecondaryZoneAllOf)
  - [SecondaryZoneCreate](docs/models/SecondaryZoneCreate)
  - [SecondaryZoneEnsure](docs/models/SecondaryZoneEnsure)
  - [SecondaryZoneRead](docs/models/SecondaryZoneRead)
  - [SecondaryZoneReadAllOf](docs/models/SecondaryZoneReadAllOf)
  - [SecondaryZoneReadList](docs/models/SecondaryZoneReadList)
@@ -243,8 +245,8 @@
  - [ZoneTransferPrimaryIpStatus](docs/models/ZoneTransferPrimaryIpStatus)
  - [ZoneTransferPrimaryIpsStatus](docs/models/ZoneTransferPrimaryIpsStatus)
  - [ZskBits](docs/models/ZskBits)
 
 
 [[Back to API list]](#documentation-for-api-endpoints) [[Back to Model list]](#documentation-for-models)
 
-</details>
+</details>
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/__init__.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # flake8: noqa
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.0"
+__version__ = "1.2.0"
 
 # import apis into sdk package
 from ionoscloud_dns.api.dnssec_api import DNSSECApi
 from ionoscloud_dns.api.quota_api import QuotaApi
 from ionoscloud_dns.api.records_api import RecordsApi
+from ionoscloud_dns.api.reverse_records_api import ReverseRecordsApi
 from ionoscloud_dns.api.secondary_zones_api import SecondaryZonesApi
 from ionoscloud_dns.api.zone_files_api import ZoneFilesApi
 from ionoscloud_dns.api.zones_api import ZonesApi
 
 # import ApiClient
 from ionoscloud_dns.api_response import ApiResponse
 from ionoscloud_dns.api_client import ApiClient
@@ -38,37 +39,47 @@
 from ionoscloud_dns.models.algorithm import Algorithm
 from ionoscloud_dns.models.common_zone import CommonZone
 from ionoscloud_dns.models.common_zone_read import CommonZoneRead
 from ionoscloud_dns.models.common_zone_read_list import CommonZoneReadList
 from ionoscloud_dns.models.dnssec_key import DnssecKey
 from ionoscloud_dns.models.dnssec_key_create import DnssecKeyCreate
 from ionoscloud_dns.models.dnssec_key_parameters import DnssecKeyParameters
+from ionoscloud_dns.models.dnssec_key_read_creation import DnssecKeyReadCreation
 from ionoscloud_dns.models.dnssec_key_read_list import DnssecKeyReadList
 from ionoscloud_dns.models.dnssec_key_read_list_metadata import DnssecKeyReadListMetadata
+from ionoscloud_dns.models.dnssec_key_read_list_properties import DnssecKeyReadListProperties
+from ionoscloud_dns.models.dnssec_key_read_list_properties_key_parameters import DnssecKeyReadListPropertiesKeyParameters
+from ionoscloud_dns.models.dnssec_key_read_list_properties_nsec_parameters import DnssecKeyReadListPropertiesNsecParameters
 from ionoscloud_dns.models.error import Error
 from ionoscloud_dns.models.error_messages import ErrorMessages
 from ionoscloud_dns.models.key_data import KeyData
 from ionoscloud_dns.models.key_parameters import KeyParameters
 from ionoscloud_dns.models.ksk_bits import KskBits
 from ionoscloud_dns.models.links import Links
 from ionoscloud_dns.models.metadata import Metadata
 from ionoscloud_dns.models.metadata_for_secondary_zone_records import MetadataForSecondaryZoneRecords
 from ionoscloud_dns.models.metadata_with_state_fqdn_zone_id import MetadataWithStateFqdnZoneId
 from ionoscloud_dns.models.metadata_with_state_fqdn_zone_id_all_of import MetadataWithStateFqdnZoneIdAllOf
 from ionoscloud_dns.models.metadata_with_state_nameservers import MetadataWithStateNameservers
 from ionoscloud_dns.models.metadata_with_state_nameservers_all_of import MetadataWithStateNameserversAllOf
+from ionoscloud_dns.models.nsec_mode import NsecMode
 from ionoscloud_dns.models.nsec_parameters import NsecParameters
 from ionoscloud_dns.models.provisioning_state import ProvisioningState
 from ionoscloud_dns.models.quota import Quota
 from ionoscloud_dns.models.quota_detail import QuotaDetail
 from ionoscloud_dns.models.record import Record
 from ionoscloud_dns.models.record_create import RecordCreate
 from ionoscloud_dns.models.record_ensure import RecordEnsure
 from ionoscloud_dns.models.record_read import RecordRead
 from ionoscloud_dns.models.record_read_list import RecordReadList
+from ionoscloud_dns.models.reverse_record import ReverseRecord
+from ionoscloud_dns.models.reverse_record_create import ReverseRecordCreate
+from ionoscloud_dns.models.reverse_record_ensure import ReverseRecordEnsure
+from ionoscloud_dns.models.reverse_record_read import ReverseRecordRead
+from ionoscloud_dns.models.reverse_records_read_list import ReverseRecordsReadList
 from ionoscloud_dns.models.secondary_zone import SecondaryZone
 from ionoscloud_dns.models.secondary_zone_all_of import SecondaryZoneAllOf
 from ionoscloud_dns.models.secondary_zone_create import SecondaryZoneCreate
 from ionoscloud_dns.models.secondary_zone_ensure import SecondaryZoneEnsure
 from ionoscloud_dns.models.secondary_zone_read import SecondaryZoneRead
 from ionoscloud_dns.models.secondary_zone_read_all_of import SecondaryZoneReadAllOf
 from ionoscloud_dns.models.secondary_zone_read_list import SecondaryZoneReadList
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/dnssec_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/dnssec_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: DnssecKeyReadCreation
         """
         kwargs['_return_http_data_only'] = True
         return self.zones_keys_post_with_http_info(zone_id, dnssec_key_create, **kwargs)  # noqa: E501
 
     def zones_keys_post_with_http_info(self, zone_id, dnssec_key_create, **kwargs):  # noqa: E501
         """Create a DNSSEC key  # noqa: E501
 
@@ -353,15 +353,15 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(DnssecKeyReadCreation, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'zone_id',
             'dnssec_key_create'
@@ -418,15 +418,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['tokenAuth']  # noqa: E501
 
-        response_type = 'object'
+        response_type = 'DnssecKeyReadCreation'
         if 'response_type' in kwargs:
             response_type = kwargs['response_type']
 
         return self.api_client.call_api(
             '/zones/{zoneId}/keys', 'POST',
             path_params,
             query_params,
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/quota_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/records_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/records_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -923,17 +923,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def zones_records_put(self, zone_id, record_id, record_ensure, **kwargs):  # noqa: E501
-        """Ensure a record  # noqa: E501
+        """Update a record  # noqa: E501
 
-        Ensures that a DNS record with the provided ID is created or modified. In order to successfully update record - all JSON parameters must be passed.  # noqa: E501
+        Updates or creates a DNS record for the provided record ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.zones_records_put(zone_id, record_id, record_ensure, async_req=True)
         >>> result = thread.get()
 
         :param zone_id: The ID (UUID) of the DNS zone. (required)
@@ -957,17 +957,17 @@
                  returns the request thread.
         :rtype: RecordRead
         """
         kwargs['_return_http_data_only'] = True
         return self.zones_records_put_with_http_info(zone_id, record_id, record_ensure, **kwargs)  # noqa: E501
 
     def zones_records_put_with_http_info(self, zone_id, record_id, record_ensure, **kwargs):  # noqa: E501
-        """Ensure a record  # noqa: E501
+        """Update a record  # noqa: E501
 
-        Ensures that a DNS record with the provided ID is created or modified. In order to successfully update record - all JSON parameters must be passed.  # noqa: E501
+        Updates or creates a DNS record for the provided record ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.zones_records_put_with_http_info(zone_id, record_id, record_ensure, async_req=True)
         >>> result = thread.get()
 
         :param zone_id: The ID (UUID) of the DNS zone. (required)
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/secondary_zones_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/secondary_zones_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,17 +863,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def secondaryzones_put(self, secondary_zone_id, secondary_zone_ensure, **kwargs):  # noqa: E501
-        """Ensure a secondary zone  # noqa: E501
+        """Update a secondary zone  # noqa: E501
 
-        Ensures that a secondary zone with the provided ID is created or modified. In order to successfully update secondary zone - all JSON parameters must be passed.  # noqa: E501
+        Updates or creates a secondary zone for the provided secondary Zone ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.secondaryzones_put(secondary_zone_id, secondary_zone_ensure, async_req=True)
         >>> result = thread.get()
 
         :param secondary_zone_id: The ID (UUID) of the DNS zone. (required)
@@ -895,17 +895,17 @@
                  returns the request thread.
         :rtype: SecondaryZoneRead
         """
         kwargs['_return_http_data_only'] = True
         return self.secondaryzones_put_with_http_info(secondary_zone_id, secondary_zone_ensure, **kwargs)  # noqa: E501
 
     def secondaryzones_put_with_http_info(self, secondary_zone_id, secondary_zone_ensure, **kwargs):  # noqa: E501
-        """Ensure a secondary zone  # noqa: E501
+        """Update a secondary zone  # noqa: E501
 
-        Ensures that a secondary zone with the provided ID is created or modified. In order to successfully update secondary zone - all JSON parameters must be passed.  # noqa: E501
+        Updates or creates a secondary zone for the provided secondary Zone ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.secondaryzones_put_with_http_info(secondary_zone_id, secondary_zone_ensure, async_req=True)
         >>> result = thread.get()
 
         :param secondary_zone_id: The ID (UUID) of the DNS zone. (required)
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/zone_files_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/zone_files_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api/zones_api.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api/zones_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,17 +589,17 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def zones_put(self, zone_id, zone_ensure, **kwargs):  # noqa: E501
-        """Ensure a zone  # noqa: E501
+        """Update a zone  # noqa: E501
 
-        Ensures that a zone with the provided ID is created or modified.  In order to successfully update zone - all JSON parameters must be passed.   # noqa: E501
+        Updates or creates a zone for the provided zone ID.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.zones_put(zone_id, zone_ensure, async_req=True)
         >>> result = thread.get()
 
         :param zone_id: The ID (UUID) of the DNS zone. (required)
@@ -621,17 +621,17 @@
                  returns the request thread.
         :rtype: ZoneRead
         """
         kwargs['_return_http_data_only'] = True
         return self.zones_put_with_http_info(zone_id, zone_ensure, **kwargs)  # noqa: E501
 
     def zones_put_with_http_info(self, zone_id, zone_ensure, **kwargs):  # noqa: E501
-        """Ensure a zone  # noqa: E501
+        """Update a zone  # noqa: E501
 
-        Ensures that a zone with the provided ID is created or modified.  In order to successfully update zone - all JSON parameters must be passed.   # noqa: E501
+        Updates or creates a zone for the provided zone ID.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.zones_put_with_http_info(zone_id, zone_ensure, async_req=True)
         >>> result = thread.get()
 
         :param zone_id: The ID (UUID) of the DNS zone. (required)
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api_client.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api_client.py`

 * *Files identical despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -110,15 +110,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'ionos-cloud-sdk-python/1.0.0'
+        self.user_agent = 'ionos-cloud-sdk-python/1.2.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -250,15 +250,15 @@
                             logger.debug('number of maximum retries exceeded {}'.format(config.max_retries))
                         raise response_error
 
                     if backoff_time > config.max_wait_time:
                         backoff_time = config.max_wait_time
 
                     if config.debug:
-                        logger.debug('HTTP response body ~BEGIN~\n#{}\n~END~\n'.format(response.body))
+                        logger.debug('HTTP response body ~BEGIN~\n#{}\n~END~\n'.format(response_error.body))
 
                     time.sleep(backoff_time)
                 except ProtocolError as protocol_error:
                     number_of_calls += 1
                     if number_of_calls >= config.max_retries:
                         if config.debug:
                             logger.debug('number of maximum retries exceeded {}'.format(config.max_retries))
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/api_response.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/api_response.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/configuration.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -200,15 +200,19 @@
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
         self.proxy = os.environ.get('IONOS_HTTP_PROXY')
         """Proxy URL
         """
-        self.proxy_headers = os.environ.get('IONOS_HTTP_PROXY_HEADERS')
+        self.proxy_headers = {}
+        proxy_headers_list = os.environ.get('IONOS_HTTP_PROXY_HEADERS','').splitlines()
+        for header in proxy_headers_list:
+            k,v = header.split(':', 1)
+            self.proxy_headers[k.strip()] = bytes(v.lstrip(), "utf-8").decode("unicode_escape")
         """Proxy headers
         """
         self.safe_chars_for_path_param = '/'
         """Safe chars for path_param
         """
         self.retries = False
         """Adding retries to override urllib3 default value 3
@@ -400,16 +404,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.12.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "Version of the API: 1.15.4\n"\
+               "SDK Package Version: 1.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/exceptions.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/__init__.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,51 +2,61 @@
 
 # flake8: noqa
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 # import models into model package
 from ionoscloud_dns.models.algorithm import Algorithm
 from ionoscloud_dns.models.common_zone import CommonZone
 from ionoscloud_dns.models.common_zone_read import CommonZoneRead
 from ionoscloud_dns.models.common_zone_read_list import CommonZoneReadList
 from ionoscloud_dns.models.dnssec_key import DnssecKey
 from ionoscloud_dns.models.dnssec_key_create import DnssecKeyCreate
 from ionoscloud_dns.models.dnssec_key_parameters import DnssecKeyParameters
+from ionoscloud_dns.models.dnssec_key_read_creation import DnssecKeyReadCreation
 from ionoscloud_dns.models.dnssec_key_read_list import DnssecKeyReadList
 from ionoscloud_dns.models.dnssec_key_read_list_metadata import DnssecKeyReadListMetadata
+from ionoscloud_dns.models.dnssec_key_read_list_properties import DnssecKeyReadListProperties
+from ionoscloud_dns.models.dnssec_key_read_list_properties_key_parameters import DnssecKeyReadListPropertiesKeyParameters
+from ionoscloud_dns.models.dnssec_key_read_list_properties_nsec_parameters import DnssecKeyReadListPropertiesNsecParameters
 from ionoscloud_dns.models.error import Error
 from ionoscloud_dns.models.error_messages import ErrorMessages
 from ionoscloud_dns.models.key_data import KeyData
 from ionoscloud_dns.models.key_parameters import KeyParameters
 from ionoscloud_dns.models.ksk_bits import KskBits
 from ionoscloud_dns.models.links import Links
 from ionoscloud_dns.models.metadata import Metadata
 from ionoscloud_dns.models.metadata_for_secondary_zone_records import MetadataForSecondaryZoneRecords
 from ionoscloud_dns.models.metadata_with_state_fqdn_zone_id import MetadataWithStateFqdnZoneId
 from ionoscloud_dns.models.metadata_with_state_fqdn_zone_id_all_of import MetadataWithStateFqdnZoneIdAllOf
 from ionoscloud_dns.models.metadata_with_state_nameservers import MetadataWithStateNameservers
 from ionoscloud_dns.models.metadata_with_state_nameservers_all_of import MetadataWithStateNameserversAllOf
+from ionoscloud_dns.models.nsec_mode import NsecMode
 from ionoscloud_dns.models.nsec_parameters import NsecParameters
 from ionoscloud_dns.models.provisioning_state import ProvisioningState
 from ionoscloud_dns.models.quota import Quota
 from ionoscloud_dns.models.quota_detail import QuotaDetail
 from ionoscloud_dns.models.record import Record
 from ionoscloud_dns.models.record_create import RecordCreate
 from ionoscloud_dns.models.record_ensure import RecordEnsure
 from ionoscloud_dns.models.record_read import RecordRead
 from ionoscloud_dns.models.record_read_list import RecordReadList
+from ionoscloud_dns.models.reverse_record import ReverseRecord
+from ionoscloud_dns.models.reverse_record_create import ReverseRecordCreate
+from ionoscloud_dns.models.reverse_record_ensure import ReverseRecordEnsure
+from ionoscloud_dns.models.reverse_record_read import ReverseRecordRead
+from ionoscloud_dns.models.reverse_records_read_list import ReverseRecordsReadList
 from ionoscloud_dns.models.secondary_zone import SecondaryZone
 from ionoscloud_dns.models.secondary_zone_all_of import SecondaryZoneAllOf
 from ionoscloud_dns.models.secondary_zone_create import SecondaryZoneCreate
 from ionoscloud_dns.models.secondary_zone_ensure import SecondaryZoneEnsure
 from ionoscloud_dns.models.secondary_zone_read import SecondaryZoneRead
 from ionoscloud_dns.models.secondary_zone_read_all_of import SecondaryZoneReadAllOf
 from ionoscloud_dns.models.secondary_zone_read_list import SecondaryZoneReadList
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/algorithm.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone_read.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/common_zone_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/common_zone_read_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,59 +31,90 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
+        'id': 'str',
+
         'type': 'str',
 
         'href': 'str',
 
         'offset': 'float',
 
         'limit': 'float',
 
         'links': 'Links',
     }
 
     attribute_map = {
 
+        'id': 'id',
+
         'type': 'type',
 
         'href': 'href',
 
         'offset': 'offset',
 
         'limit': 'limit',
 
         'links': '_links',
     }
 
-    def __init__(self, type=None, href=None, offset=None, limit=None, links=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, type=None, href=None, offset=None, limit=None, links=None, local_vars_configuration=None):  # noqa: E501
         """CommonZoneReadList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._type = None
         self._href = None
         self._offset = None
         self._limit = None
         self._links = None
         self.discriminator = None
 
+        self.id = id
         self.type = type
         self.href = href
         self.offset = offset
         self.limit = limit
         self.links = links
 
 
     @property
+    def id(self):
+        """Gets the id of this CommonZoneReadList.  # noqa: E501
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :return: The id of this CommonZoneReadList.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this CommonZoneReadList.
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :param id: The id of this CommonZoneReadList.  # noqa: E501
+        :type id: str
+        """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
+
+    @property
     def type(self):
         """Gets the type of this CommonZoneReadList.  # noqa: E501
 
 
         :return: The type of this CommonZoneReadList.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_create.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_parameters.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_properties.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from ionoscloud_dns.configuration import Configuration
 
 
-class DnssecKeyParameters(object):
+class DnssecKeyReadListProperties(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -31,113 +31,85 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'key_parameters': 'KeyParameters',
+        'key_parameters': 'DnssecKeyReadListPropertiesKeyParameters',
 
-        'nsec_parameters': 'NsecParameters',
-
-        'validity': 'int',
+        'nsec_parameters': 'DnssecKeyReadListPropertiesNsecParameters',
     }
 
     attribute_map = {
 
         'key_parameters': 'keyParameters',
 
         'nsec_parameters': 'nsecParameters',
-
-        'validity': 'validity',
     }
 
-    def __init__(self, key_parameters=None, nsec_parameters=None, validity=90, local_vars_configuration=None):  # noqa: E501
-        """DnssecKeyParameters - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, key_parameters=None, nsec_parameters=None, local_vars_configuration=None):  # noqa: E501
+        """DnssecKeyReadListProperties - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._key_parameters = None
         self._nsec_parameters = None
-        self._validity = None
         self.discriminator = None
 
-        if key_parameters is not None:
-            self.key_parameters = key_parameters
-        if nsec_parameters is not None:
-            self.nsec_parameters = nsec_parameters
-        if validity is not None:
-            self.validity = validity
+        self.key_parameters = key_parameters
+        self.nsec_parameters = nsec_parameters
 
 
     @property
     def key_parameters(self):
-        """Gets the key_parameters of this DnssecKeyParameters.  # noqa: E501
+        """Gets the key_parameters of this DnssecKeyReadListProperties.  # noqa: E501
 
 
-        :return: The key_parameters of this DnssecKeyParameters.  # noqa: E501
-        :rtype: KeyParameters
+        :return: The key_parameters of this DnssecKeyReadListProperties.  # noqa: E501
+        :rtype: DnssecKeyReadListPropertiesKeyParameters
         """
         return self._key_parameters
 
     @key_parameters.setter
     def key_parameters(self, key_parameters):
-        """Sets the key_parameters of this DnssecKeyParameters.
+        """Sets the key_parameters of this DnssecKeyReadListProperties.
 
 
-        :param key_parameters: The key_parameters of this DnssecKeyParameters.  # noqa: E501
-        :type key_parameters: KeyParameters
+        :param key_parameters: The key_parameters of this DnssecKeyReadListProperties.  # noqa: E501
+        :type key_parameters: DnssecKeyReadListPropertiesKeyParameters
         """
+        if self.local_vars_configuration.client_side_validation and key_parameters is None:  # noqa: E501
+            raise ValueError("Invalid value for `key_parameters`, must not be `None`")  # noqa: E501
 
         self._key_parameters = key_parameters
 
     @property
     def nsec_parameters(self):
-        """Gets the nsec_parameters of this DnssecKeyParameters.  # noqa: E501
+        """Gets the nsec_parameters of this DnssecKeyReadListProperties.  # noqa: E501
 
 
-        :return: The nsec_parameters of this DnssecKeyParameters.  # noqa: E501
-        :rtype: NsecParameters
+        :return: The nsec_parameters of this DnssecKeyReadListProperties.  # noqa: E501
+        :rtype: DnssecKeyReadListPropertiesNsecParameters
         """
         return self._nsec_parameters
 
     @nsec_parameters.setter
     def nsec_parameters(self, nsec_parameters):
-        """Sets the nsec_parameters of this DnssecKeyParameters.
+        """Sets the nsec_parameters of this DnssecKeyReadListProperties.
 
 
-        :param nsec_parameters: The nsec_parameters of this DnssecKeyParameters.  # noqa: E501
-        :type nsec_parameters: NsecParameters
+        :param nsec_parameters: The nsec_parameters of this DnssecKeyReadListProperties.  # noqa: E501
+        :type nsec_parameters: DnssecKeyReadListPropertiesNsecParameters
         """
+        if self.local_vars_configuration.client_side_validation and nsec_parameters is None:  # noqa: E501
+            raise ValueError("Invalid value for `nsec_parameters`, must not be `None`")  # noqa: E501
 
         self._nsec_parameters = nsec_parameters
-
-    @property
-    def validity(self):
-        """Gets the validity of this DnssecKeyParameters.  # noqa: E501
-
-        Signature validity in days. (between 90 and 365)   # noqa: E501
-
-        :return: The validity of this DnssecKeyParameters.  # noqa: E501
-        :rtype: int
-        """
-        return self._validity
-
-    @validity.setter
-    def validity(self, validity):
-        """Sets the validity of this DnssecKeyParameters.
-
-        Signature validity in days. (between 90 and 365)   # noqa: E501
-
-        :param validity: The validity of this DnssecKeyParameters.  # noqa: E501
-        :type validity: int
-        """
-
-        self._validity = validity
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -164,18 +136,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DnssecKeyParameters):
+        if not isinstance(other, DnssecKeyReadListProperties):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DnssecKeyParameters):
+        if not isinstance(other, DnssecKeyReadListProperties):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -38,47 +38,54 @@
         'id': 'str',
 
         'type': 'str',
 
         'href': 'str',
 
         'metadata': 'DnssecKeyReadListMetadata',
+
+        'properties': 'DnssecKeyReadListProperties',
     }
 
     attribute_map = {
 
         'id': 'id',
 
         'type': 'type',
 
         'href': 'href',
 
         'metadata': 'metadata',
+
+        'properties': 'properties',
     }
 
-    def __init__(self, id=None, type=None, href=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, type=None, href=None, metadata=None, properties=None, local_vars_configuration=None):  # noqa: E501
         """DnssecKeyReadList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._type = None
         self._href = None
         self._metadata = None
+        self._properties = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         if type is not None:
             self.type = type
         if href is not None:
             self.href = href
         if metadata is not None:
             self.metadata = metadata
+        if properties is not None:
+            self.properties = properties
 
 
     @property
     def id(self):
         """Gets the id of this DnssecKeyReadList.  # noqa: E501
 
 
@@ -162,14 +169,35 @@
 
 
         :param metadata: The metadata of this DnssecKeyReadList.  # noqa: E501
         :type metadata: DnssecKeyReadListMetadata
         """
 
         self._metadata = metadata
+
+    @property
+    def properties(self):
+        """Gets the properties of this DnssecKeyReadList.  # noqa: E501
+
+
+        :return: The properties of this DnssecKeyReadList.  # noqa: E501
+        :rtype: DnssecKeyReadListProperties
+        """
+        return self._properties
+
+    @properties.setter
+    def properties(self, properties):
+        """Sets the properties of this DnssecKeyReadList.
+
+
+        :param properties: The properties of this DnssecKeyReadList.  # noqa: E501
+        :type properties: DnssecKeyReadListProperties
+        """
+
+        self._properties = properties
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/dnssec_key_read_list_metadata.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/dnssec_key_read_list_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/error.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/error_messages.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/error_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/key_data.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from ionoscloud_dns.configuration import Configuration
 
 
-class KeyData(object):
+class Zone(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -31,147 +31,118 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'flags': 'int',
+        'zone_name': 'str',
 
-        'protocol': 'int',
+        'description': 'str',
 
-        'alg': 'int',
-
-        'pub_key': 'str',
+        'enabled': 'bool',
     }
 
     attribute_map = {
 
-        'flags': 'flags',
-
-        'protocol': 'protocol',
+        'zone_name': 'zoneName',
 
-        'alg': 'alg',
+        'description': 'description',
 
-        'pub_key': 'pubKey',
+        'enabled': 'enabled',
     }
 
-    def __init__(self, flags=None, protocol=None, alg=None, pub_key=None, local_vars_configuration=None):  # noqa: E501
-        """KeyData - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, zone_name=None, description=None, enabled=True, local_vars_configuration=None):  # noqa: E501
+        """Zone - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._flags = None
-        self._protocol = None
-        self._alg = None
-        self._pub_key = None
+        self._zone_name = None
+        self._description = None
+        self._enabled = None
         self.discriminator = None
 
-        if flags is not None:
-            self.flags = flags
-        if protocol is not None:
-            self.protocol = protocol
-        if alg is not None:
-            self.alg = alg
-        if pub_key is not None:
-            self.pub_key = pub_key
+        self.zone_name = zone_name
+        if description is not None:
+            self.description = description
+        if enabled is not None:
+            self.enabled = enabled
 
 
     @property
-    def flags(self):
-        """Gets the flags of this KeyData.  # noqa: E501
-
-        Represents the key's metadata and usage information.  # noqa: E501
-
-        :return: The flags of this KeyData.  # noqa: E501
-        :rtype: int
-        """
-        return self._flags
-
-    @flags.setter
-    def flags(self, flags):
-        """Sets the flags of this KeyData.
+    def zone_name(self):
+        """Gets the zone_name of this Zone.  # noqa: E501
 
-        Represents the key's metadata and usage information.  # noqa: E501
-
-        :param flags: The flags of this KeyData.  # noqa: E501
-        :type flags: int
-        """
+        The zone name  # noqa: E501
 
-        self._flags = flags
-
-    @property
-    def protocol(self):
-        """Gets the protocol of this KeyData.  # noqa: E501
-
-        Represents the protocol associated with the key (3 represents DNSSEC).  # noqa: E501
-
-        :return: The protocol of this KeyData.  # noqa: E501
-        :rtype: int
+        :return: The zone_name of this Zone.  # noqa: E501
+        :rtype: str
         """
-        return self._protocol
+        return self._zone_name
 
-    @protocol.setter
-    def protocol(self, protocol):
-        """Sets the protocol of this KeyData.
+    @zone_name.setter
+    def zone_name(self, zone_name):
+        """Sets the zone_name of this Zone.
 
-        Represents the protocol associated with the key (3 represents DNSSEC).  # noqa: E501
+        The zone name  # noqa: E501
 
-        :param protocol: The protocol of this KeyData.  # noqa: E501
-        :type protocol: int
+        :param zone_name: The zone_name of this Zone.  # noqa: E501
+        :type zone_name: str
         """
+        if self.local_vars_configuration.client_side_validation and zone_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `zone_name`, must not be `None`")  # noqa: E501
 
-        self._protocol = protocol
+        self._zone_name = zone_name
 
     @property
-    def alg(self):
-        """Gets the alg of this KeyData.  # noqa: E501
+    def description(self):
+        """Gets the description of this Zone.  # noqa: E501
 
-        Represents the signing algorithm.  # noqa: E501
+        The hosted zone is used for...  # noqa: E501
 
-        :return: The alg of this KeyData.  # noqa: E501
-        :rtype: int
+        :return: The description of this Zone.  # noqa: E501
+        :rtype: str
         """
-        return self._alg
+        return self._description
 
-    @alg.setter
-    def alg(self, alg):
-        """Sets the alg of this KeyData.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Zone.
 
-        Represents the signing algorithm.  # noqa: E501
+        The hosted zone is used for...  # noqa: E501
 
-        :param alg: The alg of this KeyData.  # noqa: E501
-        :type alg: int
+        :param description: The description of this Zone.  # noqa: E501
+        :type description: str
         """
 
-        self._alg = alg
+        self._description = description
 
     @property
-    def pub_key(self):
-        """Gets the pub_key of this KeyData.  # noqa: E501
+    def enabled(self):
+        """Gets the enabled of this Zone.  # noqa: E501
 
-        Represents the public key data in Base64 encoding.  # noqa: E501
+        Users can activate and deactivate zones.  # noqa: E501
 
-        :return: The pub_key of this KeyData.  # noqa: E501
-        :rtype: str
+        :return: The enabled of this Zone.  # noqa: E501
+        :rtype: bool
         """
-        return self._pub_key
+        return self._enabled
 
-    @pub_key.setter
-    def pub_key(self, pub_key):
-        """Sets the pub_key of this KeyData.
+    @enabled.setter
+    def enabled(self, enabled):
+        """Sets the enabled of this Zone.
 
-        Represents the public key data in Base64 encoding.  # noqa: E501
+        Users can activate and deactivate zones.  # noqa: E501
 
-        :param pub_key: The pub_key of this KeyData.  # noqa: E501
-        :type pub_key: str
+        :param enabled: The enabled of this Zone.  # noqa: E501
+        :type enabled: bool
         """
 
-        self._pub_key = pub_key
+        self._enabled = enabled
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -198,18 +169,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, KeyData):
+        if not isinstance(other, Zone):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, KeyData):
+        if not isinstance(other, Zone):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/key_parameters.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/key_parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -58,20 +58,17 @@
         self.local_vars_configuration = local_vars_configuration
 
         self._algorithm = None
         self._ksk_bits = None
         self._zsk_bits = None
         self.discriminator = None
 
-        if algorithm is not None:
-            self.algorithm = algorithm
-        if ksk_bits is not None:
-            self.ksk_bits = ksk_bits
-        if zsk_bits is not None:
-            self.zsk_bits = zsk_bits
+        self.algorithm = algorithm
+        self.ksk_bits = ksk_bits
+        self.zsk_bits = zsk_bits
 
 
     @property
     def algorithm(self):
         """Gets the algorithm of this KeyParameters.  # noqa: E501
 
 
@@ -84,14 +81,16 @@
     def algorithm(self, algorithm):
         """Sets the algorithm of this KeyParameters.
 
 
         :param algorithm: The algorithm of this KeyParameters.  # noqa: E501
         :type algorithm: Algorithm
         """
+        if self.local_vars_configuration.client_side_validation and algorithm is None:  # noqa: E501
+            raise ValueError("Invalid value for `algorithm`, must not be `None`")  # noqa: E501
 
         self._algorithm = algorithm
 
     @property
     def ksk_bits(self):
         """Gets the ksk_bits of this KeyParameters.  # noqa: E501
 
@@ -105,14 +104,16 @@
     def ksk_bits(self, ksk_bits):
         """Sets the ksk_bits of this KeyParameters.
 
 
         :param ksk_bits: The ksk_bits of this KeyParameters.  # noqa: E501
         :type ksk_bits: KskBits
         """
+        if self.local_vars_configuration.client_side_validation and ksk_bits is None:  # noqa: E501
+            raise ValueError("Invalid value for `ksk_bits`, must not be `None`")  # noqa: E501
 
         self._ksk_bits = ksk_bits
 
     @property
     def zsk_bits(self):
         """Gets the zsk_bits of this KeyParameters.  # noqa: E501
 
@@ -126,14 +127,16 @@
     def zsk_bits(self, zsk_bits):
         """Sets the zsk_bits of this KeyParameters.
 
 
         :param zsk_bits: The zsk_bits of this KeyParameters.  # noqa: E501
         :type zsk_bits: ZskBits
         """
+        if self.local_vars_configuration.client_side_validation and zsk_bits is None:  # noqa: E501
+            raise ValueError("Invalid value for `zsk_bits`, must not be `None`")  # noqa: E501
 
         self._zsk_bits = zsk_bits
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/ksk_bits.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/ksk_bits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/links.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_for_secondary_zone_records.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_for_secondary_zone_records.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -59,16 +59,15 @@
 
         self._fqdn = None
         self._zone_id = None
         self._root_name = None
         self.discriminator = None
 
         self.fqdn = fqdn
-        if zone_id is not None:
-            self.zone_id = zone_id
+        self.zone_id = zone_id
         self.root_name = root_name
 
 
     @property
     def fqdn(self):
         """Gets the fqdn of this MetadataForSecondaryZoneRecords.  # noqa: E501
 
@@ -109,14 +108,16 @@
         """Sets the zone_id of this MetadataForSecondaryZoneRecords.
 
         The ID (UUID) of the DNS zone of which record belongs to.  # noqa: E501
 
         :param zone_id: The zone_id of this MetadataForSecondaryZoneRecords.  # noqa: E501
         :type zone_id: str
         """
+        if self.local_vars_configuration.client_side_validation and zone_id is None:  # noqa: E501
+            raise ValueError("Invalid value for `zone_id`, must not be `None`")  # noqa: E501
 
         self._zone_id = zone_id
 
     @property
     def root_name(self):
         """Gets the root_name of this MetadataForSecondaryZoneRecords.  # noqa: E501
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_fqdn_zone_id_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_nameservers.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_nameservers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/metadata_with_state_nameservers_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/metadata_with_state_nameservers_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/nsec_parameters.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/nsec_parameters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,15 +31,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'nsec_mode': 'str',
+        'nsec_mode': 'NsecMode',
 
         'nsec3_iterations': 'int',
 
         'nsec3_salt_bits': 'int',
     }
 
     attribute_map = {
@@ -47,59 +47,50 @@
         'nsec_mode': 'nsecMode',
 
         'nsec3_iterations': 'nsec3Iterations',
 
         'nsec3_salt_bits': 'nsec3SaltBits',
     }
 
-    def __init__(self, nsec_mode='NSEC3', nsec3_iterations=21, nsec3_salt_bits=128, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, nsec_mode=None, nsec3_iterations=None, nsec3_salt_bits=None, local_vars_configuration=None):  # noqa: E501
         """NsecParameters - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._nsec_mode = None
         self._nsec3_iterations = None
         self._nsec3_salt_bits = None
         self.discriminator = None
 
-        if nsec_mode is not None:
-            self.nsec_mode = nsec_mode
-        if nsec3_iterations is not None:
-            self.nsec3_iterations = nsec3_iterations
-        if nsec3_salt_bits is not None:
-            self.nsec3_salt_bits = nsec3_salt_bits
+        self.nsec_mode = nsec_mode
+        self.nsec3_iterations = nsec3_iterations
+        self.nsec3_salt_bits = nsec3_salt_bits
 
 
     @property
     def nsec_mode(self):
         """Gets the nsec_mode of this NsecParameters.  # noqa: E501
 
-        NSEC mode.   # noqa: E501
 
         :return: The nsec_mode of this NsecParameters.  # noqa: E501
-        :rtype: str
+        :rtype: NsecMode
         """
         return self._nsec_mode
 
     @nsec_mode.setter
     def nsec_mode(self, nsec_mode):
         """Sets the nsec_mode of this NsecParameters.
 
-        NSEC mode.   # noqa: E501
 
         :param nsec_mode: The nsec_mode of this NsecParameters.  # noqa: E501
-        :type nsec_mode: str
+        :type nsec_mode: NsecMode
         """
-        allowed_values = ["NSEC", "NSEC3"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and nsec_mode not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `nsec_mode` ({0}), must be one of {1}"  # noqa: E501
-                .format(nsec_mode, allowed_values)
-            )
+        if self.local_vars_configuration.client_side_validation and nsec_mode is None:  # noqa: E501
+            raise ValueError("Invalid value for `nsec_mode`, must not be `None`")  # noqa: E501
 
         self._nsec_mode = nsec_mode
 
     @property
     def nsec3_iterations(self):
         """Gets the nsec3_iterations of this NsecParameters.  # noqa: E501
 
@@ -115,14 +106,22 @@
         """Sets the nsec3_iterations of this NsecParameters.
 
         Number of iterations for NSEC3. (between 0 and 50)   # noqa: E501
 
         :param nsec3_iterations: The nsec3_iterations of this NsecParameters.  # noqa: E501
         :type nsec3_iterations: int
         """
+        if self.local_vars_configuration.client_side_validation and nsec3_iterations is None:  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_iterations`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                nsec3_iterations is not None and nsec3_iterations > 50):  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_iterations`, must be a value less than or equal to `50`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                nsec3_iterations is not None and nsec3_iterations < 0):  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_iterations`, must be a value greater than or equal to `0`")  # noqa: E501
 
         self._nsec3_iterations = nsec3_iterations
 
     @property
     def nsec3_salt_bits(self):
         """Gets the nsec3_salt_bits of this NsecParameters.  # noqa: E501
 
@@ -138,14 +137,22 @@
         """Sets the nsec3_salt_bits of this NsecParameters.
 
         Salt length in bits for NSEC3. (between 64 and 128, multiples of 8)   # noqa: E501
 
         :param nsec3_salt_bits: The nsec3_salt_bits of this NsecParameters.  # noqa: E501
         :type nsec3_salt_bits: int
         """
+        if self.local_vars_configuration.client_side_validation and nsec3_salt_bits is None:  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_salt_bits`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                nsec3_salt_bits is not None and nsec3_salt_bits > 128):  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_salt_bits`, must be a value less than or equal to `128`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                nsec3_salt_bits is not None and nsec3_salt_bits < 64):  # noqa: E501
+            raise ValueError("Invalid value for `nsec3_salt_bits`, must be a value greater than or equal to `64`")  # noqa: E501
 
         self._nsec3_salt_bits = nsec3_salt_bits
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/provisioning_state.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/provisioning_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/quota.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/quota_detail.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/quota_detail.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -36,39 +36,45 @@
     openapi_types = {
 
         'zones': 'int',
 
         'secondary_zones': 'int',
 
         'records': 'int',
+
+        'reverse_records': 'int',
     }
 
     attribute_map = {
 
         'zones': 'zones',
 
         'secondary_zones': 'secondaryZones',
 
         'records': 'records',
+
+        'reverse_records': 'reverseRecords',
     }
 
-    def __init__(self, zones=500, secondary_zones=500, records=5000, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, zones=0, secondary_zones=0, records=0, reverse_records=0, local_vars_configuration=None):  # noqa: E501
         """QuotaDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._zones = None
         self._secondary_zones = None
         self._records = None
+        self._reverse_records = None
         self.discriminator = None
 
         self.zones = zones
         self.secondary_zones = secondary_zones
         self.records = records
+        self.reverse_records = reverse_records
 
 
     @property
     def zones(self):
         """Gets the zones of this QuotaDetail.  # noqa: E501
 
         count of the number of zones  # noqa: E501
@@ -137,14 +143,39 @@
         :param records: The records of this QuotaDetail.  # noqa: E501
         :type records: int
         """
         if self.local_vars_configuration.client_side_validation and records is None:  # noqa: E501
             raise ValueError("Invalid value for `records`, must not be `None`")  # noqa: E501
 
         self._records = records
+
+    @property
+    def reverse_records(self):
+        """Gets the reverse_records of this QuotaDetail.  # noqa: E501
+
+        count of the number of reverse DNS records  # noqa: E501
+
+        :return: The reverse_records of this QuotaDetail.  # noqa: E501
+        :rtype: int
+        """
+        return self._reverse_records
+
+    @reverse_records.setter
+    def reverse_records(self, reverse_records):
+        """Sets the reverse_records of this QuotaDetail.
+
+        count of the number of reverse DNS records  # noqa: E501
+
+        :param reverse_records: The reverse_records of this QuotaDetail.  # noqa: E501
+        :type reverse_records: int
+        """
+        if self.local_vars_configuration.client_side_validation and reverse_records is None:  # noqa: E501
+            raise ValueError("Invalid value for `reverse_records`, must not be `None`")  # noqa: E501
+
+        self._reverse_records = reverse_records
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/record.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_create.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_ensure.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_ensure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_read.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/record_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/record_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_create.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_ensure.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_ensure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,14 +31,16 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
+        'id': 'str',
+
         'type': 'str',
 
         'href': 'str',
 
         'offset': 'float',
 
         'limit': 'float',
@@ -46,50 +48,79 @@
         'links': 'Links',
 
         'items': 'list[SecondaryZoneRead]',
     }
 
     attribute_map = {
 
+        'id': 'id',
+
         'type': 'type',
 
         'href': 'href',
 
         'offset': 'offset',
 
         'limit': 'limit',
 
         'links': '_links',
 
         'items': 'items',
     }
 
-    def __init__(self, type=None, href=None, offset=None, limit=None, links=None, items=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, type=None, href=None, offset=None, limit=None, links=None, items=None, local_vars_configuration=None):  # noqa: E501
         """SecondaryZoneReadList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._type = None
         self._href = None
         self._offset = None
         self._limit = None
         self._links = None
         self._items = None
         self.discriminator = None
 
+        self.id = id
         self.type = type
         self.href = href
         self.offset = offset
         self.limit = limit
         self.links = links
         self.items = items
 
 
     @property
+    def id(self):
+        """Gets the id of this SecondaryZoneReadList.  # noqa: E501
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :return: The id of this SecondaryZoneReadList.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this SecondaryZoneReadList.
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :param id: The id of this SecondaryZoneReadList.  # noqa: E501
+        :type id: str
+        """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
+
+    @property
     def type(self):
         """Gets the type of this SecondaryZoneReadList.  # noqa: E501
 
 
         :return: The type of this SecondaryZoneReadList.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_read_list_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_read_list_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/secondary_zone_record_read_list_metadata.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/secondary_zone_record_read_list_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/reverse_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from ionoscloud_dns.configuration import Configuration
 
 
-class Zone(object):
+class ReverseRecord(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -31,118 +31,119 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'zone_name': 'str',
+        'name': 'str',
 
         'description': 'str',
 
-        'enabled': 'bool',
+        'ip': 'str',
     }
 
     attribute_map = {
 
-        'zone_name': 'zoneName',
+        'name': 'name',
 
         'description': 'description',
 
-        'enabled': 'enabled',
+        'ip': 'ip',
     }
 
-    def __init__(self, zone_name=None, description=None, enabled=True, local_vars_configuration=None):  # noqa: E501
-        """Zone - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name=None, description=None, ip=None, local_vars_configuration=None):  # noqa: E501
+        """ReverseRecord - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._zone_name = None
+        self._name = None
         self._description = None
-        self._enabled = None
+        self._ip = None
         self.discriminator = None
 
-        self.zone_name = zone_name
+        self.name = name
         if description is not None:
             self.description = description
-        if enabled is not None:
-            self.enabled = enabled
+        self.ip = ip
 
 
     @property
-    def zone_name(self):
-        """Gets the zone_name of this Zone.  # noqa: E501
+    def name(self):
+        """Gets the name of this ReverseRecord.  # noqa: E501
 
-        The zone name  # noqa: E501
+        The reverse DNS record name  # noqa: E501
 
-        :return: The zone_name of this Zone.  # noqa: E501
+        :return: The name of this ReverseRecord.  # noqa: E501
         :rtype: str
         """
-        return self._zone_name
+        return self._name
 
-    @zone_name.setter
-    def zone_name(self, zone_name):
-        """Sets the zone_name of this Zone.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ReverseRecord.
 
-        The zone name  # noqa: E501
+        The reverse DNS record name  # noqa: E501
 
-        :param zone_name: The zone_name of this Zone.  # noqa: E501
-        :type zone_name: str
+        :param name: The name of this ReverseRecord.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and zone_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `zone_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._zone_name = zone_name
+        self._name = name
 
     @property
     def description(self):
-        """Gets the description of this Zone.  # noqa: E501
+        """Gets the description of this ReverseRecord.  # noqa: E501
 
-        The hosted zone is used for...  # noqa: E501
+        Description stored along with the reverse DNS record to describe its usage.  # noqa: E501
 
-        :return: The description of this Zone.  # noqa: E501
+        :return: The description of this ReverseRecord.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this Zone.
+        """Sets the description of this ReverseRecord.
 
-        The hosted zone is used for...  # noqa: E501
+        Description stored along with the reverse DNS record to describe its usage.  # noqa: E501
 
-        :param description: The description of this Zone.  # noqa: E501
+        :param description: The description of this ReverseRecord.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
-    def enabled(self):
-        """Gets the enabled of this Zone.  # noqa: E501
+    def ip(self):
+        """Gets the ip of this ReverseRecord.  # noqa: E501
 
-        Users can activate and deactivate zones.  # noqa: E501
+        Specifies for which IP address the reverse record should be created. The IP addresses needs to be owned by the contract. Accepts IPv4 and IPv6 addresses.  # noqa: E501
 
-        :return: The enabled of this Zone.  # noqa: E501
-        :rtype: bool
+        :return: The ip of this ReverseRecord.  # noqa: E501
+        :rtype: str
         """
-        return self._enabled
+        return self._ip
 
-    @enabled.setter
-    def enabled(self, enabled):
-        """Sets the enabled of this Zone.
+    @ip.setter
+    def ip(self, ip):
+        """Sets the ip of this ReverseRecord.
 
-        Users can activate and deactivate zones.  # noqa: E501
+        Specifies for which IP address the reverse record should be created. The IP addresses needs to be owned by the contract. Accepts IPv4 and IPv6 addresses.  # noqa: E501
 
-        :param enabled: The enabled of this Zone.  # noqa: E501
-        :type enabled: bool
+        :param ip: The ip of this ReverseRecord.  # noqa: E501
+        :type ip: str
         """
+        if self.local_vars_configuration.client_side_validation and ip is None:  # noqa: E501
+            raise ValueError("Invalid value for `ip`, must not be `None`")  # noqa: E501
 
-        self._enabled = enabled
+        self._ip = ip
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -169,18 +170,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Zone):
+        if not isinstance(other, ReverseRecord):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Zone):
+        if not isinstance(other, ReverseRecord):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_create.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_ensure.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_ensure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_list.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,14 +31,16 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
+        'id': 'str',
+
         'type': 'str',
 
         'href': 'str',
 
         'offset': 'float',
 
         'limit': 'float',
@@ -46,50 +48,79 @@
         'links': 'Links',
 
         'items': 'list[ZoneRead]',
     }
 
     attribute_map = {
 
+        'id': 'id',
+
         'type': 'type',
 
         'href': 'href',
 
         'offset': 'offset',
 
         'limit': 'limit',
 
         'links': '_links',
 
         'items': 'items',
     }
 
-    def __init__(self, type=None, href=None, offset=None, limit=None, links=None, items=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, type=None, href=None, offset=None, limit=None, links=None, items=None, local_vars_configuration=None):  # noqa: E501
         """ZoneReadList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._type = None
         self._href = None
         self._offset = None
         self._limit = None
         self._links = None
         self._items = None
         self.discriminator = None
 
+        self.id = id
         self.type = type
         self.href = href
         self.offset = offset
         self.limit = limit
         self.links = links
         self.items = items
 
 
     @property
+    def id(self):
+        """Gets the id of this ZoneReadList.  # noqa: E501
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :return: The id of this ZoneReadList.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this ZoneReadList.
+
+        ID (UUID) created to identify this action.  # noqa: E501
+
+        :param id: The id of this ZoneReadList.  # noqa: E501
+        :type id: str
+        """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
+
+    @property
     def type(self):
         """Gets the type of this ZoneReadList.  # noqa: E501
 
 
         :return: The type of this ZoneReadList.  # noqa: E501
         :rtype: str
         """
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_read_list_all_of.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_read_list_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_transfer_primary_ip_status.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_transfer_primary_ip_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zone_transfer_primary_ips_status.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zone_transfer_primary_ips_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/models/zsk_bits.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/models/zsk_bits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/rest.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns/test-driver.py` & `ionoscloud-dns-1.2.0/ionoscloud_dns/test-driver.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/PKG-INFO` & `ionoscloud-dns-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionoscloud-dns
-Version: 1.0.0
+Version: 1.2.0
 Summary: Python SDK for the ionoscloud-dns API
 Home-page: https://github.com/ionos-cloud/sdk-python-dns
 Author: Ionos Cloud
 Author-email: sdk@cloud.ionos.com
 Keywords: OpenAPI,OpenAPI-Generator,IONOS Cloud - DNS API
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
@@ -118,14 +118,22 @@
 
 ### HTTP proxies
 
 You can use http proxies by setting the following environment variables:
 - `IONOS_HTTP_PROXY` - proxy URL
 - `IONOS_HTTP_PROXY_HEADERS` - proxy headers
 
+Each line in `IONOS_HTTP_PROXY_HEADERS` represents one header, where the header name and value is separated by a colon. Newline characters within a value need to be escaped. See this example:
+```
+Connection: Keep-Alive
+User-Info: MyID
+User-Group: my long\nheader value
+```
+
+
 ### Changing the base URL
 
 Base URL for the HTTP operation can be changed in the following way:
 
 ```python
 import os
 
@@ -163,29 +171,34 @@
 | QuotaApi | [**quota_get**](docs/api/QuotaApi.md#quota_get) | **GET** /quota | Retrieve resources quota |
 | RecordsApi | [**records_get**](docs/api/RecordsApi.md#records_get) | **GET** /records | Retrieve all records from primary zones |
 | RecordsApi | [**secondaryzones_records_get**](docs/api/RecordsApi.md#secondaryzones_records_get) | **GET** /secondaryzones/{secondaryZoneId}/records | Retrieve records for a secondary zone |
 | RecordsApi | [**zones_records_delete**](docs/api/RecordsApi.md#zones_records_delete) | **DELETE** /zones/{zoneId}/records/{recordId} | Delete a record |
 | RecordsApi | [**zones_records_find_by_id**](docs/api/RecordsApi.md#zones_records_find_by_id) | **GET** /zones/{zoneId}/records/{recordId} | Retrieve a record |
 | RecordsApi | [**zones_records_get**](docs/api/RecordsApi.md#zones_records_get) | **GET** /zones/{zoneId}/records | Retrieve records |
 | RecordsApi | [**zones_records_post**](docs/api/RecordsApi.md#zones_records_post) | **POST** /zones/{zoneId}/records | Create a record |
-| RecordsApi | [**zones_records_put**](docs/api/RecordsApi.md#zones_records_put) | **PUT** /zones/{zoneId}/records/{recordId} | Ensure a record |
+| RecordsApi | [**zones_records_put**](docs/api/RecordsApi.md#zones_records_put) | **PUT** /zones/{zoneId}/records/{recordId} | Update a record |
+| ReverseRecordsApi | [**reverserecords_delete**](docs/api/ReverseRecordsApi.md#reverserecords_delete) | **DELETE** /reverserecords/{reverserecordId} | Delete a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_find_by_id**](docs/api/ReverseRecordsApi.md#reverserecords_find_by_id) | **GET** /reverserecords/{reverserecordId} | Retrieve a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_get**](docs/api/ReverseRecordsApi.md#reverserecords_get) | **GET** /reverserecords | Retrieves existing reverse DNS records |
+| ReverseRecordsApi | [**reverserecords_post**](docs/api/ReverseRecordsApi.md#reverserecords_post) | **POST** /reverserecords | Create a reverse DNS record |
+| ReverseRecordsApi | [**reverserecords_put**](docs/api/ReverseRecordsApi.md#reverserecords_put) | **PUT** /reverserecords/{reverserecordId} | Update a reverse DNS record |
 | SecondaryZonesApi | [**secondaryzones_axfr_get**](docs/api/SecondaryZonesApi.md#secondaryzones_axfr_get) | **GET** /secondaryzones/{secondaryZoneId}/axfr | Get status of zone transfer |
 | SecondaryZonesApi | [**secondaryzones_axfr_put**](docs/api/SecondaryZonesApi.md#secondaryzones_axfr_put) | **PUT** /secondaryzones/{secondaryZoneId}/axfr | Start zone transfer |
 | SecondaryZonesApi | [**secondaryzones_delete**](docs/api/SecondaryZonesApi.md#secondaryzones_delete) | **DELETE** /secondaryzones/{secondaryZoneId} | Delete a secondary zone |
 | SecondaryZonesApi | [**secondaryzones_find_by_id**](docs/api/SecondaryZonesApi.md#secondaryzones_find_by_id) | **GET** /secondaryzones/{secondaryZoneId} | Retrieve a secondary zone |
 | SecondaryZonesApi | [**secondaryzones_get**](docs/api/SecondaryZonesApi.md#secondaryzones_get) | **GET** /secondaryzones | Retrieve secondary zones |
 | SecondaryZonesApi | [**secondaryzones_post**](docs/api/SecondaryZonesApi.md#secondaryzones_post) | **POST** /secondaryzones | Create a secondary zone |
-| SecondaryZonesApi | [**secondaryzones_put**](docs/api/SecondaryZonesApi.md#secondaryzones_put) | **PUT** /secondaryzones/{secondaryZoneId} | Ensure a secondary zone |
+| SecondaryZonesApi | [**secondaryzones_put**](docs/api/SecondaryZonesApi.md#secondaryzones_put) | **PUT** /secondaryzones/{secondaryZoneId} | Update a secondary zone |
 | ZoneFilesApi | [**zones_zonefile_get**](docs/api/ZoneFilesApi.md#zones_zonefile_get) | **GET** /zones/{zoneId}/zonefile | Retrieve a zone file |
 | ZoneFilesApi | [**zones_zonefile_put**](docs/api/ZoneFilesApi.md#zones_zonefile_put) | **PUT** /zones/{zoneId}/zonefile | Updates a zone with a file |
 | ZonesApi | [**zones_delete**](docs/api/ZonesApi.md#zones_delete) | **DELETE** /zones/{zoneId} | Delete a zone |
 | ZonesApi | [**zones_find_by_id**](docs/api/ZonesApi.md#zones_find_by_id) | **GET** /zones/{zoneId} | Retrieve a zone |
 | ZonesApi | [**zones_get**](docs/api/ZonesApi.md#zones_get) | **GET** /zones | Retrieve zones |
 | ZonesApi | [**zones_post**](docs/api/ZonesApi.md#zones_post) | **POST** /zones | Create a zone |
-| ZonesApi | [**zones_put**](docs/api/ZonesApi.md#zones_put) | **PUT** /zones/{zoneId} | Ensure a zone |
+| ZonesApi | [**zones_put**](docs/api/ZonesApi.md#zones_put) | **PUT** /zones/{zoneId} | Update a zone |
 
 </details>
 
 ## Documentation For Models
 
 All URIs are relative to *https://dns.de-fra.ionos.com*
 <details >
@@ -194,37 +207,47 @@
  - [Algorithm](docs/models/Algorithm)
  - [CommonZone](docs/models/CommonZone)
  - [CommonZoneRead](docs/models/CommonZoneRead)
  - [CommonZoneReadList](docs/models/CommonZoneReadList)
  - [DnssecKey](docs/models/DnssecKey)
  - [DnssecKeyCreate](docs/models/DnssecKeyCreate)
  - [DnssecKeyParameters](docs/models/DnssecKeyParameters)
+ - [DnssecKeyReadCreation](docs/models/DnssecKeyReadCreation)
  - [DnssecKeyReadList](docs/models/DnssecKeyReadList)
  - [DnssecKeyReadListMetadata](docs/models/DnssecKeyReadListMetadata)
+ - [DnssecKeyReadListProperties](docs/models/DnssecKeyReadListProperties)
+ - [DnssecKeyReadListPropertiesKeyParameters](docs/models/DnssecKeyReadListPropertiesKeyParameters)
+ - [DnssecKeyReadListPropertiesNsecParameters](docs/models/DnssecKeyReadListPropertiesNsecParameters)
  - [Error](docs/models/Error)
  - [ErrorMessages](docs/models/ErrorMessages)
  - [KeyData](docs/models/KeyData)
  - [KeyParameters](docs/models/KeyParameters)
  - [KskBits](docs/models/KskBits)
  - [Links](docs/models/Links)
  - [Metadata](docs/models/Metadata)
  - [MetadataForSecondaryZoneRecords](docs/models/MetadataForSecondaryZoneRecords)
  - [MetadataWithStateFqdnZoneId](docs/models/MetadataWithStateFqdnZoneId)
  - [MetadataWithStateFqdnZoneIdAllOf](docs/models/MetadataWithStateFqdnZoneIdAllOf)
  - [MetadataWithStateNameservers](docs/models/MetadataWithStateNameservers)
  - [MetadataWithStateNameserversAllOf](docs/models/MetadataWithStateNameserversAllOf)
+ - [NsecMode](docs/models/NsecMode)
  - [NsecParameters](docs/models/NsecParameters)
  - [ProvisioningState](docs/models/ProvisioningState)
  - [Quota](docs/models/Quota)
  - [QuotaDetail](docs/models/QuotaDetail)
  - [Record](docs/models/Record)
  - [RecordCreate](docs/models/RecordCreate)
  - [RecordEnsure](docs/models/RecordEnsure)
  - [RecordRead](docs/models/RecordRead)
  - [RecordReadList](docs/models/RecordReadList)
+ - [ReverseRecord](docs/models/ReverseRecord)
+ - [ReverseRecordCreate](docs/models/ReverseRecordCreate)
+ - [ReverseRecordEnsure](docs/models/ReverseRecordEnsure)
+ - [ReverseRecordRead](docs/models/ReverseRecordRead)
+ - [ReverseRecordsReadList](docs/models/ReverseRecordsReadList)
  - [SecondaryZone](docs/models/SecondaryZone)
  - [SecondaryZoneAllOf](docs/models/SecondaryZoneAllOf)
  - [SecondaryZoneCreate](docs/models/SecondaryZoneCreate)
  - [SecondaryZoneEnsure](docs/models/SecondaryZoneEnsure)
  - [SecondaryZoneRead](docs/models/SecondaryZoneRead)
  - [SecondaryZoneReadAllOf](docs/models/SecondaryZoneReadAllOf)
  - [SecondaryZoneReadList](docs/models/SecondaryZoneReadList)
```

### Comparing `ionoscloud-dns-1.0.0/ionoscloud_dns.egg-info/SOURCES.txt` & `ionoscloud-dns-1.2.0/ionoscloud_dns.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,48 +15,59 @@
 ionoscloud_dns.egg-info/dependency_links.txt
 ionoscloud_dns.egg-info/requires.txt
 ionoscloud_dns.egg-info/top_level.txt
 ionoscloud_dns/api/__init__.py
 ionoscloud_dns/api/dnssec_api.py
 ionoscloud_dns/api/quota_api.py
 ionoscloud_dns/api/records_api.py
+ionoscloud_dns/api/reverse_records_api.py
 ionoscloud_dns/api/secondary_zones_api.py
 ionoscloud_dns/api/zone_files_api.py
 ionoscloud_dns/api/zones_api.py
 ionoscloud_dns/models/__init__.py
 ionoscloud_dns/models/algorithm.py
 ionoscloud_dns/models/common_zone.py
 ionoscloud_dns/models/common_zone_read.py
 ionoscloud_dns/models/common_zone_read_list.py
 ionoscloud_dns/models/dnssec_key.py
 ionoscloud_dns/models/dnssec_key_create.py
 ionoscloud_dns/models/dnssec_key_parameters.py
+ionoscloud_dns/models/dnssec_key_read_creation.py
 ionoscloud_dns/models/dnssec_key_read_list.py
 ionoscloud_dns/models/dnssec_key_read_list_metadata.py
+ionoscloud_dns/models/dnssec_key_read_list_properties.py
+ionoscloud_dns/models/dnssec_key_read_list_properties_key_parameters.py
+ionoscloud_dns/models/dnssec_key_read_list_properties_nsec_parameters.py
 ionoscloud_dns/models/error.py
 ionoscloud_dns/models/error_messages.py
 ionoscloud_dns/models/key_data.py
 ionoscloud_dns/models/key_parameters.py
 ionoscloud_dns/models/ksk_bits.py
 ionoscloud_dns/models/links.py
 ionoscloud_dns/models/metadata.py
 ionoscloud_dns/models/metadata_for_secondary_zone_records.py
 ionoscloud_dns/models/metadata_with_state_fqdn_zone_id.py
 ionoscloud_dns/models/metadata_with_state_fqdn_zone_id_all_of.py
 ionoscloud_dns/models/metadata_with_state_nameservers.py
 ionoscloud_dns/models/metadata_with_state_nameservers_all_of.py
+ionoscloud_dns/models/nsec_mode.py
 ionoscloud_dns/models/nsec_parameters.py
 ionoscloud_dns/models/provisioning_state.py
 ionoscloud_dns/models/quota.py
 ionoscloud_dns/models/quota_detail.py
 ionoscloud_dns/models/record.py
 ionoscloud_dns/models/record_create.py
 ionoscloud_dns/models/record_ensure.py
 ionoscloud_dns/models/record_read.py
 ionoscloud_dns/models/record_read_list.py
+ionoscloud_dns/models/reverse_record.py
+ionoscloud_dns/models/reverse_record_create.py
+ionoscloud_dns/models/reverse_record_ensure.py
+ionoscloud_dns/models/reverse_record_read.py
+ionoscloud_dns/models/reverse_records_read_list.py
 ionoscloud_dns/models/secondary_zone.py
 ionoscloud_dns/models/secondary_zone_all_of.py
 ionoscloud_dns/models/secondary_zone_create.py
 ionoscloud_dns/models/secondary_zone_ensure.py
 ionoscloud_dns/models/secondary_zone_read.py
 ionoscloud_dns/models/secondary_zone_read_all_of.py
 ionoscloud_dns/models/secondary_zone_read_list.py
```

### Comparing `ionoscloud-dns-1.0.0/pyproject.toml` & `ionoscloud-dns-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ionoscloud_dns"
-version = "1.0.0"
+version = "1.2.0"
 description = "IONOS Cloud - DNS API"
 authors = ["IONOS Cloud Support <support@cloud.ionos.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/ionos-cloud/sdk-python-dns"
 keywords = ["OpenAPI", "OpenAPI-Generator", "IONOS Cloud - DNS API"]
 include = ["ionoscloud_dns/py.typed"]
```

### Comparing `ionoscloud-dns-1.0.0/setup.py` & `ionoscloud-dns-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding: utf-8
 
 """
     IONOS Cloud - DNS API
 
     Cloud DNS service helps IONOS Cloud customers to automate DNS Zone and Record management.   # noqa: E501
 
-    The version of the OpenAPI document: 1.12.0
+    The version of the OpenAPI document: 1.15.4
     Contact: support@cloud.ionos.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup  # noqa: H301
 import os
 import codecs
 
 NAME = "ionoscloud-dns"
-VERSION = "1.0.0"
+VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

