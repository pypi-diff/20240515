# Comparing `tmp/cdnmon-0.4.0.tar.gz` & `tmp/cdnmon-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.4.0.tar", max compression
+gzip compressed data, was "cdnmon-0.4.1.tar", max compression
```

## Comparing `cdnmon-0.4.0.tar` & `cdnmon-0.4.1.tar`

### file list

```diff
@@ -1,55 +1,54 @@
--rw-r--r--   0        0        0     1098 2024-05-14 10:11:00.055964 cdnmon-0.4.0/README.md
--rw-r--r--   0        0        0     1513 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/__init__.py
--rw-r--r--   0        0        0     1535 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/__init__.py
--rw-r--r--   0        0        0      487 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/advancedhosting.py
--rw-r--r--   0        0        0     1813 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/akamai.py
--rw-r--r--   0        0        0     5259 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_cdn.py
--rw-r--r--   0        0        0      910 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_dcdn.py
--rw-r--r--   0        0        0      626 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_waf.py
--rw-r--r--   0        0        0      509 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/asia_isp.py
--rw-r--r--   0        0        0      531 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/baidu.py
--rw-r--r--   0        0        0      498 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/baishan.py
--rw-r--r--   0        0        0      437 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/belugacdn.py
--rw-r--r--   0        0        0      467 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/bunny.py
--rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cachefly.py
--rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdn77.py
--rw-r--r--   0        0        0      442 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdnetworks.py
--rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdnvideo.py
--rw-r--r--   0        0        0      442 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/chinacache.py
--rw-r--r--   0        0        0     1218 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cloudflare.py
--rw-r--r--   0        0        0     1408 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cloudfront.py
--rw-r--r--   0        0        0      496 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/ctyun.py
--rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/dnion.py
--rw-r--r--   0        0        0      476 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/douyin.py
--rw-r--r--   0        0        0      479 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgecast.py
--rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgenext.py
--rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgio.py
--rw-r--r--   0        0        0     1676 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/fastly.py
--rw-r--r--   0        0        0      486 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/fastly_edge_compute.py
--rw-r--r--   0        0        0      495 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/frontdoor.py
--rw-r--r--   0        0        0     1682 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/gcore.py
--rw-r--r--   0        0        0     1819 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/google.py
--rw-r--r--   0        0        0     4153 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/huawei.py
--rw-r--r--   0        0        0      436 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/imperva.py
--rw-r--r--   0        0        0      478 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/incapsula.py
--rw-r--r--   0        0        0      585 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/jd.py
--rw-r--r--   0        0        0      469 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/keycdn.py
--rw-r--r--   0        0        0      544 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/kingsoft.py
--rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/leaseweb.py
--rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/lumen.py
--rw-r--r--   0        0        0     1659 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/maxcdn.py
--rw-r--r--   0        0        0      440 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/medianova.py
--rw-r--r--   0        0        0      493 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/microsoft.py
--rw-r--r--   0        0        0      470 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/qiniu.py
--rw-r--r--   0        0        0      445 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/tata_communications.py
--rw-r--r--   0        0        0      836 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/tencent.py
--rw-r--r--   0        0        0      531 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/ucloud.py
--rw-r--r--   0        0        0      468 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/upyun.py
--rw-r--r--   0        0        0      436 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/verizon.py
--rw-r--r--   0        0        0      474 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/volc.py
--rw-r--r--   0        0        0      736 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/wangsu.py
--rw-r--r--   0        0        0      690 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/aws.py
--rw-r--r--   0        0        0     1525 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/bgpview.py
--rw-r--r--   0        0        0      389 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/cidr.py
--rw-r--r--   0        0        0      435 2024-05-14 10:11:00.059965 cdnmon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 cdnmon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-15 01:02:08.908555 cdnmon-0.4.1/README.md
+-rw-r--r--   0        0        0     1610 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/__init__.py
+-rw-r--r--   0        0        0     5532 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1766 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0     7896 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0      980 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0      543 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      302 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      390 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      342 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      205 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/beluga.py
+-rw-r--r--   0        0        0      292 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      217 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cdnvideo.py
+-rw-r--r--   0        0        0      217 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0     1087 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1283 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0      359 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/dnion.py
+-rw-r--r--   0        0        0      324 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      307 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      211 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgenext.py
+-rw-r--r--   0        0        0      202 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     1549 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      309 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0      350 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1481 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0     1620 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/google.py
+-rw-r--r--   0        0        0     5969 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      208 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      307 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0      470 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/jingdong.py
+-rw-r--r--   0        0        0      295 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0      375 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      227 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      218 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/lumen.py
+-rw-r--r--   0        0        0     1438 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/maxcdn.py
+-rw-r--r--   0        0        0      230 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/medianova.py
+-rw-r--r--   0        0        0      311 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0      230 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/tata_communications.py
+-rw-r--r--   0        0        0      883 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0      407 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0      328 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      224 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/verizon.py
+-rw-r--r--   0        0        0      318 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0      748 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      691 2024-05-15 01:02:08.908555 cdnmon-0.4.1/cdnmon/util/aws.py
+-rw-r--r--   0        0        0      897 2024-05-15 01:02:08.912555 cdnmon-0.4.1/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-15 01:02:08.912555 cdnmon-0.4.1/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      436 2024-05-15 01:02:08.912555 cdnmon-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 cdnmon-0.4.1/PKG-INFO
```

### Comparing `cdnmon-0.4.0/README.md` & `cdnmon-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.4.0/cdnmon/__init__.py` & `cdnmon-0.4.1/cdnmon/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import coloredlogs
+import functools
+import glob
 import logging
