# Comparing `tmp/iguana-0.1.1.tar.gz` & `tmp/iguana-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguana-0.1.1.tar", last modified: Wed May 15 20:43:47 2024, max compression
+gzip compressed data, was "iguana-0.1.2.tar", last modified: Wed May 15 20:49:57 2024, max compression
```

## Comparing `iguana-0.1.1.tar` & `iguana-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.1/LICENSE
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:43:47.971476 iguana-0.1.1/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.1/README.md
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/iguana/
--rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.1/iguana/__init__.py
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7668 2024-05-15 13:59:07.000000 iguana-0.1.1/iguana/iguana.py
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:43:47.971476 iguana-0.1.1/iguana.egg-info/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/SOURCES.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/dependency_links.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       39 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/entry_points.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/requires.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-15 20:43:47.000000 iguana-0.1.1/iguana.egg-info/top_level.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-15 20:43:47.971476 iguana-0.1.1/setup.cfg
--rw-r--r--   0 keksi     (1000) keksi     (1000)      761 2024-05-15 20:42:05.000000 iguana-0.1.1/setup.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:49:57.958752 iguana-0.1.2/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.2/LICENSE
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:49:57.958752 iguana-0.1.2/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.2/README.md
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:49:57.958752 iguana-0.1.2/iguana/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.2/iguana/__init__.py
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7959 2024-05-15 20:47:59.000000 iguana-0.1.2/iguana/iguana.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 20:49:57.958752 iguana-0.1.2/iguana.egg-info/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/SOURCES.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/dependency_links.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       46 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/entry_points.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/requires.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-15 20:49:57.000000 iguana-0.1.2/iguana.egg-info/top_level.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-15 20:49:57.958752 iguana-0.1.2/setup.cfg
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      768 2024-05-15 20:49:35.000000 iguana-0.1.2/setup.py
```

### Comparing `iguana-0.1.1/LICENSE` & `iguana-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iguana-0.1.1/PKG-INFO` & `iguana-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.1
+Version: 0.1.2
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.1/README.md` & `iguana-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iguana-0.1.1/iguana/iguana.py` & `iguana-0.1.2/iguana/iguana.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,25 @@
 │   python iguana.py -m port-scan --ip [IP address] : Scan open ports on IP.         │
 │   python iguana.py -m sniff --interface [Interface] : Sniff packets on interface.  │
 │   python iguana.py -m dns-gather --domain [Domain] : Gather DNS info for domain.   │
 │   python iguana.py -h or --help             : Show help message and exit.          │
 ╰────────────────────────────────────────────────────────────────────────────────────╯
 """)
 
+# iguana/iguana.py
+
+def main():
+    parser = argparse.ArgumentParser(description="Iguana Network Tools")
+    parser.add_argument('--example', help='Example argument')
+    args = parser.parse_args()
+    print(f"Example argument value: {args.example}")
+
+if __name__ == "__main__":
+    main()
+
 
 # Function to perform a basic network scan
 def scan_network(ip):
     print(f"Scanning network: {ip}")
     arp_request = ARP(pdst=ip)
     broadcast = Ether(dst="ff:ff:ff:ff:ff:ff")
     packet = broadcast / arp_request
```

### Comparing `iguana-0.1.1/iguana.egg-info/PKG-INFO` & `iguana-0.1.2/iguana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.1
+Version: 0.1.2
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.1/setup.py` & `iguana-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iguana',
-    version='0.1.1',
+    version='0.1.2',
     description='A network scanning tool for Kali Linux',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Uveis Smajli',
     author_email='smajliuveis@yahoo.com',
     url='https://github.com/uveissmjl/iguana',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'iguana=iguana:main',
+            'iguana=iguana.iguana:main',
         ],
     },
     install_requires=[
         'scapy',
         'dnspython',
     ],
     classifiers=[
```

