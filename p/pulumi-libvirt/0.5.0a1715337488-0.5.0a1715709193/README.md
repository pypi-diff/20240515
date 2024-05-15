# Comparing `tmp/pulumi_libvirt-0.5.0a1715337488.tar.gz` & `tmp/pulumi_libvirt-0.5.0a1715709193.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.5.0a1715337488.tar", last modified: Fri May 10 10:45:08 2024, max compression
+gzip compressed data, was "pulumi_libvirt-0.5.0a1715709193.tar", last modified: Tue May 14 17:57:08 2024, max compression
```

## Comparing `pulumi_libvirt-0.5.0a1715337488.tar` & `pulumi_libvirt-0.5.0a1715709193.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:45:08.311232 pulumi_libvirt-0.5.0a1715337488/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-10 10:45:08.311232 pulumi_libvirt-0.5.0a1715337488/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:45:08.307232 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:45:08.311232 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:45:08.311232 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-10 10:45:08.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-10 10:45:08.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:45:08.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 10:45:08.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 10:45:08.000000 pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-10 10:45:01.000000 pulumi_libvirt-0.5.0a1715337488/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:45:08.311232 pulumi_libvirt-0.5.0a1715337488/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:57:08.128564 pulumi_libvirt-0.5.0a1715709193/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-14 17:57:08.128564 pulumi_libvirt-0.5.0a1715709193/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:57:08.124565 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:57:08.128564 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40872 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:57:08.128564 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-14 17:57:08.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-14 17:57:08.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:57:08.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 17:57:08.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 17:57:08.000000 pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-14 17:57:01.000000 pulumi_libvirt-0.5.0a1715709193/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:57:08.128564 pulumi_libvirt-0.5.0a1715709193/setup.cfg
```

### Comparing `pulumi_libvirt-0.5.0a1715337488/PKG-INFO` & `pulumi_libvirt-0.5.0a1715709193/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1715337488
+Version: 0.5.0a1715709193
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1715337488/README.md` & `pulumi_libvirt-0.5.0a1715709193/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/network.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,705 +7,606 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['NetworkArgs', 'Network']
+__all__ = ['VolumeArgs', 'Volume']
 
 @pulumi.input_type
-class NetworkArgs:
+class VolumeArgs:
     def __init__(__self__, *,
-                 addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 autostart: Optional[pulumi.Input[bool]] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 dhcp: Optional[pulumi.Input['NetworkDhcpArgs']] = None,
-                 dns: Optional[pulumi.Input['NetworkDnsArgs']] = None,
-                 dnsmasq_options: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 mtu: Optional[pulumi.Input[int]] = None,
+                 base_volume_id: Optional[pulumi.Input[str]] = None,
+                 base_volume_name: Optional[pulumi.Input[str]] = None,
+                 base_volume_pool: Optional[pulumi.Input[str]] = None,
+                 format: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]] = None,
-                 xml: Optional[pulumi.Input['NetworkXmlArgs']] = None):
-        """
-        The set of arguments for constructing a Network resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-               CIDR notation.  This defines the subnets associated to that network.
-               This argument is also used to define the address on the real host.
-               If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-               the DHCP server.
-               No DHCP server will be started if `addresses` is omitted.
-        :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
-               If not specified `false` is assumed.
-        :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
-               device which will be used to construct the virtual network (when not provided,
-               it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input['NetworkDnsArgs'] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[str] domain: The domain used by the DNS server.
-        :param pulumi.Input[str] mode: One of:
-        :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
-               not supplied, libvirt will use the default for the interface, usually 1500.
-               Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+                 pool: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 xml: Optional[pulumi.Input['VolumeXmlArgs']] = None):
+        """
+        The set of arguments for constructing a Volume resource.
+        :param pulumi.Input[str] base_volume_id: The backing volume (CoW) to use for this volume.
+        :param pulumi.Input[str] base_volume_name: The name of the backing volume (CoW) to use
+               for this volume. Note well: when `base_volume_pool` is not specified the
+               volume is going to be searched inside of `pool`.
+        :param pulumi.Input[str] base_volume_pool: The name of the storage pool containing the
+               volume defined by `base_volume_name`.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
-        :param pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]] routes: a list of static routes. A `cidr` and a `gateway` must
-               be provided. The `gateway` must be reachable via the bridge interface.
-        """
-        if addresses is not None:
-            pulumi.set(__self__, "addresses", addresses)
-        if autostart is not None:
-            pulumi.set(__self__, "autostart", autostart)
-        if bridge is not None:
-            pulumi.set(__self__, "bridge", bridge)
-        if dhcp is not None:
-            pulumi.set(__self__, "dhcp", dhcp)
-        if dns is not None:
-            pulumi.set(__self__, "dns", dns)
-        if dnsmasq_options is not None:
-            pulumi.set(__self__, "dnsmasq_options", dnsmasq_options)
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if mode is not None:
-            pulumi.set(__self__, "mode", mode)
-        if mtu is not None:
-            pulumi.set(__self__, "mtu", mtu)
+        :param pulumi.Input[str] pool: The storage pool where the resource will be created.
+               If not given, the `default` storage pool will be used.
+        :param pulumi.Input[int] size: The size of the volume in bytes (if you don't like this,
+               help fix this issue.
+               If `source` is specified, `size` will be set to the source image file size.
+               `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+               `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+               If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
+        """
+        if base_volume_id is not None:
+            pulumi.set(__self__, "base_volume_id", base_volume_id)
+        if base_volume_name is not None:
+            pulumi.set(__self__, "base_volume_name", base_volume_name)
+        if base_volume_pool is not None:
+            pulumi.set(__self__, "base_volume_pool", base_volume_pool)
+        if format is not None:
+            pulumi.set(__self__, "format", format)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if routes is not None:
-            pulumi.set(__self__, "routes", routes)
+        if pool is not None:
+            pulumi.set(__self__, "pool", pool)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if source is not None:
+            pulumi.set(__self__, "source", source)
         if xml is not None:
             pulumi.set(__self__, "xml", xml)
 
     @property