+import os
+
+import coloredlogs
 import requests
 import yaml
-import glob
-import os
-import functools
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level="DEBUG", logger=logger)
 
 
 class CDN:
     def __init__(self, name):
         self._data = self._fetch_cdn_data(name)
         self.name = self._data["name"]
         self.cname_suffixes = self._data["cname_suffixes"] if "cname_suffixes" in self._data.keys() else []
         self.asn_patterns = self._data["asn_patterns"] if "asn_patterns" in self._data.keys() else []
         self.ipv4_prefixes = self._data["ipv4_prefixes"] if "ipv4_prefixes" in self._data.keys() else []
         self.ipv6_prefixes = self._data["ipv6_prefixes"] if "ipv6_prefixes" in self._data.keys() else []
+        self.updated_at = self._data["updated_at"] if "updated_at" in self._data.keys() else ""
 
     @staticmethod
     @functools.lru_cache(maxsize=None)
     def _fetch_cdn_data(name):
         url = f"https://cdnmon.vercel.app/{name}.yaml"
         response = requests.get(url)
         if response.status_code != 200:
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/akamai.py` & `cdnmon-0.4.1/cdnmon/model/cdn/akamai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CNAMEPattern
+from cdnmon.model.cdn import CommonCDN
 from cdnmon.util.cidr import deduplicate_networks
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "akamai"
-        self.ipv4_url = "https://techdocs.akamai.com/property-manager/pdfs/akamai_ipv4_ipv6_CIDRs-txt.zip"
-        self.ipv6_url = self.ipv4_url
-        self.asn_patterns = ["akamai"]
-        self.cname_suffixes = [
-            ".edgesuite.net",
-            ".edgekey.net",
-            ".akamaized.net",
-            ".akadns.net",
-            ".akamai.net",
-        ]
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class AkamaiCIDR(CIDR):
+    ipv4_url: str = "https://techdocs.akamai.com/property-manager/pdfs/akamai_ipv4_ipv6_CIDRs-txt.zip"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
         """
         [1] https://techdocs.akamai.com/property-mgr/docs/origin-ip-access-control
         """
-        import requests
         import zipfile
         import io
 
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/107.0.0.0 Safari/537.36 "
-        }
-        content = requests.get(self.ipv4_url, headers=headers).content
+        content = self.http_get(AkamaiCIDR.ipv4_url).content
         z = zipfile.ZipFile(io.BytesIO(content), mode="r")
         return {
             "ipv4": z.read("akamai_ipv4_CIDRs.txt").decode("utf-8"),
             "ipv6": z.read("akamai_ipv6_CIDRs.txt").decode("utf-8"),
         }
 
