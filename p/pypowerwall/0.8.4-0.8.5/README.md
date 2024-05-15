# Comparing `tmp/pypowerwall-0.8.4-py2.py3-none-any.whl.zip` & `tmp/pypowerwall-0.8.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 62053 bytes, number of entries: 21
--rw-r--r--  2.0 unx    32843 b- defN 24-May-05 03:49 pypowerwall/__init__.py
--rw-r--r--  2.0 unx     5835 b- defN 24-Mar-31 06:45 pypowerwall/__main__.py
--rw-r--r--  2.0 unx     1889 b- defN 24-Mar-30 06:29 pypowerwall/aux.py
+Zip file size: 62071 bytes, number of entries: 21
+-rw-r--r--  2.0 unx    32843 b- defN 24-May-15 14:44 pypowerwall/__init__.py
+-rw-r--r--  2.0 unx     5835 b- defN 24-May-15 14:43 pypowerwall/__main__.py
+-rw-r--r--  2.0 unx     1889 b- defN 24-May-15 14:43 pypowerwall/aux.py
 -rw-r--r--  2.0 unx      133 b- defN 24-Mar-30 06:29 pypowerwall/exceptions.py
 -rw-r--r--  2.0 unx     2897 b- defN 24-Apr-04 04:31 pypowerwall/pypowerwall_base.py
 -rw-r--r--  2.0 unx     6718 b- defN 24-Mar-26 02:39 pypowerwall/scan.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/cloud/__init__.py
 -rw-r--r--  2.0 unx      638 b- defN 24-Mar-26 02:39 pypowerwall/cloud/decorators.py
 -rw-r--r--  2.0 unx      242 b- defN 24-Mar-30 06:29 pypowerwall/cloud/exceptions.py
 -rw-r--r--  2.0 unx    18733 b- defN 24-Mar-26 02:39 pypowerwall/cloud/mock_data.py
--rw-r--r--  2.0 unx    46292 b- defN 24-Apr-05 03:05 pypowerwall/cloud/pypowerwall_cloud.py
+-rw-r--r--  2.0 unx    46441 b- defN 24-May-15 14:44 pypowerwall/cloud/pypowerwall_cloud.py
 -rw-r--r--  2.0 unx     4355 b- defN 24-Mar-26 02:39 pypowerwall/cloud/stubs.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/local/__init__.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 02:39 pypowerwall/local/exceptions.py
--rw-r--r--  2.0 unx    20404 b- defN 24-Apr-13 03:48 pypowerwall/local/pypowerwall_local.py
+-rw-r--r--  2.0 unx    20404 b- defN 24-May-15 14:43 pypowerwall/local/pypowerwall_local.py
 -rw-r--r--  2.0 unx    71273 b- defN 24-Mar-26 02:39 pypowerwall/local/tesla_pb2.py
--rw-r--r--  2.0 unx     1066 b- defN 24-May-05 03:50 pypowerwall-0.8.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    41728 b- defN 24-May-05 03:50 pypowerwall-0.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-05 03:50 pypowerwall-0.8.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-05 03:50 pypowerwall-0.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1766 b- defN 24-May-05 03:50 pypowerwall-0.8.4.dist-info/RECORD
-21 files, 257026 bytes uncompressed, 59173 bytes compressed:  77.0%
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    41728 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1766 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/RECORD
+21 files, 257175 bytes uncompressed, 59191 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pypowerwall/local/pypowerwall_local.py
 Comment: 
 
 Filename: pypowerwall/local/tesla_pb2.py
 Comment: 
 
-Filename: pypowerwall-0.8.4.dist-info/LICENSE
+Filename: pypowerwall-0.8.5.dist-info/LICENSE
 Comment: 
 
-Filename: pypowerwall-0.8.4.dist-info/METADATA
+Filename: pypowerwall-0.8.5.dist-info/METADATA
 Comment: 
 
-Filename: pypowerwall-0.8.4.dist-info/WHEEL
+Filename: pypowerwall-0.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: pypowerwall-0.8.4.dist-info/top_level.txt
+Filename: pypowerwall-0.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pypowerwall-0.8.4.dist-info/RECORD
+Filename: pypowerwall-0.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pypowerwall/__init__.py

```diff
@@ -86,15 +86,15 @@
 from pypowerwall.exceptions import PyPowerwallInvalidConfigurationParameter, InvalidBatteryReserveLevelException
 from pypowerwall.cloud.pypowerwall_cloud import PyPowerwallCloud
 from pypowerwall.local.pypowerwall_local import PyPowerwallLocal
 from pypowerwall.pypowerwall_base import parse_version, PyPowerwallBase
 
 urllib3.disable_warnings()  # Disable SSL warnings
 
-version_tuple = (0, 8, 4)
+version_tuple = (0, 8, 5)
 version = __version__ = '%d.%d.%d' % version_tuple
 __author__ = 'jasonacox'
 
 log = logging.getLogger(__name__)
 log.debug('%s version %s', __name__, __version__)
 log.debug('Python %s on %s', sys.version, sys.platform)
```

## pypowerwall/cloud/pypowerwall_cloud.py

