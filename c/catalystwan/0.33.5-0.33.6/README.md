# Comparing `tmp/catalystwan-0.33.5.tar.gz` & `tmp/catalystwan-0.33.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.5.tar", max compression
+gzip compressed data, was "catalystwan-0.33.6.tar", max compression
```

## Comparing `catalystwan-0.33.5.tar` & `catalystwan-0.33.6.tar`

### file list

```diff
@@ -1,341 +1,344 @@
--rw-r--r--   0        0        0    11375 2024-04-30 16:52:48.715403 catalystwan-0.33.5/LICENSE
--rw-r--r--   0        0        0    13533 2024-04-30 16:52:48.715403 catalystwan-0.33.5/README.md
--rw-r--r--   0        0        0     2524 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3220 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4301 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     4645 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    15767 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    28976 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    29260 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3107 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5235 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-04-30 16:52:48.715403 catalystwan-0.33.5/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    15887 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0     7715 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/api/virtual_image_action_api.py
--rw-r--r--   0        0        0    21802 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    25601 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     4037 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2064 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4836 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     2028 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2091 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2092 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2247 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2324 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2174 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2032 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     2073 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2132 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     2039 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2159 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2104 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2263 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2186 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1793 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1950 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1848 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1870 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1827 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1911 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     2016 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1932 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2079 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1806 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1953 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1974 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1932 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1890 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1953 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1848 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1874 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1806 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2115 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1848 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1974 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1781 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1946 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1845 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1806 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1926 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1926 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1787 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1806 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-04-30 16:52:48.719403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    13587 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     5158 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    24950 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14328 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      400 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/monitoring/security_policy.py
--rw-r--r--   0        0        0      347 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3582 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     5747 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1902 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/logging.conf
--rw-r--r--   0        0        0     3079 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     1090 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0    10043 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9117 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0     5553 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1342 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1121 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      577 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1033 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      885 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      731 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1034 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1034 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1268 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
--rw-r--r--   0        0        0     2867 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1028 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5197 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0      925 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1581 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1177 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      759 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      738 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1182 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1496 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      801 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      691 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1131 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0      883 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1384 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0    14665 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     8961 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     3448 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-04-30 16:52:48.723403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0    13826 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0     2179 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      167 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1041 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      346 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/monitoring/security_policy.py
--rw-r--r--   0        0        0      405 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0     4567 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     9426 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5540 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/access_control_list.py
--rw-r--r--   0        0        0     5726 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/access_control_list_ipv6.py
--rw-r--r--   0        0        0    11851 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/control.py
--rw-r--r--   0        0        0     3861 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/device_access.py
--rw-r--r--   0        0        0     3961 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/device_access_ipv6.py
--rw-r--r--   0        0        0     3004 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/hub_and_spoke.py
--rw-r--r--   0        0        0     1184 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/mesh.py
--rw-r--r--   0        0        0     3454 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/qos_map.py
--rw-r--r--   0        0        0     1193 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/rewrite.py
--rw-r--r--   0        0        0    12252 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/rule_set.py
--rw-r--r--   0        0        0     2948 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/security_group.py
--rw-r--r--   0        0        0    13309 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/traffic_data.py
--rw-r--r--   0        0        0     1074 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/vpn_membership.py
--rw-r--r--   0        0        0     9345 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/definitions/zone_based_firewall.py
--rw-r--r--   0        0        0    10893 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/lists.py
--rw-r--r--   0        0        0    14613 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/lists_entries.py
--rw-r--r--   0        0        0     5558 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3553 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    31904 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1274 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     7100 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     5239 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9300 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/response.py
--rw-r--r--   0        0        0    19161 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/session.py
--rw-r--r--   0        0        0      401 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-04-30 16:52:48.727403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     4598 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    33583 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0      894 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     2896 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_monitoring_security_policy.py
--rw-r--r--   0        0        0     1809 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     5883 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    11346 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     8547 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      154 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     5066 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0    17168 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     9946 2024-04-30 16:52:48.731403 catalystwan-0.33.5/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      862 2024-04-30 16:52:48.735403 catalystwan-0.33.5/pyproject.toml
--rw-r--r--   0        0        0    17144 1970-01-01 00:00:00.000000 catalystwan-0.33.5/setup.py
--rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 catalystwan-0.33.5/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-14 22:23:34.199131 catalystwan-0.33.6/LICENSE
+-rw-r--r--   0        0        0    13654 2024-05-14 22:23:34.199131 catalystwan-0.33.6/README.md
+-rw-r--r--   0        0        0     2524 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3220 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0     2053 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4301 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     4645 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     1290 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/configuration_groups/parcels/cellular_controller.py
+-rw-r--r--   0        0        0     7315 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    15767 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    28976 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    29260 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3107 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5235 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    15887 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0     7715 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/virtual_image_action_api.py
+-rw-r--r--   0        0        0    21802 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    25866 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     4037 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2064 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     4836 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     2028 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2091 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2092 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2247 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2324 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     2174 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2032 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     2073 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2132 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     2039 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2159 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     2104 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2263 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2186 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1793 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1950 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1870 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1827 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1911 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     2016 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1932 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2079 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1953 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1932 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1890 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1953 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1874 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2115 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1781 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1946 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1845 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1926 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1926 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1787 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1782 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    13587 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     5158 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    24950 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14444 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      400 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/security_policy.py
+-rw-r--r--   0        0        0      347 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3582 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0      802 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/url_monitoring.py
+-rw-r--r--   0        0        0     5714 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1902 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/logging.conf
+-rw-r--r--   0        0        0     3079 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/common.py
+-rw-r--r--   0        0        0      171 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0     1090 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0    10043 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0     9117 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     1086 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
+-rw-r--r--   0        0        0     5553 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1342 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1121 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      577 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1033 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      885 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      731 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1034 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1268 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
+-rw-r--r--   0        0        0     2867 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1028 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5197 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0      925 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1581 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1177 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      759 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      738 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1182 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1496 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      801 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      691 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1131 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0      883 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     1384 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0    14665 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0     8961 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14020 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     3448 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     3835 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     2777 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    14424 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     9128 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6575 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     7971 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24489 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10081 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3294 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     6725 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    11900 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     6391 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6993 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5179 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3790 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5294 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0    13826 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0     2179 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0      167 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1041 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      346 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/monitoring/security_policy.py
+-rw-r--r--   0        0        0      405 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0     4567 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     9426 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5540 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list.py
+-rw-r--r--   0        0        0     5726 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list_ipv6.py
+-rw-r--r--   0        0        0    11851 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/control.py
+-rw-r--r--   0        0        0     3861 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access.py
+-rw-r--r--   0        0        0     3961 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access_ipv6.py
+-rw-r--r--   0        0        0     3004 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/hub_and_spoke.py
+-rw-r--r--   0        0        0     1184 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/mesh.py
+-rw-r--r--   0        0        0     3454 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/qos_map.py
+-rw-r--r--   0        0        0     1193 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/rewrite.py
+-rw-r--r--   0        0        0    12252 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/rule_set.py
+-rw-r--r--   0        0        0     2948 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/security_group.py
+-rw-r--r--   0        0        0    13309 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/traffic_data.py
+-rw-r--r--   0        0        0     1074 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/vpn_membership.py
+-rw-r--r--   0        0        0     9345 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/zone_based_firewall.py
+-rw-r--r--   0        0        0    10893 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/lists.py
+-rw-r--r--   0        0        0    14613 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/lists_entries.py
+-rw-r--r--   0        0        0     5558 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3553 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    31904 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1274 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     7100 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     5239 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0      924 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/url_monitoring.py
+-rw-r--r--   0        0        0     9586 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/response.py
+-rw-r--r--   0        0        0    19488 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/session.py
+-rw-r--r--   0        0        0      401 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     4598 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1756 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    33583 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0      894 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     2896 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_security_policy.py
+-rw-r--r--   0        0        0     1809 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16472 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7440 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15050 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    11346 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     3746 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_url_monitoring.py
+-rw-r--r--   0        0        0     2968 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     8547 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      154 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     5066 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0    17168 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0     9946 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      862 2024-05-14 22:23:34.219131 catalystwan-0.33.6/pyproject.toml
+-rw-r--r--   0        0        0    17267 1970-01-01 00:00:00.000000 catalystwan-0.33.6/setup.py
+-rw-r--r--   0        0        0    14781 1970-01-01 00:00:00.000000 catalystwan-0.33.6/PKG-INFO
```

### Comparing `catalystwan-0.33.5/LICENSE` & `catalystwan-0.33.6/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/README.md` & `catalystwan-0.33.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,28 +178,30 @@
 n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n)
 ```
 
 To get all critical alarms from past `n` hours:
 
 ```python