-    @pulumi.getter
-    def addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="baseVolumeId")
+    def base_volume_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-        CIDR notation.  This defines the subnets associated to that network.
-        This argument is also used to define the address on the real host.
-        If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-        the DHCP server.
-        No DHCP server will be started if `addresses` is omitted.
+        The backing volume (CoW) to use for this volume.
         """
-        return pulumi.get(self, "addresses")
+        return pulumi.get(self, "base_volume_id")
 
-    @addresses.setter
-    def addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "addresses", value)
+    @base_volume_id.setter
+    def base_volume_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_id", value)
 
     @property
-    @pulumi.getter
-    def autostart(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="baseVolumeName")
+    def base_volume_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to `true` to start the network on host boot up.
-        If not specified `false` is assumed.
+        The name of the backing volume (CoW) to use
+        for this volume. Note well: when `base_volume_pool` is not specified the
+        volume is going to be searched inside of `pool`.
         """
-        return pulumi.get(self, "autostart")
-
-    @autostart.setter
-    def autostart(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "autostart", value)
-
-    @property
-    @pulumi.getter
-    def bridge(self) -> Optional[pulumi.Input[str]]:
-        """
-        The bridge device defines the name of a bridge
-        device which will be used to construct the virtual network (when not provided,
-        it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        """
-        return pulumi.get(self, "bridge")
-
-    @bridge.setter
-    def bridge(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "bridge", value)
-
-    @property
-    @pulumi.getter
-    def dhcp(self) -> Optional[pulumi.Input['NetworkDhcpArgs']]:
-        return pulumi.get(self, "dhcp")
+        return pulumi.get(self, "base_volume_name")
 
-    @dhcp.setter
-    def dhcp(self, value: Optional[pulumi.Input['NetworkDhcpArgs']]):
-        pulumi.set(self, "dhcp", value)
+    @base_volume_name.setter
+    def base_volume_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_name", value)
 
     @property
-    @pulumi.getter
-    def dns(self) -> Optional[pulumi.Input['NetworkDnsArgs']]:
+    @pulumi.getter(name="baseVolumePool")
+    def base_volume_pool(self) -> Optional[pulumi.Input[str]]:
         """
-        configuration of DNS specific settings for the network
+        The name of the storage pool containing the
+        volume defined by `base_volume_name`.
         """
-        return pulumi.get(self, "dns")
+        return pulumi.get(self, "base_volume_pool")
 
-    @dns.setter
-    def dns(self, value: Optional[pulumi.Input['NetworkDnsArgs']]):
-        pulumi.set(self, "dns", value)
-
-    @property
-    @pulumi.getter(name="dnsmasqOptions")
-    def dnsmasq_options(self) -> Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]:
-        return pulumi.get(self, "dnsmasq_options")
-
-    @dnsmasq_options.setter
-    def dnsmasq_options(self, value: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]):
-        pulumi.set(self, "dnsmasq_options", value)
+    @base_volume_pool.setter
+    def base_volume_pool(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_pool", value)
 
     @property
     @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
-        """
-        The domain used by the DNS server.
-        """
-        return pulumi.get(self, "domain")
+    def format(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "format")
 
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
+    @format.setter
+    def format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "format", value)
 
     @property
     @pulumi.getter
