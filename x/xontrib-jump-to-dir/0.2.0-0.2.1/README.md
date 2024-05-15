# Comparing `tmp/xontrib-jump-to-dir-0.2.0.tar.gz` & `tmp/xontrib_jump_to_dir-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-jump-to-dir-0.2.0.tar", last modified: Thu Feb 22 21:23:44 2024, max compression
+gzip compressed data, was "xontrib_jump_to_dir-0.2.1.tar", last modified: Wed May 15 18:00:53 2024, max compression
```

## Comparing `xontrib-jump-to-dir-0.2.0.tar` & `xontrib_jump_to_dir-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:23:44.504860 xontrib-jump-to-dir-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-22 21:23:44.504860 xontrib-jump-to-dir-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 21:23:44.504860 xontrib-jump-to-dir-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:23:44.500860 xontrib-jump-to-dir-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/tests/test_xontrib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:23:44.500860 xontrib-jump-to-dir-0.2.0/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-22 21:23:35.000000 xontrib-jump-to-dir-0.2.0/xontrib/jump_to_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:23:44.500860 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-22 21:23:44.000000 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-22 21:23:44.000000 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 21:23:44.000000 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 21:23:44.000000 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 21:23:44.000000 xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:00:53.625811 xontrib_jump_to_dir-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-15 18:00:53.625811 xontrib_jump_to_dir-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:00:53.625811 xontrib_jump_to_dir-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:00:53.621811 xontrib_jump_to_dir-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/tests/test_xontrib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:00:53.621811 xontrib_jump_to_dir-0.2.1/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-15 18:00:49.000000 xontrib_jump_to_dir-0.2.1/xontrib/jump_to_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:00:53.625811 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-15 18:00:53.000000 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 18:00:53.000000 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:00:53.000000 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 18:00:53.000000 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:00:53.000000 xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/top_level.txt
```

### Comparing `xontrib-jump-to-dir-0.2.0/LICENSE` & `xontrib_jump_to_dir-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-jump-to-dir-0.2.0/PKG-INFO` & `xontrib_jump_to_dir-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-jump-to-dir
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.2.0 Summary: Jump to
+Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.2.1 Summary: Jump to
 used before directory by part of the path. Lightweight zero-dependency
 implementation of autojump or zoxide projects functionality. Author-email:
 anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `xontrib-jump-to-dir-0.2.0/README.md` & `xontrib_jump_to_dir-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-jump-to-dir-0.2.0/pyproject.toml` & `xontrib_jump_to_dir-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "xontrib-jump-to-dir"
-version = "0.2.0"
+version = "0.2.1"
 license = {file = "LICENSE"}
 description = "Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
```

### Comparing `xontrib-jump-to-dir-0.2.0/xontrib/jump_to_dir.py` & `xontrib_jump_to_dir-0.2.1/xontrib/jump_to_dir.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,13 +29,13 @@
                     break
         finally:
             con.close()
 
         return 0 if success else 1
 
     _sc = __xonsh__.env.get('XONTRIB_JUMP_TO_DIR_SHORTCUT', 'j')
-    aliases[_sc] = functools.partial(_jump_to_dir, search_column='cwd', shortcut=_sc)
-    aliases[_sc+'c'] = functools.partial(_jump_to_dir, search_column='inp', shortcut=_sc)
+    aliases[_sc] = lambda args: _jump_to_dir(args, search_column='cwd', shortcut=_sc)
+    aliases[_sc+'c'] = lambda args: _jump_to_dir(args, search_column='inp', shortcut=_sc)
 
 elif __xonsh__.env.get('XONTRIB_JUMP_TO_DIR_WARNING', True):
     print(f"xontrib-jump-to-dir: You're using {_hist_backend} for history backend. It's not supported for jump.")
     print("xontrib-jump-to-dir: Feel free to contribute: https://github.com/anki-code/xontrib-jump-to-dir")
```

### Comparing `xontrib-jump-to-dir-0.2.0/xontrib_jump_to_dir.egg-info/PKG-INFO` & `xontrib_jump_to_dir-0.2.1/xontrib_jump_to_dir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-jump-to-dir
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jump to used before directory by part of the path. Lightweight zero-dependency implementation of autojump or zoxide projects functionality.
 Author-email: anki-code <no@no.no>
 License: MIT License
         
         Copyright (c) 2023, anki-code
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.2.0 Summary: Jump to
+Metadata-Version: 2.1 Name: xontrib-jump-to-dir Version: 0.2.1 Summary: Jump to
 used before directory by part of the path. Lightweight zero-dependency
 implementation of autojump or zoxide projects functionality. Author-email:
 anki-code
 no.no> License: MIT License Copyright (c) 2023, anki-code Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

