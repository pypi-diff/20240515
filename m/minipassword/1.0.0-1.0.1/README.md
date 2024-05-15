# Comparing `tmp/minipassword-1.0.0.tar.gz` & `tmp/minipassword-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minipassword-1.0.0.tar", last modified: Mon May 13 06:23:02 2024, max compression
+gzip compressed data, was "minipassword-1.0.1.tar", last modified: Wed May 15 07:05:23 2024, max compression
```

## Comparing `minipassword-1.0.0.tar` & `minipassword-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-13 06:23:02.168518 minipassword-1.0.0/
--rw-r--r--   0 Alan       (501) staff       (20)     1063 2024-04-18 07:30:55.000000 minipassword-1.0.0/LICENSE
--rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-13 06:23:02.168305 minipassword-1.0.0/PKG-INFO
--rw-r--r--   0 Alan       (501) staff       (20)     3871 2024-05-13 06:18:57.000000 minipassword-1.0.0/README.md
--rw-r--r--   0 Alan       (501) staff       (20)       84 2022-04-22 08:08:10.000000 minipassword-1.0.0/pyproject.toml
--rw-r--r--   0 Alan       (501) staff       (20)       38 2024-05-13 06:23:02.168563 minipassword-1.0.0/setup.cfg
--rw-r--r--   0 Alan       (501) staff       (20)     1004 2024-05-11 10:52:48.000000 minipassword-1.0.0/setup.py
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-13 06:23:02.164585 minipassword-1.0.0/src/
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-13 06:23:02.165885 minipassword-1.0.0/src/minipassword/
--rw-r--r--   0 Alan       (501) staff       (20)        0 2024-05-10 03:57:36.000000 minipassword-1.0.0/src/minipassword/__init__.py
--rw-r--r--   0 Alan       (501) staff       (20)     7004 2024-05-13 04:10:22.000000 minipassword-1.0.0/src/minipassword/box.py
--rw-r--r--   0 Alan       (501) staff       (20)    12387 2024-05-13 04:27:45.000000 minipassword-1.0.0/src/minipassword/commands.py
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-13 06:23:02.168086 minipassword-1.0.0/src/minipassword.egg-info/
--rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-13 06:23:02.000000 minipassword-1.0.0/src/minipassword.egg-info/PKG-INFO
--rw-r--r--   0 Alan       (501) staff       (20)      420 2024-05-13 06:23:02.000000 minipassword-1.0.0/src/minipassword.egg-info/SOURCES.txt
--rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-13 06:23:02.000000 minipassword-1.0.0/src/minipassword.egg-info/dependency_links.txt
--rw-r--r--   0 Alan       (501) staff       (20)       62 2024-05-13 06:23:02.000000 minipassword-1.0.0/src/minipassword.egg-info/requires.txt
--rw-r--r--   0 Alan       (501) staff       (20)       13 2024-05-13 06:23:02.000000 minipassword-1.0.0/src/minipassword.egg-info/top_level.txt
--rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-10 04:26:04.000000 minipassword-1.0.0/src/minipassword.egg-info/zip-safe
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-13 06:23:02.167634 minipassword-1.0.0/tests/
--rw-r--r--   0 Alan       (501) staff       (20)      538 2024-05-10 06:27:51.000000 minipassword-1.0.0/tests/test_conf.py
--rw-r--r--   0 Alan       (501) staff       (20)     1722 2024-05-10 07:07:49.000000 minipassword-1.0.0/tests/test_manager.py
--rw-r--r--   0 Alan       (501) staff       (20)      114 2024-05-10 07:34:17.000000 minipassword-1.0.0/tests/testcommands.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.782304 minipassword-1.0.1/
+-rw-r--r--   0 Alan       (501) staff       (20)     1063 2024-04-18 07:30:55.000000 minipassword-1.0.1/LICENSE
+-rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-15 07:05:23.782111 minipassword-1.0.1/PKG-INFO
+-rw-r--r--   0 Alan       (501) staff       (20)     3871 2024-05-13 06:18:57.000000 minipassword-1.0.1/README.md
+-rw-r--r--   0 Alan       (501) staff       (20)       84 2022-04-22 08:08:10.000000 minipassword-1.0.1/pyproject.toml
+-rw-r--r--   0 Alan       (501) staff       (20)       38 2024-05-15 07:05:23.782361 minipassword-1.0.1/setup.cfg
+-rw-r--r--   0 Alan       (501) staff       (20)     1004 2024-05-15 06:59:16.000000 minipassword-1.0.1/setup.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.779612 minipassword-1.0.1/src/
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.780509 minipassword-1.0.1/src/minipassword/
+-rw-r--r--   0 Alan       (501) staff       (20)        0 2024-05-10 03:57:36.000000 minipassword-1.0.1/src/minipassword/__init__.py
+-rw-r--r--   0 Alan       (501) staff       (20)     7004 2024-05-13 04:10:22.000000 minipassword-1.0.1/src/minipassword/box.py
+-rw-r--r--   0 Alan       (501) staff       (20)    12705 2024-05-15 06:57:19.000000 minipassword-1.0.1/src/minipassword/commands.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.781895 minipassword-1.0.1/src/minipassword.egg-info/
+-rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/PKG-INFO
+-rw-r--r--   0 Alan       (501) staff       (20)      420 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/SOURCES.txt
+-rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/dependency_links.txt
+-rw-r--r--   0 Alan       (501) staff       (20)       62 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/requires.txt
+-rw-r--r--   0 Alan       (501) staff       (20)       13 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/top_level.txt
+-rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-10 04:26:04.000000 minipassword-1.0.1/src/minipassword.egg-info/zip-safe
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.781707 minipassword-1.0.1/tests/
+-rw-r--r--   0 Alan       (501) staff       (20)      538 2024-05-10 06:27:51.000000 minipassword-1.0.1/tests/test_conf.py
+-rw-r--r--   0 Alan       (501) staff       (20)     1722 2024-05-10 07:07:49.000000 minipassword-1.0.1/tests/test_manager.py
+-rw-r--r--   0 Alan       (501) staff       (20)      114 2024-05-10 07:34:17.000000 minipassword-1.0.1/tests/testcommands.py
```

### Comparing `minipassword-1.0.0/LICENSE` & `minipassword-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.0/PKG-INFO` & `minipassword-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipassword
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mini Password is a command-line password manager.
 Home-page: https://github.com/laonan/minipassword
 Author: Laonan
 Author-email: hello@laonan.net
 Project-URL: Bug Tracker, https://github.com/laonan/minipassword/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `minipassword-1.0.0/README.md` & `minipassword-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.0/setup.py` & `minipassword-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="minipassword",