-    def mode(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        One of:
+        A unique name for the resource, required by libvirt.
+        Changing this forces a new resource to be created.
         """
-        return pulumi.get(self, "mode")
+        return pulumi.get(self, "name")
 
-    @mode.setter
-    def mode(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "mode", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def mtu(self) -> Optional[pulumi.Input[int]]:
+    def pool(self) -> Optional[pulumi.Input[str]]:
         """
-        The MTU to set for the underlying network interfaces. When
-        not supplied, libvirt will use the default for the interface, usually 1500.
-        Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+        The storage pool where the resource will be created.
+        If not given, the `default` storage pool will be used.
         """
-        return pulumi.get(self, "mtu")
+        return pulumi.get(self, "pool")
 
-    @mtu.setter
-    def mtu(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "mtu", value)
+    @pool.setter
+    def pool(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pool", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        A unique name for the resource, required by libvirt.
-        Changing this forces a new resource to be created.
+        The size of the volume in bytes (if you don't like this,
+        help fix this issue.
+        If `source` is specified, `size` will be set to the source image file size.
+        `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+        `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+        If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "size")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
-    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]]:
-        """
-        a list of static routes. A `cidr` and a `gateway` must
-        be provided. The `gateway` must be reachable via the bridge interface.
-        """
-        return pulumi.get(self, "routes")
+    def source(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "source")
 
-    @routes.setter
-    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]]):
-        pulumi.set(self, "routes", value)
+    @source.setter
+    def source(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
-    def xml(self) -> Optional[pulumi.Input['NetworkXmlArgs']]:
+    def xml(self) -> Optional[pulumi.Input['VolumeXmlArgs']]:
         return pulumi.get(self, "xml")
 
     @xml.setter
-    def xml(self, value: Optional[pulumi.Input['NetworkXmlArgs']]):
+    def xml(self, value: Optional[pulumi.Input['VolumeXmlArgs']]):
         pulumi.set(self, "xml", value)
 
 
 @pulumi.input_type
-class _NetworkState:
+class _VolumeState:
     def __init__(__self__, *,
-                 addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 autostart: Optional[pulumi.Input[bool]] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 dhcp: Optional[pulumi.Input['NetworkDhcpArgs']] = None,
-                 dns: Optional[pulumi.Input['NetworkDnsArgs']] = None,
-                 dnsmasq_options: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 mtu: Optional[pulumi.Input[int]] = None,
+                 base_volume_id: Optional[pulumi.Input[str]] = None,
+                 base_volume_name: Optional[pulumi.Input[str]] = None,
+                 base_volume_pool: Optional[pulumi.Input[str]] = None,
+                 format: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]] = None,
-                 xml: Optional[pulumi.Input['NetworkXmlArgs']] = None):
-        """
-        Input properties used for looking up and filtering Network resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-               CIDR notation.  This defines the subnets associated to that network.
-               This argument is also used to define the address on the real host.
-               If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-               the DHCP server.
-               No DHCP server will be started if `addresses` is omitted.
-        :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
-               If not specified `false` is assumed.
-        :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
-               device which will be used to construct the virtual network (when not provided,
-               it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input['NetworkDnsArgs'] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[str] domain: The domain used by the DNS server.
-        :param pulumi.Input[str] mode: One of:
-        :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
-               not supplied, libvirt will use the default for the interface, usually 1500.
-               Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+                 pool: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 xml: Optional[pulumi.Input['VolumeXmlArgs']] = None):
+        """
+        Input properties used for looking up and filtering Volume resources.
+        :param pulumi.Input[str] base_volume_id: The backing volume (CoW) to use for this volume.
+        :param pulumi.Input[str] base_volume_name: The name of the backing volume (CoW) to use
+               for this volume. Note well: when `base_volume_pool` is not specified the
+               volume is going to be searched inside of `pool`.
+        :param pulumi.Input[str] base_volume_pool: The name of the storage pool containing the
+               volume defined by `base_volume_name`.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
-        :param pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]] routes: a list of static routes. A `cidr` and a `gateway` must
-               be provided. The `gateway` must be reachable via the bridge interface.
-        """
-        if addresses is not None:
-            pulumi.set(__self__, "addresses", addresses)
-        if autostart is not None:
-            pulumi.set(__self__, "autostart", autostart)
-        if bridge is not None:
-            pulumi.set(__self__, "bridge", bridge)
-        if dhcp is not None:
-            pulumi.set(__self__, "dhcp", dhcp)
-        if dns is not None:
-            pulumi.set(__self__, "dns", dns)
-        if dnsmasq_options is not None:
-            pulumi.set(__self__, "dnsmasq_options", dnsmasq_options)
-        if domain is not None:
-            pulumi.set(__self__, "domain", domain)
-        if mode is not None:
-            pulumi.set(__self__, "mode", mode)
-        if mtu is not None:
-            pulumi.set(__self__, "mtu", mtu)
+        :param pulumi.Input[str] pool: The storage pool where the resource will be created.
+               If not given, the `default` storage pool will be used.
+        :param pulumi.Input[int] size: The size of the volume in bytes (if you don't like this,
+               help fix this issue.
+               If `source` is specified, `size` will be set to the source image file size.
+               `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+               `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+               If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
+        """
+        if base_volume_id is not None:
+            pulumi.set(__self__, "base_volume_id", base_volume_id)
+        if base_volume_name is not None:
+            pulumi.set(__self__, "base_volume_name", base_volume_name)
+        if base_volume_pool is not None:
+            pulumi.set(__self__, "base_volume_pool", base_volume_pool)
+        if format is not None:
+            pulumi.set(__self__, "format", format)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if routes is not None:
-            pulumi.set(__self__, "routes", routes)
+        if pool is not None:
+            pulumi.set(__self__, "pool", pool)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if source is not None:
+            pulumi.set(__self__, "source", source)
         if xml is not None:
             pulumi.set(__self__, "xml", xml)
 
     @property
-    @pulumi.getter
-    def addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="baseVolumeId")
+    def base_volume_id(self) -> Optional[pulumi.Input[str]]:
         """
-        A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-        CIDR notation.  This defines the subnets associated to that network.
-        This argument is also used to define the address on the real host.
-        If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-        the DHCP server.
-        No DHCP server will be started if `addresses` is omitted.
+        The backing volume (CoW) to use for this volume.
         """
-        return pulumi.get(self, "addresses")
+        return pulumi.get(self, "base_volume_id")
 
-    @addresses.setter
-    def addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "addresses", value)
+    @base_volume_id.setter
+    def base_volume_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_id", value)
 
     @property
-    @pulumi.getter
-    def autostart(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="baseVolumeName")
+    def base_volume_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to `true` to start the network on host boot up.
-        If not specified `false` is assumed.
+        The name of the backing volume (CoW) to use
+        for this volume. Note well: when `base_volume_pool` is not specified the
+        volume is going to be searched inside of `pool`.
         """
-        return pulumi.get(self, "autostart")
+        return pulumi.get(self, "base_volume_name")
 
-    @autostart.setter
-    def autostart(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "autostart", value)
+    @base_volume_name.setter
+    def base_volume_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_name", value)
 
     @property
-    @pulumi.getter
-    def bridge(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="baseVolumePool")
+    def base_volume_pool(self) -> Optional[pulumi.Input[str]]:
         """
-        The bridge device defines the name of a bridge
-        device which will be used to construct the virtual network (when not provided,
-        it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
+        The name of the storage pool containing the
+        volume defined by `base_volume_name`.
         """
-        return pulumi.get(self, "bridge")
-
-    @bridge.setter
-    def bridge(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "bridge", value)
-
-    @property
-    @pulumi.getter
-    def dhcp(self) -> Optional[pulumi.Input['NetworkDhcpArgs']]:
-        return pulumi.get(self, "dhcp")
+        return pulumi.get(self, "base_volume_pool")
 
-    @dhcp.setter
-    def dhcp(self, value: Optional[pulumi.Input['NetworkDhcpArgs']]):
-        pulumi.set(self, "dhcp", value)
+    @base_volume_pool.setter
+    def base_volume_pool(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_volume_pool", value)
 
     @property
     @pulumi.getter
-    def dns(self) -> Optional[pulumi.Input['NetworkDnsArgs']]:
-        """
-        configuration of DNS specific settings for the network
-        """
-        return pulumi.get(self, "dns")
-
-    @dns.setter
-    def dns(self, value: Optional[pulumi.Input['NetworkDnsArgs']]):
-        pulumi.set(self, "dns", value)
+    def format(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "format")
 
-    @property
-    @pulumi.getter(name="dnsmasqOptions")
-    def dnsmasq_options(self) -> Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]:
-        return pulumi.get(self, "dnsmasq_options")
-
-    @dnsmasq_options.setter
-    def dnsmasq_options(self, value: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]):
-        pulumi.set(self, "dnsmasq_options", value)
+    @format.setter
+    def format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "format", value)
 
     @property
     @pulumi.getter