+from catalystwan.utils.alarm_status import Severity
 n = 48
 critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
 ```
 
 </details>
 
 <details>
     <summary> <b>Users</b> <i>(click to expand)</i></summary>
 
 ```python
 # Get all users
 session.api.users.get()
 
 # Create user
+from catalystwan.endpoints.administration_user_and_group import User
 new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
 session.api.users.create(new_user)
 
 # Update user data
 new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
 session.api.users.update(new_user_update)
```

#### html2text {}

```diff
@@ -72,18 +72,20 @@
 session.api.repository.upload_image(image) # Install software install_task =
 session.api.software.install(devices=vsmarts, image=image) # Check action
 status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
 get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
 viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
 (viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
-critical alarms from past `n` hours: ```python n = 48 critical_alarms =
+critical alarms from past `n` hours: ```python from
+catalystwan.utils.alarm_status import Severity n = 48 critical_alarms =
 session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
 UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
-Create user new_user = User(username="new_user", password="new_user", group=
+Create user from catalystwan.endpoints.administration_user_and_group import
+User new_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user") session.api.users.create(new_user) #
 Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description") session.api.users.update(new_user_update) # Update user password
 session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
 session.api.users.reset("new_user") # Delete user session.api.users.delete
 ("new_user") # Get current user authentication type and role
```

### Comparing `catalystwan-0.33.5/catalystwan/__init__.py` & `catalystwan-0.33.6/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/abstractions.py` & `catalystwan-0.33.6/catalystwan/abstractions.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     def text(self) -> str:
         ...
 
     @property
     def content(self) -> bytes:
         ...
 
-    def dataobj(self, cls: Type[T], sourcekey: Optional[str]) -> T:
+    def dataobj(self, cls: Type[T], sourcekey: Optional[str], validate: bool) -> T:
         ...
 
-    def dataseq(self, cls: Type[T], sourcekey: Optional[str]) -> DataSequence[T]:
+    def dataseq(self, cls: Type[T], sourcekey: Optional[str], validate: bool) -> DataSequence[T]:
         ...
 
     def json(self) -> dict:
         ...
 
 
 class APIEndpointClient(Protocol):
@@ -48,7 +48,11 @@
     @property
     def api_version(self) -> Optional[Version]:
         ...
 
     @property
     def session_type(self) -> Optional[SessionType]:
         ...
+
+    @property
+    def validate_responses(self) -> bool:
+        ...
```

### Comparing `catalystwan-0.33.5/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.6/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/administration.py` & `catalystwan-0.33.6/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/alarms_api.py` & `catalystwan-0.33.6/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/api_container.py` & `catalystwan-0.33.6/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/basic_api.py` & `catalystwan-0.33.6/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.6/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/config_group_api.py` & `catalystwan-0.33.6/catalystwan/api/config_group_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.6/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/configuration_groups/parcels/cellular_controller.py` & `catalystwan-0.33.6/catalystwan/api/configuration_groups/parcels/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.6/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/device_action_api.py` & `catalystwan-0.33.6/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.6/catalystwan/api/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/logs_api.py` & `catalystwan-0.33.6/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.6/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.6/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/omp_api.py` & `catalystwan-0.33.6/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.6/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/parcel_api.py` & `catalystwan-0.33.6/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.6/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/policy_api.py` & `catalystwan-0.33.6/catalystwan/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.6/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/software_action_api.py` & `catalystwan-0.33.6/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.6/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/task_status_api.py` & `catalystwan-0.33.6/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/template_api.py` & `catalystwan-0.33.6/catalystwan/api/template_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/README.md` & `catalystwan-0.33.6/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.6/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.6/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.6/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.6/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.6/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.6/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.6/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/versions_utils.py` & `catalystwan-0.33.6/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/api/virtual_image_action_api.py` & `catalystwan-0.33.6/catalystwan/api/virtual_image_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/dataclasses.py` & `catalystwan-0.33.6/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.6/catalystwan/endpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,17 +561,23 @@
                         else:
                             raise TypeError(f"Expected dictionary as json payload but found: {type(full_json)}")
                     return full_json
                 if self.return_spec.payload_type is None:
                     pass
                 elif issubclass(self.return_spec.payload_type, BaseModel):
                     if self.return_spec.sequence_type == DataSequence:
-                        return response.dataseq(self.return_spec.payload_type, self.resp_json_key)
+                        return response.dataseq(
+                            cls=self.return_spec.payload_type,
+                            sourcekey=self.resp_json_key,
+                            validate=_self._client.validate_responses,
+                        )
                     else:
-                        return response.dataobj(self.return_spec.payload_type, self.resp_json_key)
+                        return response.dataobj(
+                            self.return_spec.payload_type, self.resp_json_key, validate=_self._client.validate_responses
+                        )
                 elif issubclass(self.return_spec.payload_type, str):
                     return response.text
                 elif issubclass(self.return_spec.payload_type, bytes):
                     return response.content
                 elif issubclass(self.return_spec.payload_type, dict):
                     return response.json()
```

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.6/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.6/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.6/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/client.py` & `catalystwan-0.33.6/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.6/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.6/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.6/catalystwan/endpoints/endpoints_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 from catalystwan.endpoints.monitoring.status import MonitoringStatus
 from catalystwan.endpoints.real_time_monitoring.reboot_history import RealTimeMonitoringRebootHistory
 from catalystwan.endpoints.sdavc_cloud_connector import SDAVCCloudConnector
 from catalystwan.endpoints.tenant_backup_restore import TenantBackupRestore
 from catalystwan.endpoints.tenant_management import TenantManagement
 from catalystwan.endpoints.tenant_migration import TenantMigration
 from catalystwan.endpoints.troubleshooting_tools.device_connectivity import TroubleshootingToolsDeviceConnectivity
+from catalystwan.endpoints.url_monitoring import UrlMonitoring
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 
 class ConfigurationPolicyListContainer:
     def __init__(self, session: ManagerSession):
@@ -211,7 +212,8 @@
         self.configuration_group = ConfigurationGroup(session)
         self.sd_routing_configuration_feature_profile = SDRoutingConfigurationFeatureProfile(session)
         self.configuration_device_inventory = ConfigurationDeviceInventory(session)
         self.troubleshooting_tools = TroubleshootingToolsContainer(session)
         self.misc = MiscellaneousEndpoints(session)
         self.real_time_monitoring = RealTimeMonitoringContainer(session)
         self.certificate_management_device = CertificateManagementDevice(session)
+        self.url_monitoring = UrlMonitoring(session)
```

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/misc.py` & `catalystwan-0.33.6/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.6/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.6/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.6/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.6/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.6/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.6/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.6/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.6/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/exceptions.py` & `catalystwan-0.33.6/catalystwan/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from typing import Any, Optional, Union
+from typing import Union
 
 from pydantic import BaseModel
 from requests import HTTPError, RequestException
 
 
 class ManagerErrorInfo(BaseModel):
     message: Union[str, None]
@@ -15,24 +15,26 @@
 class CatalystwanException(Exception):
     """Superclass of all catalystwan SDK exception types."""
 
 
 class ManagerRequestException(RequestException, CatalystwanException):
     """Exception raised when there is ambigous problem during sending of request to Manager"""
 
-    def __init__(self, *args, **kwargs):
-        """Initialize RequestException with `request` and `response` objects."""
-        super().__init__(*args, **kwargs)
-
 
 class ManagerHTTPError(HTTPError, ManagerRequestException):
-    def __init__(self, *, error_info: Optional[ManagerErrorInfo], request: Any, response: Any):
+    def __init__(self, *args, error_info: ManagerErrorInfo, **kwargs):
         """Initialize RequestException with `error_info`, `request` and `response` objects."""
         self.info = error_info
-        super().__init__(request=request, response=response)
+        info_str = str(self.info)
+        _args = args
+        if not _args:
+            _args = (info_str,)
+        else:
+            _args = (str(_args[0]) + "\n" + info_str,) + _args[1:]
+        super().__init__(*_args, **kwargs)
 
 
 class DefaultPasswordError(CatalystwanException):
     """Default password for SDWAN Manager user was detected and needs to be changed."""
 
     pass
```

### Comparing `catalystwan-0.33.5/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.6/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/logging.conf` & `catalystwan-0.33.6/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/common.py` & `catalystwan-0.33.6/catalystwan/models/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.33.6/catalystwan/models/configuration/config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/device_inventory.py` & `catalystwan-0.33.6/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.6/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.6/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.6/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/access_control_list.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/access_control_list_ipv6.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/control.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/device_access.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/device_access_ipv6.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/hub_and_spoke.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/mesh.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/qos_map.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/rewrite.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/rule_set.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/security_group.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/traffic_data.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/vpn_membership.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/definitions/zone_based_firewall.py` & `catalystwan-0.33.6/catalystwan/models/policy/definitions/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/lists.py` & `catalystwan-0.33.6/catalystwan/models/policy/lists.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/lists_entries.py` & `catalystwan-0.33.6/catalystwan/models/policy/lists_entries.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/localized.py` & `catalystwan-0.33.6/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/policy.py` & `catalystwan-0.33.6/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.6/catalystwan/models/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.6/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/policy/security.py` & `catalystwan-0.33.6/catalystwan/models/policy/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/models/tenant.py` & `catalystwan-0.33.6/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/response.py` & `catalystwan-0.33.6/catalystwan/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         Returns:
             str
         """
         if history:
             return response_history_debug(self, None)
         return response_debug(self, None)
 
-    def dataseq(self, cls: Type[T], sourcekey: Optional[str] = "data") -> DataSequence[T]:
+    def dataseq(self, cls: Type[T], sourcekey: Optional[str] = "data", validate: bool = True) -> DataSequence[T]:
         """Returns data contents from JSON payload parsed as DataSequence of Dataclass/BaseModel instances
         Args:
             cls: Dataclass/BaseModel subtype (eg. Devices)
             sourcekey: name of the JSON key from response payload to be parsed. If None whole JSON payload will be used
 
         Returns:
             DataSequence[T] of given type T which is subclassing from Dataclass/BaseModel,
@@ -191,18 +191,20 @@
 
         if isinstance(data, Sequence):
             sequence = data
         else:
             sequence = [cast(dict, data)]
 
         if issubclass(cls, BaseModel):
-            return DataSequence(cls, [cls.model_validate(item) for item in sequence])  # type: ignore
+            if validate:
+                return DataSequence(cls, [cls.model_validate(item) for item in sequence])  # type: ignore
+            return DataSequence(cls, [cls.model_construct(**item) for item in sequence])  # type: ignore
         return DataSequence(cls, [create_dataclass(cls, item) for item in sequence])
 
-    def dataobj(self, cls: Type[T], sourcekey: Optional[str] = "data") -> T:
+    def dataobj(self, cls: Type[T], sourcekey: Optional[str] = "data", validate: bool = True) -> T:
         """Returns data contents from JSON payload parsed as Dataclass/BaseModel instance
         Args:
             cls: Dataclass/BaseModel subtype (eg. Devices)
             sourcekey: name of the JSON key from response payload to be parsed. If None whole JSON payload will be used
 
         Returns:
             Object of given type T which is subclassing from Dataclass/BaseModel,
@@ -210,15 +212,17 @@
         """
         if sourcekey is None:
             data = self.payload.json
         else:
             data = self.payload.json.get(sourcekey)
 
         if issubclass(cls, BaseModel):
-            return cls.model_validate(data)  # type: ignore[return-value]
+            if validate:
+                return cls.model_validate(data)  # type: ignore[return-value]
+            return cls.model_construct(**data)  # type: ignore[return-value]
         return create_dataclass(cls, data)
 
     def get_error_info(self) -> ManagerErrorInfo:
         """Returns error information from JSON payload"""
 
         if self.payload.error is None:
             return ManagerErrorInfo(
```

### Comparing `catalystwan-0.33.5/catalystwan/session.py` & `catalystwan-0.33.6/catalystwan/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         url: str,
         username: str,
         password: str,
         verify: bool = False,
         port: Optional[int] = None,
         subdomain: Optional[str] = None,
         auth: Optional[AuthBase] = None,
+        validate_responses: bool = True,
     ):
         self.url = url
         self.port = port
         self.base_url = self.__create_base_url()
         self.username = username
         self.password = password
         self.subdomain = subdomain
@@ -173,14 +174,15 @@
         self.api = APIContainer(self)
         self.endpoints = APIEndpointContainter(self)
         self._platform_version: str = ""
         self._api_version: Version
         self._state: ManagerSessionState = ManagerSessionState.OPERATIVE
         self.restart_timeout: int = 1200
         self.polling_requests_timeout: int = 10
+        self._validate_responses = validate_responses
 
     @property
     def state(self) -> ManagerSessionState:
         return self._state
 
     @state.setter
     def state(self, state: ManagerSessionState) -> None:
@@ -232,15 +234,15 @@
         if self.subdomain:
             tenant_id = self.get_tenant_id()
             vsession_id = self.get_virtual_session_id(tenant_id)
             self.headers.update({"VSessionId": vsession_id})
         try:
             server_info = self.server()
         except DefaultPasswordError:
-            server_info = ServerInfo.parse_obj({})
+            server_info = ServerInfo.model_construct(**{})
 
         self.server_name = server_info.server
 
         tenancy_mode = server_info.tenancy_mode
         user_mode = server_info.user_mode
         view_mode = server_info.view_mode
 
@@ -307,15 +309,15 @@
                     if resp.json().get("isServerReady") is True:
                         self.logger.debug(f"Waiting for server ready took: {elapsed()} seconds.")
                         return
                 sleep(poll_period)
                 continue
             except RequestException as exception:
                 self.logger.debug(self.response_trace(exception.response, exception.request))
-                raise ManagerRequestException(request=exception.request, response=exception.response)
+                raise ManagerRequestException(*exception.args)
 
         raise ManagerReadyTimeout(f"Waiting for server ready took longer than {timeout} seconds.")
 
     def request(self, method, url, *args, **kwargs) -> ManagerResponse:
         full_url = self.get_full_url(url)
         try:
             response = super(ManagerSession, self).request(method, full_url, *args, **kwargs)
@@ -324,30 +326,30 @@
                 self.state = ManagerSessionState.WAIT_SERVER_READY_AFTER_RESTART
         except RequestException as exception:
             self.logger.debug(self.response_trace(exception.response, exception.request))
             if self.state == ManagerSessionState.RESTART_IMMINENT and isinstance(exception, ConnectionError):
                 self.state = ManagerSessionState.WAIT_SERVER_READY_AFTER_RESTART
                 return self.request(method, url, *args, **kwargs)
             self.logger.debug(exception)
-            raise ManagerRequestException(request=exception.request, response=exception.response)
+            raise ManagerRequestException(*exception.args, request=exception.request, response=exception.response)
 
         if self.enable_relogin and response.jsessionid_expired and self.state == ManagerSessionState.OPERATIVE:
             self.logger.warning("Logging to session. Reason: expired JSESSIONID detected in response headers")
             self.state = ManagerSessionState.LOGIN
             return self.request(method, url, *args, **kwargs)
 
         if response.request.url and "passwordReset.html" in response.request.url:
             raise DefaultPasswordError("Password must be changed to use this session.")
 
         try:
             response.raise_for_status()
         except HTTPError as error:
             self.logger.debug(error)
             error_info = response.get_error_info()
-            raise ManagerHTTPError(error_info=error_info, request=error.request, response=error.response)
+            raise ManagerHTTPError(*error.args, error_info=error_info, request=error.request, response=error.response)
         return response
 
     def get_full_url(self, url_path: str) -> str:
         """Returns base API url plus given url path."""
         return urljoin(self.base_url, url_path)
 
     def __create_base_url(self) -> str:
@@ -400,15 +402,15 @@
 
     def get_tenant_id(self) -> str:
         """Gets tenant UUID for its subdomain.
 
         Returns:
             Tenant UUID.
         """
-        tenants = self.get("dataservice/tenant").dataseq(Tenant)
+        tenants = self.get("dataservice/tenant").dataseq(Tenant, validate=False)
         tenant = tenants.filter(subdomain=self.subdomain).single_or_default()
 
         if not tenant or not tenant.tenant_id:
             raise TenantSubdomainNotFound(f"Tenant ID for sub-domain: {self.subdomain} not found")
 
         return tenant.tenant_id
 
@@ -476,14 +478,22 @@
         self._platform_version = version
         self._api_version = parse_api_version(version)
 
     @property
     def api_version(self) -> Version:
         return self._api_version
 
+    @property
+    def validate_responses(self) -> bool:
+        return self._validate_responses
+
+    @validate_responses.setter
+    def validate_responses(self, value: bool):
+        self._validate_responses = value
+
     def __str__(self) -> str:
         return f"{self.username}@{self.base_url}"
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}('{self.url}', '{self.username}', '{self.password}', port={self.port}, "
             f"subdomain='{self.subdomain}')"
```

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.6/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.6/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.6/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.6/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.6/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.6/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.6/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_administration.py` & `catalystwan-0.33.6/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.6/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.6/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.6/catalystwan/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.6/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_monitoring_security_policy.py` & `catalystwan-0.33.6/catalystwan/tests/test_monitoring_security_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.6/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.6/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_response.py` & `catalystwan-0.33.6/catalystwan/tests/test_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import unittest
 from typing import Any, List, Optional
 from unittest.mock import patch
 
 from attr import define, field  # type: ignore
 from parameterized import parameterized  # type: ignore
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, ValidationError
 
 from catalystwan.dataclasses import DataclassBase
 from catalystwan.response import ManagerErrorInfo, ManagerResponse
 from catalystwan.typed_list import DataSequence
 
 
 @define
@@ -22,14 +22,19 @@
 
 class ParsedDataTypePydanticV2(BaseModel):
     key1: str
     key2: int
     key3: Optional[float] = Field(default=None)
 
 
+class DataForValidateTest(BaseModel):
+    important: str
+    not_important: ParsedDataTypePydanticV2
+
+
 PARSE_DATASEQ_TEST_DATA: List = [
     (True, None, 0, "data"),
     (True, "string", 0, "data"),
     (True, {}, 0, "data"),
     (True, {"key1": "string", "key2": 12, "key3": 4.5}, 0, "data"),
     (True, 15, 0, "data"),
     (True, {"data": None}, 0, "data"),
@@ -52,14 +57,19 @@
     (True, {"data": "something"}, "data"),
     (False, {"data": {"key1": "string", "key2": 12, "key3": None}}, "data"),
     (True, {"data": {"key1": "string", "key2": 12, "key3": None}}, "other"),
     (False, {"other": {"key1": "string", "key2": 12, "key3": 55.13}}, "other"),
     (True, {"data": [{"key1": "string", "key2": 66}, {"key1": "required", "key2": 18, "key3": 0.1}]}, "data"),
 ]
 
+VALIDATE_DATASEQ_TEST_DATA = [
+    {"important": "correct1", "not_important": {"invalid-key1": "string", "key2": "not int"}},
+    {"important": "correct2", "not_important": {}},
+]
+
 
 class TestResponse(unittest.TestCase):
     @patch("requests.Response")
     def setUp(self, response_mock) -> None:
         self.response_mock = response_mock
         self.response_mock.headers = {"set-cookie": ""}
         self.response_mock.cookies = {}
@@ -132,7 +142,32 @@
         vmng_response = ManagerResponse(self.response_mock)
         error_info = vmng_response.get_error_info()
         assert isinstance(error_info, ManagerErrorInfo)
         if empty_error:
             assert error_info.message is None
             assert error_info.details is None
             assert error_info.code is None
+
+    def test_dataobj_optional_validate(self):
+        # Arrange
+        self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA[0]
+        vmng_response = ManagerResponse(self.response_mock)
+        # Act
+        data = vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=False)
+        # Assert
+        assert isinstance(data, DataForValidateTest)
+        assert data.important == VALIDATE_DATASEQ_TEST_DATA[0]["important"]
+        with self.assertRaises(ValidationError):
+            vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=True)
+
+    def test_dataseq_optional_validate(self):
+        self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA
+        vmng_response = ManagerResponse(self.response_mock)
+        # Act
+        dataseq = vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=False)
+        # Assert
+        assert isinstance(dataseq, DataSequence)
+        for i, data in enumerate(dataseq):
+            assert isinstance(data, DataForValidateTest)
+            assert data.important == VALIDATE_DATASEQ_TEST_DATA[i]["important"]
+        with self.assertRaises(ValidationError):
+            vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=True)
```

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_session.py` & `catalystwan-0.33.6/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_templates.py` & `catalystwan-0.33.6/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.6/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.6/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_version.py` & `catalystwan-0.33.6/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.6/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.6/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/typed_list.py` & `catalystwan-0.33.6/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.6/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/dashboard.py` & `catalystwan-0.33.6/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/device_model.py` & `catalystwan-0.33.6/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/dict.py` & `catalystwan-0.33.6/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.6/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.6/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/operation_status.py` & `catalystwan-0.33.6/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/timezone.py` & `catalystwan-0.33.6/catalystwan/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.6/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/version.py` & `catalystwan-0.33.6/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/vmanage_auth.py` & `catalystwan-0.33.6/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.6/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.5/pyproject.toml` & `catalystwan-0.33.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.5"
+version = "0.33.6"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.33.5/setup.py` & `catalystwan-0.33.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.33.5',
+    'version': '0.33.6',
     'description': 'Cisco Catalyst WAN SDK for Python',
-    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
+    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nfrom catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nfrom catalystwan.endpoints.administration_user_and_group import User\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -34,15 +34,15 @@
 'catalystwan.tests.templates': ['definitions/*', 'definitions/basic/*',
 'schemas/*', 'schemas/basic/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
 'attrs>=21.4.0,<22.0.0', 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0',
 'flake8-quotes>=3.3.1,<4.0.0', 'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0',
 'python-dateutil>=2.8.2,<3.0.0', 'requests-toolbelt>=1.0.0,<2.0.0',
 'requests>=2.27.1,<3.0.0', 'tenacity>=8.1.0,<9.0.0', 'typing-
 extensions>=4.6.1,<5.0.0'] setup_kwargs = { 'name': 'catalystwan', 'version':
-'0.33.5', 'description': 'Cisco Catalyst WAN SDK for Python',
+'0.33.6', 'description': 'Cisco Catalyst WAN SDK for Python',
 'long_description': '
                       \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
 \n\n[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
@@ -121,19 +121,21 @@
 software\n\ninstall_task = session.api.software.install(devices=vsmarts,
 image=image)\n\n# Check action status\ninstall_task.wait_for_completed
 ()\n```\n\n\n\n\n GGeett aallaarrmmss (click to expand)\nTo get all alarms:
 \n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed
 alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter
 (viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn =
 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get
-all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms
-= session.api.alarms.get(from_time=n).filter
+all critical alarms from past `n` hours:\n\n```python\nfrom
+catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms =
+session.api.alarms.get(from_time=n).filter
 (severity=Severity.CRITICAL)\n```\n\n\n\n\n UUsseerrss (click to
 expand)\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create
-user\nnew_user = User(username="new_user", password="new_user", group=
+user\nfrom catalystwan.endpoints.administration_user_and_group import
+User\nnew_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n#
 Update user data\nnew_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description")\nsession.api.users.update(new_user_update)\n\n# Update user
 password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n#
 Reset user\nsession.api.users.reset("new_user")\n\n# Delete
 user\nsession.api.users.delete("new_user")\n\n# Get current user authentication
```

### Comparing `catalystwan-0.33.5/PKG-INFO` & `catalystwan-0.33.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.5
+Version: 0.33.6
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -206,28 +206,30 @@
 n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n)
 ```
 
 To get all critical alarms from past `n` hours:
 
 ```python
+from catalystwan.utils.alarm_status import Severity
 n = 48
 critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
 ```
 
 </details>
 
 <details>
     <summary> <b>Users</b> <i>(click to expand)</i></summary>
 
 ```python
 # Get all users
 session.api.users.get()
 
 # Create user
+from catalystwan.endpoints.administration_user_and_group import User
 new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
 session.api.users.create(new_user)
 
 # Update user data
 new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
 session.api.users.update(new_user_update)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.5 Summary: Cisco Catalyst
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.6 Summary: Cisco Catalyst
 WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-catalyst-wan-
 sdk Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist: ciscoconfparse
@@ -87,18 +87,20 @@
 session.api.repository.upload_image(image) # Install software install_task =
 session.api.software.install(devices=vsmarts, image=image) # Check action
 status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
 get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
 viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
 (viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
-critical alarms from past `n` hours: ```python n = 48 critical_alarms =
+critical alarms from past `n` hours: ```python from
+catalystwan.utils.alarm_status import Severity n = 48 critical_alarms =
 session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
 UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
-Create user new_user = User(username="new_user", password="new_user", group=
+Create user from catalystwan.endpoints.administration_user_and_group import
+User new_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user") session.api.users.create(new_user) #
 Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description") session.api.users.update(new_user_update) # Update user password
 session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
 session.api.users.reset("new_user") # Delete user session.api.users.delete
 ("new_user") # Get current user authentication type and role
```