-    version="1.0.0",
+    version="1.0.1",
     author="Laonan",
     author_email="hello@laonan.net",
     description="Mini Password is a command-line password manager.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/laonan/minipassword",  # github url
     project_urls={
```

### Comparing `minipassword-1.0.0/src/minipassword/box.py` & `minipassword-1.0.1/src/minipassword/box.py`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.0/src/minipassword/commands.py` & `minipassword-1.0.1/src/minipassword/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 import configparser
 import os
 import re
 import argparse
+import sys
+
 from simple_term_menu import TerminalMenu
 from cryptography.fernet import Fernet
 from .box import ConfUtils, PasswordManager
 
 
 parser = argparse.ArgumentParser(description='Mini Password is a command-line password manager.')
-parser.add_argument('-a', '--add', action='store_true', help='add a new password')
-parser.add_argument('-d', '--delete', action='store_true', help='delete a password')
-parser.add_argument('-u', '--update', action='store_true', help='update a password')
-parser.add_argument('-l', '--list-file', action='store_true', help='list database file and configuration file paths')
-parser.add_argument('-b', '--backup', action='store_true', help='backup the database file')
-parser.add_argument('-p', '--upload', action='store_true', help='upload the database file to a cloud service')
-parser.add_argument('-r', '--restore', action='store_true', help='restore the database file from cloud service')
-parser.add_argument('-api', '--api', action='store_true', help='set cloud API url and token')
-parser.add_argument('-dd', '--destroy', action='store_true', help='destroy the database, all data will be lost!')
+group = parser.add_mutually_exclusive_group()
+group.add_argument('-a', '--add', action='store_true', help='add a new password')
+group.add_argument('-d', '--delete', action='store_true', help='delete a password')
+group.add_argument('-u', '--update', action='store_true', help='update a password')
+group.add_argument('-l', '--list-file', action='store_true', help='list database file and configuration file paths')
+group.add_argument('-b', '--backup', action='store_true', help='backup the database file')
+group.add_argument('-p', '--upload', action='store_true', help='upload the database file to a cloud service')
+group.add_argument('-r', '--restore', action='store_true', help='restore the database file from cloud service')
+group.add_argument('-api', '--api', action='store_true', help='set cloud API url and token')
+group.add_argument('-dd', '--destroy', action='store_true', help='destroy the database, all data will be lost!')
 args = parser.parse_args()
 
 
 class CommandHandler:
 
     def __init__(self):
+        if len(sys.argv) > 2:
+            print('Only one argument is allowed!')
+
         self.conf_utils = ConfUtils()
         self.run_trigger = True
         self.add_arg = args.add
         self.delete_arg = args.delete
         self.update_arg = args.update
         self.list_files_arg = args.list_file
         self.destroy_arg = args.destroy
         self.backup_arg = args.backup
         self.upload_arg = args.upload
         self.restore_arg = args.restore
         self.api_arg = args.api
 
+
         try:
             self.conf_utils.get('db', 'database_file')
             self.conf_utils.get('common', 'aes_key')
         except (configparser.NoSectionError, configparser.NoOptionError):
 
             self.run_trigger = False
             try:
@@ -111,15 +118,20 @@
         try:
             query_string = input('Enter a query string: ')
             passwords = self.password_manager.get_password(query_string)
             if len(passwords) > 0:
                 if len(passwords) == 1:
                     self.show_password(passwords[0])
                 else:
-                    menu_items = [f'#{password[0]} \| name: {password[1]} \| url: {password[5]} \| {password[4]}' for password in passwords]
+                    menu_items = []
+                    for password in passwords:
+                        item = f'#{password[0]} \| {password[1]} \| {password[5]} \| {password[4]}'
+                        if len(item) > 40:
+                            item = item[:40] + '...'
+                        menu_items.append(item)
                     menu = TerminalMenu(menu_items)
                     menu_entry_index = menu.show()
                     selected_password = passwords[menu_entry_index]
                     self.show_password(selected_password)
             else:
                 print('No password found!')
```

### Comparing `minipassword-1.0.0/src/minipassword.egg-info/PKG-INFO` & `minipassword-1.0.1/src/minipassword.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipassword
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mini Password is a command-line password manager.
 Home-page: https://github.com/laonan/minipassword
 Author: Laonan
 Author-email: hello@laonan.net
 Project-URL: Bug Tracker, https://github.com/laonan/minipassword/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `minipassword-1.0.0/tests/test_conf.py` & `minipassword-1.0.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.0/tests/test_manager.py` & `minipassword-1.0.1/tests/test_manager.py`

 * *Files identical despite different names*