-    def transform(self, response):
+    def transform(self, response: dict):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
+
+
+CDN = CommonCDN(
+    name="akamai",
+    asn_patterns=["akamai"],
+    cname_suffixes=[
+        CNAMEPattern(suffix=".edgesuite.net", pattern=r"${domain}.edgesuite.net"),
+        CNAMEPattern(suffix=".edgekey.net", pattern=r"${domain}.edgekey.net"),
+        CNAMEPattern(suffix="-v1.akamaized.net", pattern=r"${domain}-v1.akamaized.net"),
+        CNAMEPattern(suffix="-v1.edgekey.net", pattern=r"${domain}-v1.edgekey.net"),
+        CNAMEPattern(suffix=".akadns.net"),
+        CNAMEPattern(suffix=".akamai.net"),
+    ],
+    cidr=AkamaiCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/cloudflare.py` & `cdnmon-0.4.1/cdnmon/model/cdn/cloudfront.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CNAMEPattern
+from cdnmon.model.cdn import CommonCDN
+from cdnmon.util.aws import get_ip_range_of_aws
 from cdnmon.util.cidr import deduplicate_networks
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "cloudflare"
-        self.ipv4_url = "https://www.cloudflare.com/ips-v4"
-        self.ipv6_url = "https://www.cloudflare.com/ips-v6"
-        self.asn_patterns = [
-            "cloudflare",
-        ]
-        self.cname_suffixes = [
-            ".cdn.cloudflare.net",
-        ]
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class CloudFrontCIDR(CIDR):
+    ipv4_url: str = "https://ip-ranges.amazonaws.com/ip-ranges.json"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
-        import requests
-
+        """
+        [1] https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html
+        """
+        ipv4_networks, ipv6_networks = get_ip_range_of_aws("CLOUDFRONT")
         return {
-            "ipv4": requests.get(self.ipv4_url).text,
-            "ipv6": requests.get(self.ipv6_url).text,
+            "ipv4": "\n".join(ipv4_networks),
+            "ipv6": "\n".join(ipv6_networks),
         }
 
     def transform(self, response):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
+
+
+CDN = CommonCDN(
+    name="cloudfront",
+    asn_patterns=["cloudfront", "amazon"],
+    cname_suffixes=[
+        CNAMEPattern(suffix=".cloudfront.net"),
+    ],
+    cidr=CloudFrontCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/cloudfront.py` & `cdnmon-0.4.1/cdnmon/model/cdn/google.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,50 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CommonCDN
 from cdnmon.util.cidr import deduplicate_networks
-from cdnmon.util.aws import get_ip_range_of_aws
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "cloudfront"
-        self.ipv4_url = "https://ip-ranges.amazonaws.com/ip-ranges.json"
-        self.ipv6_url = self.ipv4_url
-        self.asn_patterns = [
-            "cloudfront",
-            "amazon",
-        ]
-        self.cname_suffixes = [
-            ".cloudfront.net",
-        ]
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class GoogleCIDR(CIDR):
+    ipv4_url: str = "https://www.gstatic.com/ipranges/cloud.json"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
         """
-        [1] https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html
+        [1] https://support.google.com/a/answer/10026322
+        [2] https://www.gstatic.com/ipranges/goog.json
+        [3] https://www.gstatic.com/ipranges/cloud.json
         """
-        ipv4_networks, ipv6_networks = get_ip_range_of_aws("CLOUDFRONT")
+        import ipaddress
+
+        data = self.http_get(self.ipv4_url).json()
+
+        ipv4_networks = []
+        ipv6_networks = []
+
+        prefixes = data["prefixes"]
+        for prefix in prefixes:
+            if "ipv4Prefix" in prefix:
+                ipv4_networks.append(str(ipaddress.IPv4Network(prefix.get("ipv4Prefix"), strict=False)))
+
+            if "ipv6Prefix" in prefix:
+                ipv6_networks.append(str(ipaddress.IPv6Network(prefix.get("ipv6Prefix"), strict=False)))
+
         return {
             "ipv4": "\n".join(ipv4_networks),
             "ipv6": "\n".join(ipv6_networks),
         }
 
     def transform(self, response):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
+
+
+CDN = CommonCDN(
+    name="google",
+    asn_patterns=["google"],
+    cname_suffixes=[],
+    cidr=GoogleCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/fastly.py` & `cdnmon-0.4.1/cdnmon/model/cdn/fastly.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CNAMEPattern
+from cdnmon.model.cdn import CommonCDN
 from cdnmon.util.cidr import deduplicate_networks
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "fastly"
-        self.ipv4_url = "https://api.fastly.com/public-ip-list"
-        self.ipv6_url = self.ipv4_url
-        self.asn_patterns = [
-            "fastly",
-        ]
-        self.cname_suffixes = [
-            ".fastly.net",
-            ".fastlylb.net",
-        ]
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class FastlyCIDR(CIDR):
+    ipv4_url: str = "https://api.fastly.com/public-ip-list"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
         """
         [1] https://api.fastly.com/public-ip-list
         """
-        import requests
         import ipaddress
 
-        data = requests.get(self.ipv4_url).json()
+        data = self.http_get(self.ipv4_url).json()
 
         ipv4_networks = []
         for ipv4_prefix in data["addresses"]:
             ipv4_networks.append(str(ipaddress.IPv4Network(ipv4_prefix, strict=False)))
 
         ipv6_networks = []
         for ipv6_prefix in data["ipv6_addresses"]:
@@ -42,7 +32,18 @@
     def transform(self, response):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
+
+
+CDN = CommonCDN(
+    name="fastly",
+    asn_patterns=["fastly"],
+    cname_suffixes=[
+        CNAMEPattern(suffix=".fastly.net"),
+        CNAMEPattern(suffix=".fastlylb.net"),
+    ],
+    cidr=FastlyCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/gcore.py` & `cdnmon-0.4.1/cdnmon/model/cdn/gcore.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CommonCDN
 from cdnmon.util.cidr import deduplicate_networks
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "gcore"
-        self.ipv4_url = "https://api.gcore.com/cdn/public-ip-list"
-        self.ipv6_url = self.ipv4_url
-        self.asn_patterns = [
-            "gcore",
-        ]
-        self.cname_suffixes = []
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class GCoreCIDR(CIDR):
+    ipv4_url: str = "https://api.gcore.com/cdn/public-ip-list"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
         """
         [1] https://apidocs.gcore.com/cdn#tag/IP-Addresses-List
         [2] https://api.gcorelabs.com/cdn/public-net-list
         """
-        import requests
         import ipaddress
 
-        data = requests.get(self.ipv4_url).json()
+        data = self.http_get(self.ipv4_url).json()
 
         ipv4_networks = []
         for ipv4_prefix in data["addresses"]:
             ipv4_networks.append(str(ipaddress.IPv4Network(ipv4_prefix, strict=False)))
 
         ipv6_networks = []
         for ipv6_prefix in data["addresses_v6"]:
@@ -40,7 +32,15 @@
     def transform(self, response):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
+
+
+CDN = CommonCDN(
+    name="gcore",
+    asn_patterns=["gcore"],
+    cname_suffixes=[],
+    cidr=GCoreCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/model/cdn/maxcdn.py` & `cdnmon-0.4.1/cdnmon/model/cdn/maxcdn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,41 @@
-from cdnmon.model.cdn import AbstractCDN
+from cdnmon.model.cdn import CIDR
+from cdnmon.model.cdn import CNAMEPattern
+from cdnmon.model.cdn import CommonCDN
 from cdnmon.util.cidr import deduplicate_networks
 
 
-class CDN(AbstractCDN):
-    def __init__(self):
-        self.abbreviation = "maxcdn"
-        self.ipv4_url = "https://support.maxcdn.com/hc/en-us/article_attachments/360051920551/maxcdn_ips.txt"
-        self.ipv6_url = self.ipv4_url
-        self.asn_patterns = [
-            "maxcdn",
-        ]
-        self.cname_suffixes = [
-            ".netdna-cdn.com",
-            ".netdna-ssl.com",
-            ".netdna.com",
-        ]
-        self.ipv4_prefixes = self.transform(self.extract())["ipv4_prefixes"]
-        self.ipv6_prefixes = self.transform(self.extract())["ipv6_prefixes"]
+class MaxCDNCIDR(CIDR):
+    ipv4_url: str = "https://support.maxcdn.com/hc/en-us/article_attachments/360051920551/maxcdn_ips.txt"
+    ipv6_url: str = ipv4_url
 
     def extract(self):
         """
         [1] https://support.maxcdn.com/one/tutorial/ip-blocks/
         [2] https://support.maxcdn.com/one/assets/ips.txt (302 Redirected to [3])
         [3] https://support.maxcdn.com/hc/en-us/article_attachments/360051920551/maxcdn_ips.txt
         """
-        import requests
-
-        text = requests.get(self.ipv4_url).text
+        text = self.http_get(self.ipv4_url).text
         return {
             "ipv4": text,
             "ipv6": text,
         }
 
     def transform(self, response):
         ipv4_networks = [line.strip() for line in response["ipv4"].split("\n") if line.strip() != ""]
         ipv6_networks = [line.strip() for line in response["ipv6"].split("\n") if line.strip() != ""]
         return {
             "ipv4_prefixes": deduplicate_networks(ipv4_networks, filter_version=4),
             "ipv6_prefixes": deduplicate_networks(ipv6_networks, filter_version=6),
         }
 
 
-def main():
-    cdn = CDN()
-    print(cdn.transform(cdn.extract()))
-
-
-if __name__ == "__main__":
-    main()
+CDN = CommonCDN(
+    name="maxcdn",
+    asn_patterns=["maxcdn"],
+    cname_suffixes=[
+        CNAMEPattern(suffix=".netdna-cdn.com"),
+        CNAMEPattern(suffix=".netdna-ssl.com"),
+        CNAMEPattern(suffix=".netdna.com"),
+    ],
+    cidr=MaxCDNCIDR(),
+)
```

### Comparing `cdnmon-0.4.0/cdnmon/util/aws.py` & `cdnmon-0.4.1/cdnmon/util/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ipaddress
+
 import requests
 
 
 def get_ip_range_of_aws(pattern):
     data = requests.get("https://ip-ranges.amazonaws.com/ip-ranges.json").json()
 
     ipv4_networks = []
```

### Comparing `cdnmon-0.4.0/PKG-INFO` & `cdnmon-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: ipy (>=1.1,<2.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