```diff
@@ -173,16 +173,17 @@
                     found = True
                     break
             if not found:
                 log.error("Site %r not found for %s" % (self.siteid, self.email))
                 return False
         # Set site
         self.site = sites[self.siteindex]
+        site_name = sites[self.siteindex].get('site_name') or 'Unknown'
         log.debug(f"Connected to Tesla Cloud - Site {self.siteid} "
-                  f"({sites[self.siteindex]['site_name']}) for {self.email}")
+                  f"({site_name}) for {self.email}")
         return True
 
     # Function to map Powerwall API to Tesla Cloud Data
     def poll(self, api: str, force: bool = False,
              recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
         """
         Map Powerwall API to Tesla Cloud Data
@@ -261,15 +262,16 @@
             return False
         # Set siteindex - Find siteid in sites
         for idx, site in enumerate(sites):
             if site['energy_site_id'] == siteid:
                 self.siteid = siteid
                 self.siteindex = idx
                 self.site = sites[self.siteindex]
-                log.debug(f"Changed site to {self.siteid} ({sites[self.siteindex]['site_name']}) for {self.email}")
+                site_name = sites[self.siteindex].get('site_name') or 'Unknown'
+                log.debug(f"Changed site to {self.siteid} ({site_name}) for {self.email}")
                 return True
         log.error("Site %d not found for %s" % (siteid, self.email))
         return False
 
     # Functions to get data from Tesla Cloud
 
     def _site_api(self, name: str, ttl: int, force: bool, **kwargs):
@@ -969,15 +971,16 @@
                 else:
                     print(f"  - Invalid: {response} is not a valid site number")
             else:
                 break
         # Lookup the site id
         self.siteid = siteids[self.siteindex]
         self.site = sites[self.siteindex]
-        print("\nSelected site %d - %s (%s)" % (self.siteindex + 1, sites[self.siteindex]["site_name"], self.siteid))
+        site_name = sites[self.siteindex].get('site_name') or 'Unknown'
+        print("\nSelected site %d - %s (%s)" % (self.siteindex + 1, site_name, self.siteid))
         # Write the site id to the sitefile
         with open(self.sitefile, "w") as f:
             f.write(str(self.siteid))
 
         return True
 
     def close_session(self):
```

## Comparing `pypowerwall-0.8.4.dist-info/LICENSE` & `pypowerwall-0.8.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pypowerwall-0.8.4.dist-info/METADATA` & `pypowerwall-0.8.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypowerwall
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python module to access Tesla Energy Gateway for Powerwall and solar power data
 Home-page: https://github.com/jasonacox/pypowerwall
 Author: Jason Cox
 Author-email: jason@jasonacox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pypowerwall-0.8.4.dist-info/RECORD` & `pypowerwall-0.8.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-pypowerwall/__init__.py,sha256=gg3HnUJ44_GR0yI9KGvRIFypDLZ-EgwcBuJrRG80zzs,32843
+pypowerwall/__init__.py,sha256=zptASN1StYU71e9z9hSviBxeKMxq4dh0mmxNWabbXIk,32843
 pypowerwall/__main__.py,sha256=yDDWrUHvdk_jy5JUOqHYWNgGyTsBaL9j8DqQQtoE080,5835
 pypowerwall/aux.py,sha256=9VR4d4q163AdQQ4ELHLUYEH-RDOr-490cNZiGZFXlXM,1889
 pypowerwall/exceptions.py,sha256=D2TxwF42_quXoVr7CSQ1ifhSms_eHBJnFwy9l-bdtB0,133
 pypowerwall/pypowerwall_base.py,sha256=HKTNQQ59QfqtZtqYBe5rSkB8qyfZq9WPOwywzFvK7bs,2897
 pypowerwall/scan.py,sha256=DM9CxQLceu0bmyPaH8fNRdLgkS3oe4ata_78eObSNn8,6718
 pypowerwall/cloud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/cloud/decorators.py,sha256=aDwS9G-g7B8Md0dPPucHVd5mIdvrGKlz8typC-YHBCU,638
 pypowerwall/cloud/exceptions.py,sha256=tBSq0cUJvINmTMIcaq53iceSOmh-7hntqHIRCG6PEL0,242
 pypowerwall/cloud/mock_data.py,sha256=8CLdxyAhMY5I-tYsxUqcjGHth4T5NJkqvm-V6GUIAXM,18733
-pypowerwall/cloud/pypowerwall_cloud.py,sha256=hq8ZRuQHJxJvP_mNn4PQLz8iThtAzbumK0ddJ8J7_IQ,46292
+pypowerwall/cloud/pypowerwall_cloud.py,sha256=DYu7C1KTd8kyNy-tTSwML_wvvkypjRIOmNAPU5vU4EQ,46441
 pypowerwall/cloud/stubs.py,sha256=JQXgAONPzJSuK7_N55ODBOHAMpm_CfZ4YYmJFbJEWvg,4355
 pypowerwall/local/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/local/exceptions.py,sha256=JRm141HHbwKSkdeIWttOrniQTeehGJ3Zo6Fg9KH4Scc,92
 pypowerwall/local/pypowerwall_local.py,sha256=4DcdxnJT7e2SxDgYqXhWOlZUvM1bGEiGfGOEuyGfZ68,20404
 pypowerwall/local/tesla_pb2.py,sha256=l3faEX13xLWbWh6KRtbyCClK3zXpyN0LY6y3kM3Dpp8,71273
-pypowerwall-0.8.4.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
-pypowerwall-0.8.4.dist-info/METADATA,sha256=Rxga_phEq5tpCA1icIBK3W70KVqMPbM1VsrNjYva71w,41728
-pypowerwall-0.8.4.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-pypowerwall-0.8.4.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
-pypowerwall-0.8.4.dist-info/RECORD,,
+pypowerwall-0.8.5.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
+pypowerwall-0.8.5.dist-info/METADATA,sha256=oIAuIoazgdrAk028Qx19RqQMeGRgCc2hJheWgN5LRm4,41728
+pypowerwall-0.8.5.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+pypowerwall-0.8.5.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
+pypowerwall-0.8.5.dist-info/RECORD,,
```

