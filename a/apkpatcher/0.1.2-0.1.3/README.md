# Comparing `tmp/apkpatcher-0.1.2.tar.gz` & `tmp/apkpatcher-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-0.1.2.tar", last modified: Tue Apr  2 21:37:07 2024, max compression
+gzip compressed data, was "apkpatcher-0.1.3.tar", last modified: Wed May 15 10:54:34 2024, max compression
```

## Comparing `apkpatcher-0.1.2.tar` & `apkpatcher-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.659760 apkpatcher-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23045 2024-04-02 21:37:07.658760 apkpatcher-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 21:37:07.659760 apkpatcher-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.654760 apkpatcher-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.656760 apkpatcher-0.1.2/src/apkpatcher/
--rw-rw-rw-   0 root         (0) root         (0)    26650 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.658760 apkpatcher-0.1.2/src/apkpatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23045 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.960172 apkpatcher-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-05-15 10:54:34.959172 apkpatcher-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:54:34.960172 apkpatcher-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.956172 apkpatcher-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.957172 apkpatcher-0.1.3/src/apkpatcher/
+-rw-rw-rw-   0 root         (0) root         (0)    26510 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.959172 apkpatcher-0.1.3/src/apkpatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/top_level.txt
```

### Comparing `apkpatcher-0.1.2/LICENSE` & `apkpatcher-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.2/PKG-INFO` & `apkpatcher-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,15 @@
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.7
+Requires-Dist: pyaxml==0.0.8
 Requires-Dist: androguard==4.1.1
 
 # README
 
 
 ## GENERAL INFO
