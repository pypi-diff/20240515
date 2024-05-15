# Comparing `tmp/cdnmon-0.3.1.tar.gz` & `tmp/cdnmon-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.3.1.tar", max compression
+gzip compressed data, was "cdnmon-0.4.0.tar", max compression
```

## Comparing `cdnmon-0.3.1.tar` & `cdnmon-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,55 @@
--rw-r--r--   0        0        0     1098 2024-05-13 15:07:35.205142 cdnmon-0.3.1/README.md
--rw-r--r--   0        0        0     1481 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/__init__.py
--rw-r--r--   0        0        0      404 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/config.py
--rw-r--r--   0        0        0       40 2024-05-13 15:07:35.205142 cdnmon-0.3.1/cdnmon/settings.py
--rw-r--r--   0        0        0      426 2024-05-13 15:07:35.205142 cdnmon-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 cdnmon-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-14 10:11:00.055964 cdnmon-0.4.0/README.md
+-rw-r--r--   0        0        0     1513 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/__init__.py
+-rw-r--r--   0        0        0     1535 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1813 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0     5259 2024-05-14 10:11:00.055964 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0      910 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0      626 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      509 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      531 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      498 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      437 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/belugacdn.py
+-rw-r--r--   0        0        0      467 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      442 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cdnvideo.py
+-rw-r--r--   0        0        0      442 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0     1218 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1408 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0      496 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/dnion.py
+-rw-r--r--   0        0        0      476 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      479 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgenext.py
+-rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     1676 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      486 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0      495 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1682 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0     1819 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/google.py
+-rw-r--r--   0        0        0     4153 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      436 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      478 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0      585 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/jd.py
+-rw-r--r--   0        0        0      469 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0      544 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      438 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      432 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/lumen.py
+-rw-r--r--   0        0        0     1659 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/maxcdn.py
+-rw-r--r--   0        0        0      440 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/medianova.py
+-rw-r--r--   0        0        0      493 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/microsoft.py
+-rw-r--r--   0        0        0      470 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0      445 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/tata_communications.py
+-rw-r--r--   0        0        0      836 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0      531 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0      468 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      436 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/verizon.py
+-rw-r--r--   0        0        0      474 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0      736 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      690 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/aws.py
+-rw-r--r--   0        0        0     1525 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-14 10:11:00.059965 cdnmon-0.4.0/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      435 2024-05-14 10:11:00.059965 cdnmon-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 cdnmon-0.4.0/PKG-INFO
```

### Comparing `cdnmon-0.3.1/README.md` & `cdnmon-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.3.1/PKG-INFO` & `cdnmon-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: ipy (>=1.1,<2.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 This project provides IP range data of multiple CDN vendors via a Python package named `cdnmon`.
```