-    def domain(self) -> Optional[pulumi.Input[str]]:
-        """
-        The domain used by the DNS server.
-        """
-        return pulumi.get(self, "domain")
-
-    @domain.setter
-    def domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "domain", value)
-
-    @property
-    @pulumi.getter
-    def mode(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        One of:
+        A unique name for the resource, required by libvirt.
+        Changing this forces a new resource to be created.
         """
-        return pulumi.get(self, "mode")
+        return pulumi.get(self, "name")
 
-    @mode.setter
-    def mode(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "mode", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def mtu(self) -> Optional[pulumi.Input[int]]:
+    def pool(self) -> Optional[pulumi.Input[str]]:
         """
-        The MTU to set for the underlying network interfaces. When
-        not supplied, libvirt will use the default for the interface, usually 1500.
-        Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+        The storage pool where the resource will be created.
+        If not given, the `default` storage pool will be used.
         """
-        return pulumi.get(self, "mtu")
+        return pulumi.get(self, "pool")
 
-    @mtu.setter
-    def mtu(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "mtu", value)
+    @pool.setter
+    def pool(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pool", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        A unique name for the resource, required by libvirt.
-        Changing this forces a new resource to be created.
+        The size of the volume in bytes (if you don't like this,
+        help fix this issue.
+        If `source` is specified, `size` will be set to the source image file size.
+        `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+        `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+        If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "size")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
-    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]]:
-        """
-        a list of static routes. A `cidr` and a `gateway` must
-        be provided. The `gateway` must be reachable via the bridge interface.
-        """
-        return pulumi.get(self, "routes")
+    def source(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "source")
 
-    @routes.setter
-    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkRouteArgs']]]]):
-        pulumi.set(self, "routes", value)
+    @source.setter
+    def source(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
-    def xml(self) -> Optional[pulumi.Input['NetworkXmlArgs']]:
+    def xml(self) -> Optional[pulumi.Input['VolumeXmlArgs']]:
         return pulumi.get(self, "xml")
 
     @xml.setter
-    def xml(self, value: Optional[pulumi.Input['NetworkXmlArgs']]):
+    def xml(self, value: Optional[pulumi.Input['VolumeXmlArgs']]):
         pulumi.set(self, "xml", value)
 
 
-class Network(pulumi.CustomResource):
+class Volume(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 autostart: Optional[pulumi.Input[bool]] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 dhcp: Optional[pulumi.Input[pulumi.InputType['NetworkDhcpArgs']]] = None,
-                 dns: Optional[pulumi.Input[pulumi.InputType['NetworkDnsArgs']]] = None,
-                 dnsmasq_options: Optional[pulumi.Input[pulumi.InputType['NetworkDnsmasqOptionsArgs']]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 mtu: Optional[pulumi.Input[int]] = None,
+                 base_volume_id: Optional[pulumi.Input[str]] = None,
+                 base_volume_name: Optional[pulumi.Input[str]] = None,
+                 base_volume_pool: Optional[pulumi.Input[str]] = None,
+                 format: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkRouteArgs']]]]] = None,
-                 xml: Optional[pulumi.Input[pulumi.InputType['NetworkXmlArgs']]] = None,
+                 pool: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 xml: Optional[pulumi.Input[pulumi.InputType['VolumeXmlArgs']]] = None,
                  __props__=None):
         """
-        Manages a VM network resource within libvirt. For more information see
-        [the official documentation](https://libvirt.org/formatnetwork.html).
+        Manages a storage volume in libvirt. For more information see
+        [the official documentation](https://libvirt.org/formatstorage.html).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_libvirt as libvirt
+
+        # Base OS image to use to create a cluster of different
+        # nodes
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
+            source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
+        # volume to attach to the "master" domain as main disk
+        master = libvirt.Volume("master",
+            name="master.qcow2",
+            base_volume_id=opensuse_leap.id)
+        # volumes to attach to the "workers" domains as main disk
+        worker = []
+        for range in [{"value": i} for i in range(0, workers_count)]:
+            worker.append(libvirt.Volume(f"worker-{range['value']}",
+                name=f"worker_{range['value']}.qcow2",
+                base_volume_id=opensuse_leap.id))
+        ```
+
+        > **Tip:** when provisioning multiple domains using the same base image, create
+        a `Volume` for the base image and then define the domain specific ones
+        as based on it. This way the image will not be modified and no extra disk space
+        is going to be used for the base image.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-               CIDR notation.  This defines the subnets associated to that network.
-               This argument is also used to define the address on the real host.
-               If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-               the DHCP server.
-               No DHCP server will be started if `addresses` is omitted.
-        :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
-               If not specified `false` is assumed.
-        :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
-               device which will be used to construct the virtual network (when not provided,
-               it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input[pulumi.InputType['NetworkDnsArgs']] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[str] domain: The domain used by the DNS server.
-        :param pulumi.Input[str] mode: One of:
-        :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
-               not supplied, libvirt will use the default for the interface, usually 1500.
-               Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+        :param pulumi.Input[str] base_volume_id: The backing volume (CoW) to use for this volume.
+        :param pulumi.Input[str] base_volume_name: The name of the backing volume (CoW) to use
+               for this volume. Note well: when `base_volume_pool` is not specified the
+               volume is going to be searched inside of `pool`.
+        :param pulumi.Input[str] base_volume_pool: The name of the storage pool containing the
+               volume defined by `base_volume_name`.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkRouteArgs']]]] routes: a list of static routes. A `cidr` and a `gateway` must
-               be provided. The `gateway` must be reachable via the bridge interface.
+        :param pulumi.Input[str] pool: The storage pool where the resource will be created.
+               If not given, the `default` storage pool will be used.
+        :param pulumi.Input[int] size: The size of the volume in bytes (if you don't like this,
+               help fix this issue.
+               If `source` is specified, `size` will be set to the source image file size.
+               `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+               `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+               If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[NetworkArgs] = None,
+                 args: Optional[VolumeArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages a VM network resource within libvirt. For more information see
-        [the official documentation](https://libvirt.org/formatnetwork.html).
+        Manages a storage volume in libvirt. For more information see
+        [the official documentation](https://libvirt.org/formatstorage.html).
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_libvirt as libvirt
+
+        # Base OS image to use to create a cluster of different
+        # nodes
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
+            source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
+        # volume to attach to the "master" domain as main disk
+        master = libvirt.Volume("master",
+            name="master.qcow2",
+            base_volume_id=opensuse_leap.id)
+        # volumes to attach to the "workers" domains as main disk
+        worker = []
+        for range in [{"value": i} for i in range(0, workers_count)]:
+            worker.append(libvirt.Volume(f"worker-{range['value']}",
+                name=f"worker_{range['value']}.qcow2",
+                base_volume_id=opensuse_leap.id))
+        ```
+
+        > **Tip:** when provisioning multiple domains using the same base image, create
+        a `Volume` for the base image and then define the domain specific ones
+        as based on it. This way the image will not be modified and no extra disk space
+        is going to be used for the base image.
 
         :param str resource_name: The name of the resource.
-        :param NetworkArgs args: The arguments to use to populate this resource's properties.
+        :param VolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NetworkArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 autostart: Optional[pulumi.Input[bool]] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 dhcp: Optional[pulumi.Input[pulumi.InputType['NetworkDhcpArgs']]] = None,
-                 dns: Optional[pulumi.Input[pulumi.InputType['NetworkDnsArgs']]] = None,
-                 dnsmasq_options: Optional[pulumi.Input[pulumi.InputType['NetworkDnsmasqOptionsArgs']]] = None,
-                 domain: Optional[pulumi.Input[str]] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 mtu: Optional[pulumi.Input[int]] = None,
+                 base_volume_id: Optional[pulumi.Input[str]] = None,
+                 base_volume_name: Optional[pulumi.Input[str]] = None,
+                 base_volume_pool: Optional[pulumi.Input[str]] = None,
+                 format: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkRouteArgs']]]]] = None,
-                 xml: Optional[pulumi.Input[pulumi.InputType['NetworkXmlArgs']]] = None,
+                 pool: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 xml: Optional[pulumi.Input[pulumi.InputType['VolumeXmlArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NetworkArgs.__new__(NetworkArgs)
+            __props__ = VolumeArgs.__new__(VolumeArgs)
 
-            __props__.__dict__["addresses"] = addresses
-            __props__.__dict__["autostart"] = autostart
-            __props__.__dict__["bridge"] = bridge
-            __props__.__dict__["dhcp"] = dhcp
-            __props__.__dict__["dns"] = dns
-            __props__.__dict__["dnsmasq_options"] = dnsmasq_options
-            __props__.__dict__["domain"] = domain
-            __props__.__dict__["mode"] = mode
-            __props__.__dict__["mtu"] = mtu
+            __props__.__dict__["base_volume_id"] = base_volume_id
+            __props__.__dict__["base_volume_name"] = base_volume_name
+            __props__.__dict__["base_volume_pool"] = base_volume_pool
+            __props__.__dict__["format"] = format
             __props__.__dict__["name"] = name
-            __props__.__dict__["routes"] = routes
+            __props__.__dict__["pool"] = pool
+            __props__.__dict__["size"] = size
+            __props__.__dict__["source"] = source
             __props__.__dict__["xml"] = xml
-        super(Network, __self__).__init__(
-            'libvirt:index/network:Network',
+        super(Volume, __self__).__init__(
+            'libvirt:index/volume:Volume',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            autostart: Optional[pulumi.Input[bool]] = None,
-            bridge: Optional[pulumi.Input[str]] = None,
-            dhcp: Optional[pulumi.Input[pulumi.InputType['NetworkDhcpArgs']]] = None,
-            dns: Optional[pulumi.Input[pulumi.InputType['NetworkDnsArgs']]] = None,
-            dnsmasq_options: Optional[pulumi.Input[pulumi.InputType['NetworkDnsmasqOptionsArgs']]] = None,
-            domain: Optional[pulumi.Input[str]] = None,
-            mode: Optional[pulumi.Input[str]] = None,
-            mtu: Optional[pulumi.Input[int]] = None,
+            base_volume_id: Optional[pulumi.Input[str]] = None,
+            base_volume_name: Optional[pulumi.Input[str]] = None,
+            base_volume_pool: Optional[pulumi.Input[str]] = None,
+            format: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            routes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkRouteArgs']]]]] = None,
-            xml: Optional[pulumi.Input[pulumi.InputType['NetworkXmlArgs']]] = None) -> 'Network':
+            pool: Optional[pulumi.Input[str]] = None,
+            size: Optional[pulumi.Input[int]] = None,
+            source: Optional[pulumi.Input[str]] = None,
+            xml: Optional[pulumi.Input[pulumi.InputType['VolumeXmlArgs']]] = None) -> 'Volume':
         """
-        Get an existing Network resource's state with the given name, id, and optional extra
+        Get an existing Volume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] addresses: A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-               CIDR notation.  This defines the subnets associated to that network.
-               This argument is also used to define the address on the real host.
-               If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-               the DHCP server.
-               No DHCP server will be started if `addresses` is omitted.
-        :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
-               If not specified `false` is assumed.
-        :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
-               device which will be used to construct the virtual network (when not provided,
-               it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input[pulumi.InputType['NetworkDnsArgs']] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[str] domain: The domain used by the DNS server.
-        :param pulumi.Input[str] mode: One of:
-        :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
-               not supplied, libvirt will use the default for the interface, usually 1500.
-               Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+        :param pulumi.Input[str] base_volume_id: The backing volume (CoW) to use for this volume.
+        :param pulumi.Input[str] base_volume_name: The name of the backing volume (CoW) to use
+               for this volume. Note well: when `base_volume_pool` is not specified the
+               volume is going to be searched inside of `pool`.
+        :param pulumi.Input[str] base_volume_pool: The name of the storage pool containing the
+               volume defined by `base_volume_name`.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkRouteArgs']]]] routes: a list of static routes. A `cidr` and a `gateway` must
-               be provided. The `gateway` must be reachable via the bridge interface.
+        :param pulumi.Input[str] pool: The storage pool where the resource will be created.
+               If not given, the `default` storage pool will be used.
+        :param pulumi.Input[int] size: The size of the volume in bytes (if you don't like this,
+               help fix this issue.
+               If `source` is specified, `size` will be set to the source image file size.
+               `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+               `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+               If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NetworkState.__new__(_NetworkState)
+        __props__ = _VolumeState.__new__(_VolumeState)
 
-        __props__.__dict__["addresses"] = addresses
-        __props__.__dict__["autostart"] = autostart
-        __props__.__dict__["bridge"] = bridge
-        __props__.__dict__["dhcp"] = dhcp
-        __props__.__dict__["dns"] = dns
-        __props__.__dict__["dnsmasq_options"] = dnsmasq_options
-        __props__.__dict__["domain"] = domain
-        __props__.__dict__["mode"] = mode
-        __props__.__dict__["mtu"] = mtu
+        __props__.__dict__["base_volume_id"] = base_volume_id
+        __props__.__dict__["base_volume_name"] = base_volume_name
+        __props__.__dict__["base_volume_pool"] = base_volume_pool
+        __props__.__dict__["format"] = format
         __props__.__dict__["name"] = name
-        __props__.__dict__["routes"] = routes
+        __props__.__dict__["pool"] = pool
+        __props__.__dict__["size"] = size
+        __props__.__dict__["source"] = source
         __props__.__dict__["xml"] = xml
-        return Network(resource_name, opts=opts, __props__=__props__)
+        return Volume(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    @pulumi.getter(name="baseVolumeId")
+    def base_volume_id(self) -> pulumi.Output[Optional[str]]:
         """
-        A list of (0 or 1) IPv4 and (0 or 1) IPv6 subnets in
-        CIDR notation.  This defines the subnets associated to that network.
-        This argument is also used to define the address on the real host.
-        If `dhcp {  enabled = true }` addresses is also used to define the address range served by
-        the DHCP server.
-        No DHCP server will be started if `addresses` is omitted.
+        The backing volume (CoW) to use for this volume.
         """
-        return pulumi.get(self, "addresses")
+        return pulumi.get(self, "base_volume_id")
 
     @property
-    @pulumi.getter
-    def autostart(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="baseVolumeName")
+    def base_volume_name(self) -> pulumi.Output[Optional[str]]:
         """
-        Set to `true` to start the network on host boot up.
-        If not specified `false` is assumed.
+        The name of the backing volume (CoW) to use
+        for this volume. Note well: when `base_volume_pool` is not specified the
+        volume is going to be searched inside of `pool`.
         """
-        return pulumi.get(self, "autostart")
+        return pulumi.get(self, "base_volume_name")
 
     @property
-    @pulumi.getter
-    def bridge(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="baseVolumePool")
+    def base_volume_pool(self) -> pulumi.Output[Optional[str]]:
         """
-        The bridge device defines the name of a bridge
-        device which will be used to construct the virtual network (when not provided,
-        it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
+        The name of the storage pool containing the
+        volume defined by `base_volume_name`.
         """
-        return pulumi.get(self, "bridge")
+        return pulumi.get(self, "base_volume_pool")
 
     @property
     @pulumi.getter
-    def dhcp(self) -> pulumi.Output['outputs.NetworkDhcp']:
-        return pulumi.get(self, "dhcp")
+    def format(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "format")
 
     @property
     @pulumi.getter
-    def dns(self) -> pulumi.Output['outputs.NetworkDns']:
-        """
-        configuration of DNS specific settings for the network
-        """
-        return pulumi.get(self, "dns")
-
-    @property
-    @pulumi.getter(name="dnsmasqOptions")
-    def dnsmasq_options(self) -> pulumi.Output[Optional['outputs.NetworkDnsmasqOptions']]:
-        return pulumi.get(self, "dnsmasq_options")
-
-    @property
-    @pulumi.getter
-    def domain(self) -> pulumi.Output[Optional[str]]:
-        """
-        The domain used by the DNS server.
-        """
-        return pulumi.get(self, "domain")
-
-    @property
-    @pulumi.getter
-    def mode(self) -> pulumi.Output[Optional[str]]:
+    def name(self) -> pulumi.Output[str]:
         """
-        One of:
+        A unique name for the resource, required by libvirt.
+        Changing this forces a new resource to be created.
         """
-        return pulumi.get(self, "mode")
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def mtu(self) -> pulumi.Output[Optional[int]]:
+    def pool(self) -> pulumi.Output[Optional[str]]:
         """
-        The MTU to set for the underlying network interfaces. When
-        not supplied, libvirt will use the default for the interface, usually 1500.
-        Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
+        The storage pool where the resource will be created.
+        If not given, the `default` storage pool will be used.
         """
-        return pulumi.get(self, "mtu")
+        return pulumi.get(self, "pool")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def size(self) -> pulumi.Output[int]:
         """
-        A unique name for the resource, required by libvirt.
-        Changing this forces a new resource to be created.
+        The size of the volume in bytes (if you don't like this,
+        help fix this issue.
+        If `source` is specified, `size` will be set to the source image file size.
+        `size` can be omitted if `source` is specified. `size` will then be set to the source image file size.
+        `size` can be omitted if `base_volume_id` or `base_volume_name` is specified. `size` will then be set to the base volume size.
+        If `size` is specified to be bigger than `base_volume_id` or `base_volume_name` size, you can use [cloudinit](https://cloudinit.readthedocs.io) if your OS supports it, with `CloudInitDisk` and the [growpart](https://cloudinit.readthedocs.io/en/latest/topics/modules.html#growpart) module to resize the partition.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def routes(self) -> pulumi.Output[Optional[Sequence['outputs.NetworkRoute']]]:
-        """
-        a list of static routes. A `cidr` and a `gateway` must
-        be provided. The `gateway` must be reachable via the bridge interface.
-        """
-        return pulumi.get(self, "routes")
+    def source(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
-    def xml(self) -> pulumi.Output[Optional['outputs.NetworkXml']]:
+    def xml(self) -> pulumi.Output[Optional['outputs.VolumeXml']]:
         return pulumi.get(self, "xml")
```

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1715337488
+Version: 0.5.0a1715709193
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1715337488/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.5.0a1715709193/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1715337488/pyproject.toml` & `pulumi_libvirt-0.5.0a1715709193/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_libvirt"
   description = "A Pulumi package for creating and managing libvirt cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "libvirt"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.5.0a1715337488"
+  version = "0.5.0a1715709193"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-libvirt"
 
 [build-system]
```

