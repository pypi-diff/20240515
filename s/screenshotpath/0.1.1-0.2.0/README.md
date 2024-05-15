# Comparing `tmp/screenshotpath-0.1.1.tar.gz` & `tmp/screenshotpath-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenshotpath-0.1.1.tar", last modified: Wed May 15 08:04:48 2024, max compression
+gzip compressed data, was "screenshotpath-0.2.0.tar", last modified: Wed May 15 10:01:10 2024, max compression
```

## Comparing `screenshotpath-0.1.1.tar` & `screenshotpath-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 08:04:48.264297 screenshotpath-0.1.1/
--rw-r--r--   0 isayamin   (501) staff       (20)     1078 2024-05-15 07:19:13.000000 screenshotpath-0.1.1/LICENSE
--rw-r--r--   0 isayamin   (501) staff       (20)      455 2024-05-15 08:04:48.264137 screenshotpath-0.1.1/PKG-INFO
--rw-r--r--   0 isayamin   (501) staff       (20)      114 2024-05-15 07:19:13.000000 screenshotpath-0.1.1/README.md
-drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 08:04:48.262598 screenshotpath-0.1.1/screenshotpath/
--rw-r--r--   0 isayamin   (501) staff       (20)        0 2024-05-15 07:19:13.000000 screenshotpath-0.1.1/screenshotpath/__init__.py
--rw-r--r--   0 isayamin   (501) staff       (20)     1717 2024-05-15 07:19:13.000000 screenshotpath-0.1.1/screenshotpath/screenshotpath.py
-drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 08:04:48.263899 screenshotpath-0.1.1/screenshotpath.egg-info/
--rw-r--r--   0 isayamin   (501) staff       (20)      455 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/PKG-INFO
--rw-r--r--   0 isayamin   (501) staff       (20)      316 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/SOURCES.txt
--rw-r--r--   0 isayamin   (501) staff       (20)        1 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/dependency_links.txt
--rw-r--r--   0 isayamin   (501) staff       (20)       71 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/entry_points.txt
--rw-r--r--   0 isayamin   (501) staff       (20)        9 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/requires.txt
--rw-r--r--   0 isayamin   (501) staff       (20)       15 2024-05-15 08:04:48.000000 screenshotpath-0.1.1/screenshotpath.egg-info/top_level.txt
--rw-r--r--   0 isayamin   (501) staff       (20)       38 2024-05-15 08:04:48.264351 screenshotpath-0.1.1/setup.cfg
--rw-r--r--   0 isayamin   (501) staff       (20)      616 2024-05-15 08:04:35.000000 screenshotpath-0.1.1/setup.py
+drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 10:01:10.472715 screenshotpath-0.2.0/
+-rw-r--r--   0 isayamin   (501) staff       (20)     1078 2024-05-15 07:19:13.000000 screenshotpath-0.2.0/LICENSE
+-rw-r--r--   0 isayamin   (501) staff       (20)      658 2024-05-15 10:01:10.472565 screenshotpath-0.2.0/PKG-INFO
+-rw-r--r--   0 isayamin   (501) staff       (20)      317 2024-05-15 09:58:16.000000 screenshotpath-0.2.0/README.md
+drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 10:01:10.471416 screenshotpath-0.2.0/screenshotpath/
+-rw-r--r--   0 isayamin   (501) staff       (20)        0 2024-05-15 07:19:13.000000 screenshotpath-0.2.0/screenshotpath/__init__.py
+-rw-r--r--   0 isayamin   (501) staff       (20)     2821 2024-05-15 09:54:33.000000 screenshotpath-0.2.0/screenshotpath/screenshotpath.py
+drwxr-xr-x   0 isayamin   (501) staff       (20)        0 2024-05-15 10:01:10.472361 screenshotpath-0.2.0/screenshotpath.egg-info/
+-rw-r--r--   0 isayamin   (501) staff       (20)      658 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/PKG-INFO
+-rw-r--r--   0 isayamin   (501) staff       (20)      316 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/SOURCES.txt
+-rw-r--r--   0 isayamin   (501) staff       (20)        1 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/dependency_links.txt
+-rw-r--r--   0 isayamin   (501) staff       (20)       71 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/entry_points.txt
+-rw-r--r--   0 isayamin   (501) staff       (20)        9 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/requires.txt
+-rw-r--r--   0 isayamin   (501) staff       (20)       15 2024-05-15 10:01:10.000000 screenshotpath-0.2.0/screenshotpath.egg-info/top_level.txt
+-rw-r--r--   0 isayamin   (501) staff       (20)       38 2024-05-15 10:01:10.472770 screenshotpath-0.2.0/setup.cfg
+-rw-r--r--   0 isayamin   (501) staff       (20)      616 2024-05-15 10:00:01.000000 screenshotpath-0.2.0/setup.py
```

### Comparing `screenshotpath-0.1.1/LICENSE` & `screenshotpath-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenshotpath-0.1.1/screenshotpath/screenshotpath.py` & `screenshotpath-0.2.0/screenshotpath/screenshotpath.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 #!/usr/bin/env python3
 import argparse
 import subprocess
 import os
 
 def main():
+    """
+    usage: screenshot_utility.py [-h] [--get] [--set NEW_LOCATION]
+
+    optional arguments:
+    -h, --help           show this help message and exit
+    --get                Retrieve the current screenshot location
+    --set NEW_LOCATION   Set a new screenshot location
+    """
+
     parser = argparse.ArgumentParser(description="Change macOS screenshot path.")
-    # Required:
-    requiredNamed = parser.add_argument_group('required named arguments')
-    requiredNamed.add_argument('location', 
-                               help="the absolute path to your screenshot location (will be prompted to create directory if path not found)")
+    parser.add_argument("--get", action="store_true", help="Retrieve the current screenshot location")
+    parser.add_argument('--set', help="Set a new screenshot location based on the absolute path provided.")
 
     args = parser.parse_args()
     # Runs the program
-    change_screenshot_location(args.location)
+    if args.get:
+        screenshot_location = get_screenshot_location()
+        if screenshot_location:
+            print("Current screenshots directory: ", screenshot_location)
+    elif args.set:
+        change_screenshot_location(args.location)
+    else:
+        print("No action specified. Use --get to retrieve the current screenshot location or --set to set a new location.")
+
+def get_screenshot_location():
+    try:
+        # Run the defaults command to get the screenshot location
+        result = subprocess.run(["defaults", "read", "com.apple.screencapture", "location"],
+                                capture_output=True, text=True, check=True)
+        
+        # Extract the path from the command output
+        location_path = result.stdout.strip()
+        
+        return location_path
+    except subprocess.CalledProcessError:
+        print("Error: Unable to retrieve screenshot location.")
+        return None
 
 def change_screenshot_location(new_path):
     # Check if the directory exists
     if not os.path.exists(new_path):
         # Ask the user if they want to create the directory
         user_input = input(f"The directory {new_path} does not exist. Do you want to create it? (y/[N]): ")
         if user_input.lower() != 'y':
```

### Comparing `screenshotpath-0.1.1/setup.py` & `screenshotpath-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='screenshotpath',
-    version='0.1.1',
+    version='0.2.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'screenshotpath=screenshotpath.screenshotpath:main',
         ],
     },
     install_requires=[
```