```

### Comparing `apkpatcher-0.1.2/README.md` & `apkpatcher-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.2/pyproject.toml` & `apkpatcher-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apkpatcher"
 dynamic = ["version", "readme"]
 dependencies = [
   'sty',
-  'pyaxml==0.0.7',
+  'pyaxml==0.0.8',
   'androguard==4.1.1',
 ]
 requires-python = ">=3.5"
 authors = [
   {name = "Benoit Forgette (MadSquirrel)", email = "benoit.forgette@ci-yow.com"},
 ]
 maintainers = [
```

### Comparing `apkpatcher-0.1.2/src/apkpatcher/__init__.py` & `apkpatcher-0.1.3/src/apkpatcher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,137 +66,124 @@
 #            CERTIFICATES                                                      #
 #                                                                              #
 ################################################################################
    
     def add_network_certificate(self, cert):
         self.network_certificates.append(cert)
 
-    def inject_custom_network_certificate(self):
-        if len(self.network_certificates) == 0:
-            return
-        res_path = os.path.join(self.final_dir, 'res')
-        xml_path = os.path.join(res_path, 'xml')
-        netsec_path = os.path.join(xml_path, 'network_security_config.xml')
+    def inject_custom_network_certificate(self, rsc, path_network : str):
+        netsec_path = os.path.join(self.final_dir, path_network)
+        ca_path = os.path.join(self.final_dir, "res/my_ca")
 
-        buf = """
+        ID = rsc.add_id_public(rsc.get_packages()[0],"raw", "network_security_config_ca", "res/my_ca")
+
+        buf = f"""
         <network-security-config>
             <base-config cleartextTrafficPermitted="true">
                 <trust-anchors>
                     <certificates src="system"/>
                     <certificates src="user"/>
-                    <certificates src="@raw/my_ca"/>
+                    <certificates src="@{hex(ID)[2:]}"/>
                 </trust-anchors>
             </base-config>
         </network-security-config>
         """
+
         root = ET.fromstring(buf)
         res_aml = pyaxml.axml.AXML()
         res_aml.from_xml(root)
         with open(netsec_path, "wb") as f:
             f.write(res_aml.pack())
 
-        os.makedirs(f"{res_path}/raw", exist_ok=True)
         for cert in self.network_certificates:
-            shutil.copyfile(cert, f"{res_path}/raw/my_ca")
+            shutil.copyfile(cert, ca_path)
         logging.info("Custom certificate was injected inside the apk")
+    
+    def create_security_config_xml(self, path_network : str):
+        netsec_path = os.path.join(self.final_dir, path_network)
+
+        buf = """
+        <network-security-config>
+            <base-config cleartextTrafficPermitted="true">
+                <trust-anchors>
+                    <certificates src="system"/>
+                    <certificates src="user"/>
+                </trust-anchors>
+            </base-config>
+        </network-security-config>
+        """
+        root = ET.fromstring(buf)
+        res_aml = pyaxml.axml.AXML()
+        res_aml.from_xml(root)
+        with open(netsec_path, "wb") as f:
+            f.write(res_aml.pack())
 
 
-    def enable_user_certificates(self):
-        #if not self.has_user_certificates_label():
-        self.inject_user_certificates_label()
+        logging.info('The network_security_config.xml file was created!')
+
 
-        self.create_security_config_xml()
+    def enable_user_certificates(self, rsc):
+        path_network = self.inject_user_certificates_label(rsc)
+        if path_network:
+            if self.network_certificates:
+                self.inject_custom_network_certificate(rsc, path_network)
+            else:
+                self.create_security_config_xml(path_network)
     
     def has_user_certificates_label(self):
         manifest_path = os.path.join(self.final_dir, 'AndroidManifest.xml')
 
         if not os.path.isfile(manifest_path):
             logging.error("Couldn't find the Manifest file. Something is wrong with the apk!")
             return False
 
         with open(manifest_path, 'r') as manifest_file:
             manifest_content = manifest_file.read()
             has_netsec_label = manifest_content.find('network_security_config') != -1
 
         return has_netsec_label
 
-    def inject_user_certificates_label(self):
+    def inject_user_certificates_label(self, rsc : pyaxml.ARSC):
         logging.info('Injecting Network Security label to accept user certificates...')
 
         manifest_path = os.path.join(self.final_dir, 'AndroidManifest.xml')
 
         if not os.path.isfile(manifest_path):
             logging.error("Couldn't find the Manifest file. Something is wrong with the apk!")
-            return False
+            return None
+        
+        with open(manifest_path, 'rb') as fp:
+            buf = fp.read()
 
 
-        with open(f"{self.final_dir}/resources.arsc", "rb") as fp:
-            rsc = axml.ARSCParser(fp.read())
-            package = rsc.get_packages_names()[0]
-            buf = rsc.get_public_resources(package)
-            root = ET.fromstring(buf)
-            e = root.findall("./public/[@name='network_security_config']")
-            ID = None
-            if len(e) > 0:
-                ID = e[0].get('id')
-            else:
-                logging.error("Could not inject certificate for the moment")
-                return 1
 
-        with open(manifest_path, 'rb') as fp:
-            buf = fp.read()
+            ID = rsc.get_id_public(rsc.get_packages()[0], "xml", "network_security_config")
+            if not ID:
+                path_network = "res/network_security_config.xml"
+                ID = rsc.add_id_public(rsc.get_packages()[0],"xml", "network_security_config", path_network)
+            else:
+                ID, path_network = ID
+                path_network = pyaxml.StringBlocks(proto=rsc.proto.stringblocks).decode_str(path_network)
 
+            
             aml = axml.AXMLPrinter(buf)
             etree = aml.root
             application = etree.findall("./application")[0]
-            application.attrib["{http://schemas.android.com/apk/res/android}networkSecurityConfig"] = f"@{ID[2:]}"
+            application.attrib["{http://schemas.android.com/apk/res/android}networkSecurityConfig"] = f"@{hex(ID)[2:]}"
             res_aml = pyaxml.axml.AXML()
             res_aml.from_xml(etree)
 
-        with open(manifest_path, 'wb') as fp:
-            fp.write(res_aml.pack())
-
-        logging.info('The Network Security label was added!')
-
-    def create_security_config_xml(self):
-        res_path = os.path.join(self.final_dir, 'res')
-
-        # Probably this if statement will never be reached
-        if not os.path.isdir(res_path):
-            logging.info('Resources path not found. Creating one...')
-
-            os.makedirs(res_path)
-
-        xml_path = os.path.join(res_path, 'xml')
-
-        if not os.path.isdir(xml_path):
-            logging.info('res/xml path not found. Creating one...')
-
-            os.makedirs(xml_path)
-
-        netsec_path = os.path.join(xml_path, 'network_security_config.xml')
-
-        buf = """
-        <network-security-config>
-            <base-config cleartextTrafficPermitted="true">
-                <trust-anchors>
-                    <certificates src="system"/>
-                    <certificates src="user"/>
-                </trust-anchors>
-            </base-config>
-        </network-security-config>
-        """
-        root = ET.fromstring(buf)
-        res_aml = pyaxml.axml.AXML()
-        res_aml.from_xml(root)
-        with open(netsec_path, "wb") as f:
-            f.write(res_aml.pack())
+            with open(manifest_path, 'wb') as fp:
+                fp.write(res_aml.pack())
+    
+            logging.info('The Network Security label was added!')
 
+        return path_network
 
-        logging.info('The network_security_config.xml file was created!')
+    
 
 
 
 
 
 ################################################################################
 #                                                                              #
@@ -688,16 +675,21 @@
             has_internet_permission = self.has_permission(self.INTERNET_PERMISSION)
             if not has_internet_permission:
                 if not self.inject_permission_manifest(self.INTERNET_PERMISSION):
                     sys.exit(1)
 
             # add users certificate
             if user_certificate:
-                self.enable_user_certificates()
-                self.inject_custom_network_certificate()
+                with open(f"{self.final_dir}/resources.arsc", "r+b") as fp:
+                    rsc, _ = pyaxml.ARSC.from_axml(fp.read())
+                    self.enable_user_certificates(rsc)
+                    rsc.compute()
+                    fp.seek(0)
+                    fp.write(rsc.pack())
+
 
             # inject frida library
             self.entrypoint_class = self.get_entrypoint_class_name()
             self.entrypoint_smali_path = self.get_entrypoint_smali_path()
             if gadget_to_use:
                 self.insert_frida_loader()
             self.check_libextract()
```

### Comparing `apkpatcher-0.1.2/src/apkpatcher/cli.py` & `apkpatcher-0.1.3/src/apkpatcher/cli.py`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.2/src/apkpatcher.egg-info/PKG-INFO` & `apkpatcher-0.1.3/src/apkpatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,15 @@
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.7
+Requires-Dist: pyaxml==0.0.8
 Requires-Dist: androguard==4.1.1
 
 # README
 
 
 ## GENERAL INFO
```

