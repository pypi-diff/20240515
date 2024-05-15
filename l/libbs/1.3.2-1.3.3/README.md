# Comparing `tmp/libbs-1.3.2.tar.gz` & `tmp/libbs-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.3.2.tar", last modified: Tue May 14 16:10:05 2024, max compression
+gzip compressed data, was "libbs-1.3.3.tar", last modified: Wed May 15 18:52:13 2024, max compression
```

## Comparing `libbs-1.3.2.tar` & `libbs-1.3.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.851747 libbs-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 16:10:01.000000 libbs-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-14 16:10:05.851747 libbs-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-14 16:10:01.000000 libbs-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.839746 libbs-1.3.2/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.839746 libbs-1.3.2/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.843747 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.847746 libbs-1.3.2/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.847746 libbs-1.3.2/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.847746 libbs-1.3.2/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.847746 libbs-1.3.2/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.847746 libbs-1.3.2/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.851747 libbs-1.3.2/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.851747 libbs-1.3.2/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 16:10:01.000000 libbs-1.3.2/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.851747 libbs-1.3.2/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 16:10:05.000000 libbs-1.3.2/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 16:10:05.851747 libbs-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 16:10:01.000000 libbs-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:10:05.851747 libbs-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-14 16:10:01.000000 libbs-1.3.2/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-14 16:10:01.000000 libbs-1.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-14 16:10:01.000000 libbs-1.3.2/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 18:51:56.000000 libbs-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 18:52:13.731921 libbs-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-15 18:51:56.000000 libbs-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.719921 libbs-1.3.3/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.723921 libbs-1.3.3/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89855 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.727921 libbs-1.3.3/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32836 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12644 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 18:51:56.000000 libbs-1.3.3/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 18:52:13.000000 libbs-1.3.3/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 18:52:13.731921 libbs-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 18:51:56.000000 libbs-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:13.731921 libbs-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-15 18:51:56.000000 libbs-1.3.3/tests/test_decompilers.py
```

### Comparing `libbs-1.3.2/LICENSE` & `libbs-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/PKG-INFO` & `libbs-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.3.2/README.md` & `libbs-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/__main__.py` & `libbs-1.3.3/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/api/artifact_dict.py` & `libbs-1.3.3/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/api/artifact_lifter.py` & `libbs-1.3.3/libbs/api/artifact_lifter.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,36 +29,30 @@
     # Override Mandatory Funcs
     #
 
     def lift_type(self, type_str: str) -> str:
         pass
 
     def lift_addr(self, addr: int) -> int:
-        # TODO: there seems to be a bug in how we are using this in BinSync/DAILA. When used in DAILA,
-        #   there are cases where the addr is < binary_base_addr, but we still need to lift it, but removing this
-        #   check breaks BinSync. Need to investigate further.
         if addr < self.deci.binary_base_addr:
-            self.deci.debug(f"Lifting an address that appears already lifted: {addr}...")
-            return addr
-        else:
-            return addr - self.deci.binary_base_addr
+            self.deci.warning(f"Lifting an address that appears already lifted: {addr}...")
+
+        return addr - self.deci.binary_base_addr
 
     def lift_stack_offset(self, offset: int, func_addr: int) -> int:
         pass
 
     def lower_type(self, type_str: str) -> str:
         pass
 
     def lower_addr(self, addr: int) -> int:
-        # TODO: see comment in lift_addr
         if addr >= self.deci.binary_base_addr:
-            self.deci.debug(f"Lowering an address that appears already lowered: {addr}...")
-            return addr
-        else:
-            return addr + self.deci.binary_base_addr
+            self.deci.warning(f"Lowering an address that appears already lowered: {addr}...")
+
+        return addr + self.deci.binary_base_addr
 
     def lower_stack_offset(self, offset: int, func_addr: int) -> int:
         pass
 
     #
     # Private
     #
```

### Comparing `libbs-1.3.2/libbs/api/decompiler_interface.py` & `libbs-1.3.3/libbs/api/decompiler_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,35 +247,35 @@
     def decompiler_available(self) -> bool:
         """
         @return: True if decompiler is available for decompilation, False if otherwise
         """
         return True
 
     def decompile(self, addr: int) -> Optional[str]:
-        addr = self.art_lifter.lower_addr(addr)
+        lowered_addr = self.art_lifter.lower_addr(addr)
         if not self.decompiler_available:
             _l.error("Decompiler is not available.")
             return None
 
         # TODO: make this a function call after transitioning decompiler artifacts to LiveState
-        for func_addr, func in self._functions().items():
-            if func.addr <= addr < (func.addr + func.size):
+        sorted_funcs = sorted(self._functions().items(), key=lambda x: x[0])
+        for func_addr, func in sorted_funcs:
+            if func.addr <= lowered_addr < (func.addr + func.size):
                 break
         else:
             func = None
 
         if func is None:
-            self.warning(f"Failed to find function for address {hex(addr)}")
+            self.warning(f"Failed to find function for address {hex(lowered_addr)}")
             return None
 
-        func = self.art_lifter.lower(func)
         try:
             decompilation = self._decompile(func)
         except Exception as e:
-            self.warning(f"Failed to decompile function at {hex(addr)}: {e}")
+            self.warning(f"Failed to decompile function at {hex(lowered_addr)}: {e}")
             decompilation = None
 
         return decompilation
 
     def xrefs_to(self, artifact: Artifact) -> List[Artifact]:
         """
         Returns a list of artifacts that reference the provided artifact.
@@ -286,15 +286,15 @@
 
     def get_func_containing(self, addr: int) -> Optional[Function]:
         raise NotImplementedError
 
     def _decompile(self, function: Function) -> Optional[str]:
         raise NotImplementedError
 
-    def get_decompilation_object(self, function: Function) -> Optional[object]:
+    def get_decompilation_object(self, function: Function, **kwargs) -> Optional[object]:
         raise NotImplementedError
 
     #
     # Override Optional API:
     # These are API that provide extra introspection for plugins that may rely on LibBS Interface
     #
 
@@ -454,43 +454,63 @@
         return {}
 
     # others...
     def _set_function_header(self, fheader: FunctionHeader, **kwargs) -> bool:
         return False
 
     #
-    # Change Callback API
+    # Change Callback API:
+    # Every callback in this group assumes the input will be decompiler-specific (lowered) and will
+    # lift it ONCE inside this function. Each one will return the lifted form, for easier overriding.
     #
 
-    def function_header_changed(self, fheader: FunctionHeader, **kwargs):
+    def function_header_changed(self, fheader: FunctionHeader, **kwargs) -> FunctionHeader:
+        lifted_fheader = self.art_lifter.lift(fheader)
         for callback_func in self.artifact_write_callbacks[FunctionHeader]:
-            threading.Thread(target=callback_func, args=(fheader,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_fheader,), kwargs=kwargs, daemon=True).start()
 
-    def stack_variable_changed(self, svar: StackVariable, **kwargs):
+        return lifted_fheader
+
+    def stack_variable_changed(self, svar: StackVariable, **kwargs) -> StackVariable:
+        lifted_svar = self.art_lifter.lift(svar)
         for callback_func in self.artifact_write_callbacks[StackVariable]:
-            threading.Thread(target=callback_func, args=(svar,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_svar,), kwargs=kwargs, daemon=True).start()
+
+        return lifted_svar
 
-    def comment_changed(self, comment: Comment, deleted=False, **kwargs):
+    def comment_changed(self, comment: Comment, deleted=False, **kwargs) -> Comment:
         kwargs["deleted"] = deleted
+        lifted_cmt = self.art_lifter.lift(comment)
         for callback_func in self.artifact_write_callbacks[Comment]:
-            threading.Thread(target=callback_func, args=(comment,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_cmt,), kwargs=kwargs, daemon=True).start()
+
+        return lifted_cmt
 
-    def struct_changed(self, struct: Struct, deleted=False, **kwargs):
+    def struct_changed(self, struct: Struct, deleted=False, **kwargs) -> Struct:
         kwargs["deleted"] = deleted
+        lifted_struct = self.art_lifter.lift(struct)
         for callback_func in self.artifact_write_callbacks[Struct]:
-            threading.Thread(target=callback_func, args=(struct,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_struct,), kwargs=kwargs, daemon=True).start()
 
-    def enum_changed(self, enum: Enum, deleted=False, **kwargs):
+        return lifted_struct
+
+    def enum_changed(self, enum: Enum, deleted=False, **kwargs) -> Enum:
         kwargs["deleted"] = deleted
+        lifted_enum = self.art_lifter.lift(enum)
         for callback_func in self.artifact_write_callbacks[Enum]:
-            threading.Thread(target=callback_func, args=(enum,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_enum,), kwargs=kwargs, daemon=True).start()
+
+        return lifted_enum
 
-    def global_variable_changed(self, gvar: GlobalVariable, **kwargs):
+    def global_variable_changed(self, gvar: GlobalVariable, **kwargs) -> GlobalVariable:
+        lifted_gvar = self.art_lifter.lift(gvar)
         for callback_func in self.artifact_write_callbacks[GlobalVariable]:
-            threading.Thread(target=callback_func, args=(gvar,), kwargs=kwargs, daemon=True).start()
+            threading.Thread(target=callback_func, args=(lifted_gvar,), kwargs=kwargs, daemon=True).start()
+
+        return lifted_gvar
 
     #
     # Special Loggers and Printers
     #
 
     def print(self, msg: str, **kwargs):
         print(msg)
```

### Comparing `libbs-1.3.2/libbs/api/type_parser.py` & `libbs-1.3.3/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/api/utils.py` & `libbs-1.3.3/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/__init__.py` & `libbs-1.3.3/libbs/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/artifact.py` & `libbs-1.3.3/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/comment.py` & `libbs-1.3.3/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/decompilation.py` & `libbs-1.3.3/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/enum.py` & `libbs-1.3.3/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/func.py` & `libbs-1.3.3/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/global_variable.py` & `libbs-1.3.3/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/patch.py` & `libbs-1.3.3/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/stack_variable.py` & `libbs-1.3.3/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/artifacts/struct.py` & `libbs-1.3.3/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.3.3/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
         """wait for the response"""
         if timeout is not None and timeout < 0:
             # can't pass in None higher up reliably, as it gets used to indicate "default timeout".
             # Instead, treat a negative timeout as "wait forever", and set timeout to None, so event.wait
             # will wait forever.
             timeout = None
 
-        if not self.event.wait(timeout):
+        if not self.event.wait(None):
             raise BridgeTimeoutException(
                 "Didn't receive response {} before timeout".format(self.response_id)
             )
 
         return self.response
```

### Comparing `libbs-1.3.2/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.3.3/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/angr/compat.py` & `libbs-1.3.3/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/angr/interface.py` & `libbs-1.3.3/libbs/decompilers/angr/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,21 +105,21 @@
 
         return xrefs
 
     def _decompile(self, function: Function) -> Optional[str]:
         if function.dec_obj is not None:
             dec_text = function.dec_obj.text
         else:
-            function.dec_obj = self.get_decompilation_object(function)
+            function.dec_obj = self.get_decompilation_object(function, do_lower=False)
             dec_text = function.dec_obj.text if function.dec_obj else None
 
         return dec_text
 
-    def get_decompilation_object(self, function: Function) -> Optional[object]:
-        func_addr = self.art_lifter.lower_addr(function.addr)
+    def get_decompilation_object(self, function: Function, do_lower=True, **kwargs) -> Optional[object]:
+        func_addr = self.art_lifter.lower_addr(function.addr) if do_lower else function.addr
         func = self.main_instance.project.kb.functions.get(func_addr, None)
         if func is None:
             return None
 
         try:
             codegen = self.decompile_function(func)
         except Exception as e:
@@ -191,22 +191,21 @@
         )
 
     #
     # Artifact API
     #
 
     def _set_function(self, func: Function, **kwargs) -> bool:
-        func_addr = self.art_lifter.lower_addr(func.addr)
-        angr_func = self.main_instance.project.kb.functions[func_addr]
+        angr_func = self.main_instance.project.kb.functions[func.addr]
 
         # re-decompile a function if needed
         decompilation = self.decompile_function(angr_func)
         changes = super()._set_function(func, decompilation=decompilation, **kwargs)
         if not self.headless:
-            self.refresh_decompilation(func_addr)
+            self.refresh_decompilation(func.addr)
 
         return changes
 
     def _get_function(self, addr, **kwargs) -> Optional[Function]:
         try:
             _func = self.main_instance.project.kb.functions[addr]
         except KeyError:
```

### Comparing `libbs-1.3.2/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.3.3/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/binja/hooks.py` & `libbs-1.3.3/libbs/decompilers/binja/hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,35 +49,31 @@
                 for addr, prev_comment in prev_comments.items():
                     curr_comment = current_comments.get(addr, None)
                     # no change for this comment
                     if curr_comment == prev_comment:
                         continue
 
                     self._interface.comment_changed(
-                        self._interface.art_lifter.lift(
-                            Comment(
-                                addr,
-                                str(curr_comment) if curr_comment else "",
-                                decompiled=True,
-                                func_addr=func_addr
-                            )
+                        Comment(
+                            addr,
+                            str(curr_comment) if curr_comment else "",
+                            decompiled=True,
+                            func_addr=func_addr
                         ),
                         deleted=curr_comment is None,
                     )
 
                 # Find any comment which was newly added in this change
                 for addr, curr_comment in current_comments.items():
                     if addr in prev_comments:
                         continue
 
                     if curr_comment:
                         self._interface.comment_changed(
-                            self._interface.art_lifter.lift(
-                                Comment(addr, str(curr_comment), decompiled=True, func_addr=func_addr)
-                            )
+                            Comment(addr, str(curr_comment), decompiled=True, func_addr=func_addr)
                         )
 
                 self._seen_comments[func_addr] = current_comments
 
         # service requested function only
         if self._changing_func_pre_change is not None and self._changing_func_addr == func_.start:
             l.debug(f"Update on {hex(self._changing_func_addr)} being processed...")
@@ -115,31 +111,26 @@
                     if old_arg.type != new_arg.type:
                         diff_arg.type = str(new_arg.type)
 
                     if old_arg.size != new_arg.size:
                         diff_arg.size = int(new_arg.size)
 
                     self._interface.function_header_changed(
-                        self._interface.art_lifter.lift(
-                            FunctionHeader(None, old_header.addr, args={off: diff_arg})
-                        )
+                        FunctionHeader(None, old_header.addr, args={off: diff_arg})
                     )
 
                 # new func args added to header
                 for off, new_arg in bs_func.args.items():
                     if off in old_args:
                         continue
 
                     self._interface.function_header_changed(
-                        self._interface.art_lifter.lift(
-                            FunctionHeader(None, old_header.addr, args={
-                                    off: FunctionArgument(off, str(new_arg.name), str(new_arg.type), int(new_arg.size))
-                                }
-                            )
-                        )
+                        FunctionHeader(None, old_header.addr, args={
+                            off: FunctionArgument(off, str(new_arg.name), str(new_arg.type), int(new_arg.size))
+                        })
                     )
 
             #
             # stack vars
             #
 
             header_args_names = set([arg.name for arg in bs_func.header.args.values()])
@@ -158,26 +149,22 @@
                     diff_sv = StackVariable(off, None, None, old_sv.size, bs_func.addr)
                     if old_sv.name != new_sv.name:
                         diff_sv.name = str(new_sv.name)
 
                     if old_sv.type != new_sv.type:
                         diff_sv.type = str(new_sv.type)
 
-                    self._interface.stack_variable_changed(
-                        self._interface.art_lifter.lift(diff_sv)
-                    )
+                    self._interface.stack_variable_changed(diff_sv)
 
                 for off, new_sv in new_svs.items():
                     if off in old_svs or new_sv.name in header_args_names:
                         continue
 
                     self._interface.stack_variable_changed(
-                        self._interface.art_lifter.lift(
-                            StackVariable(off, str(new_sv.name), str(new_sv.type), new_sv.size, bs_func.addr)
-                        )
+                        StackVariable(off, str(new_sv.name), str(new_sv.type), new_sv.size, bs_func.addr)
                     )
 
             self._changing_func_pre_change = None
 
     def function_update_requested(self, view, func):
         if self._changing_func_addr is None:
             l.debug(f"Update on {func} requested...")
@@ -187,34 +174,28 @@
     def symbol_updated(self, view, sym):
         l.debug(f"Symbol update Requested on {sym}...")
         if sym.type == SymbolType.FunctionSymbol:
             l.debug(f"   -> Function Symbol")
             func = view.get_function_at(sym.address)
             bs_func = BinjaInterface.bn_func_to_bs(func)
             self._interface.function_header_changed(
-                self._interface.art_lifter.lift(FunctionHeader(bs_func.name, bs_func.addr))
+                FunctionHeader(bs_func.name, bs_func.addr)
             )
         elif sym.type == SymbolType.DataSymbol:
             l.debug(f"   -> Data Symbol")
             var: binaryninja.DataVariable = view.get_data_var_at(sym.address)
             self._interface.global_variable_changed(
-                self._interface.art_lifter.lift(
-                    GlobalVariable(int(sym.address), str(var.name), type_=str(var.type), size=int(var.type.width))
-                )
+                GlobalVariable(int(sym.address), str(var.name), type_=str(var.type), size=int(var.type.width))
             )
         else:
             print(f"   -> Other Symbol: {sym.type}")
             pass
 
     def type_defined(self, view, name, type_):
         l.debug(f"Type Defined: {name} {type_}")
         name = str(name)
         if isinstance(type_, StructureType):
             bs_struct = BinjaInterface.bn_struct_to_bs(name, type_)
-            self._interface.struct_changed(
-                self._interface.art_lifter.lift(bs_struct)
-            )
+            self._interface.struct_changed(bs_struct)
         elif isinstance(type_, EnumerationType):
             bs_enum = BinjaInterface.bn_enum_to_bs(name, type_)
-            self._interface.enum_changed(
-                self._interface.art_lifter.lift(bs_enum)
-            )
+            self._interface.enum_changed(bs_enum)
```

### Comparing `libbs-1.3.2/libbs/decompilers/binja/interface.py` & `libbs-1.3.3/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.3.3/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.3.3/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ghidra/hooks.py` & `libbs-1.3.3/libbs/decompilers/ghidra/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,36 +81,31 @@
                         if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
                             gvar = GlobalVariable(obj.getAddress().getOffset(), obj.getName())
                             self._interface.global_variable_changed(gvar)
                     elif changeType == self.changeManager.DOCR_SYMBOL_RENAMED:
                         if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
                             gvar = GlobalVariable(obj.getAddress().getOffset(), newValue)
                             self._interface.global_variable_changed(gvar)
-
                         if self._interface.ghidra.isinstance(obj, self.db.symbol.FunctionSymbol):
                             header = FunctionHeader(newValue, int(obj.getAddress().offset))
-                            self._interface.function_header_changed(
-                                self._interface.art_lifter.lift(header)
-                            )
+                            self._interface.function_header_changed(header)
                     elif self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
                         parent_namespace = obj.getParentNamespace()
                         storage = obj.getVariableStorage()
                         if (
                             (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
                             and (parent_namespace is not None)
                         ):
                             self._interface.stack_variable_changed(
-                                self._interface.art_lifter.lift(
-                                    StackVariable(
-                                        int(obj.variableStorage.stackOffset),
-                                        newValue,
-                                        None,
-                                        None,
-                                        int(obj.parentNamespace.entryPoint.offset)
-                                    )
+                                StackVariable(
+                                    int(obj.variableStorage.stackOffset),
+                                    newValue,
+                                    None,
+                                    None,
+                                    int(obj.parentNamespace.entryPoint.offset)
                                 )
                             )
                         else:
                             # TODO: figure out how to differentiate type changes
                             # print(f"VariableSymbolDB caught: {obj}")
                             # print(f"Obj type: {type(obj)}")
                             # print(f"Old value: {oldValue}")
@@ -127,14 +122,15 @@
                         pass
                     else:
                         continue
 
     data_monitor = DataMonitor(interface)
     return data_monitor
 
+
 def create_context_action(ghidra: "GhidraAPIWrapper", name, action_string, callback_func, category=None):
     ProgramLocationContextAction = ghidra.import_module_object("ghidra.app.context", "ProgramLocationContextAction")
     MenuData = ghidra.import_module_object("docking.action", "MenuData")
 
     # XXX: you can't ever use super().__init__() due to some remote import issues
     class GenericDecompilerCtxAction(ProgramLocationContextAction):
         def actionPerformed(self, ctx):
```

### Comparing `libbs-1.3.2/libbs/decompilers/ghidra/interface.py` & `libbs-1.3.3/libbs/decompilers/ghidra/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,26 +208,27 @@
         return int(gfunc.getBody().getNumAddresses())
 
     def connect_ghidra_bridge(self):
         self.ghidra = GhidraAPIWrapper(self, connection_timeout=25)
         return self.ghidra.connected
 
     def _decompile(self, function: Function) -> Optional[str]:
-        dec_obj = self.get_decompilation_object(function)
+        dec_obj = self.get_decompilation_object(function, do_lower=False)
         if dec_obj is None:
             return None
 
         dec_func = dec_obj.getDecompiledFunction()
         if dec_func is None:
             return None
 
         return str(dec_func.getC())
 
-    def get_decompilation_object(self, function: Function) -> Optional[object]:
-        return self._ghidra_decompile(self._get_nearest_function(self.art_lifter.lower_addr(function.addr)))
+    def get_decompilation_object(self, function: Function, do_lower=True) -> Optional[object]:
+        lowered_addr = self.art_lifter.lower_addr(function.addr) if do_lower else function.addr
+        return self._ghidra_decompile(self._get_nearest_function(lowered_addr))
 
     #
     # Extra API
     #
 
     def undo(self):
         self.ghidra.currentProgram.undo()
@@ -249,16 +250,15 @@
         return self._update_local_variable_symbols(symbols_to_update) if symbols_to_update else False
 
     #
     # Private Artifact API
     #
 
     def _set_function(self, func: Function, **kwargs) -> bool:
-        func_addr = self.art_lifter.lower_addr(func.header.addr)
-        decompilation = self._ghidra_decompile(self._get_nearest_function(func_addr))
+        decompilation = self._ghidra_decompile(self._get_nearest_function(func.addr))
         changes = super()._set_function(func, decompilation=decompilation, **kwargs)
         return changes
 
     def _get_function(self, addr, **kwargs) -> Optional[Function]:
         func = self._get_nearest_function(addr)
         dec = self._ghidra_decompile(func)
         # optimize on remote
@@ -353,14 +353,15 @@
     def _set_function_header(self, fheader: FunctionHeader, decompilation=None, **kwargs) -> bool:
         changes = False
         func_addr = fheader.addr
         ghidra_func = decompilation.getFunction() if decompilation else self._get_nearest_function(func_addr)
         src_type = self.ghidra.import_module_object("ghidra.program.model.symbol", "SourceType")
 
         # func name
+        self.info(f"Setting function header: {fheader}")
         if fheader.name and fheader.name != ghidra_func.getName():
             with Transaction(self.ghidra, msg="BS::set_function_header::set_name"):
                 ghidra_func.setName(fheader.name, src_type.USER_DEFINED)
             changes = True
 
         # return type
         if fheader.type and decompilation is not None:
@@ -373,18 +374,16 @@
 
         # args
         # TODO: Only works for function arguments passed by register
         if fheader.args and decompilation is not None:
             high_func_util = self.ghidra.import_module_object("ghidra.program.model.pcode", "HighFunctionDBUtil")
             params = ghidra_func.getParameters()
             if len(params) == 0:
-                self.info("Commiting some atuff")
                 with Transaction(self.ghidra, msg="BS::set_function_header::update_params"):
                     high_func_util.commitParamsToDatabase(decompilation.highFunction, True, src_type.USER_DEFINED)
-                self.info("Done commiting ")
 
             with Transaction(self.ghidra, msg="BS::set_function_header::set_arguments"):
                 for offset, param in zip(fheader.args, params):
                     arg = fheader.args[offset]
                     gtype = self.typestr_to_gtype(arg.type)
                     param.setName(arg.name, src_type.USER_DEFINED)
                     param.setDataType(gtype, src_type.USER_DEFINED)
```

### Comparing `libbs-1.3.2/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.3.3/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ida/compat.py` & `libbs-1.3.3/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ida/hooks.py` & `libbs-1.3.3/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/decompilers/ida/interface.py` & `libbs-1.3.3/libbs/decompilers/ida/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
             if from_func_addr is None:
                 continue
 
             xrefs.append(Function(from_func_addr, 0))
 
         return xrefs
 
-    def get_decompilation_object(self, function: Function) -> Optional[object]:
-        function = self.art_lifter.lower(function)
+    def get_decompilation_object(self, function: Function, do_lower=True, **kwargs) -> Optional[object]:
+        function = self.art_lifter.lower(function) if do_lower else function
         dec = idaapi.decompile(function.addr)
         if dec is None:
             return None
 
         return dec
 
     def _decompile(self, function: Function) -> Optional[str]:
```

### Comparing `libbs-1.3.2/libbs/logger.py` & `libbs-1.3.3/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/plugin_installer.py` & `libbs-1.3.3/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/ui/__init__.py` & `libbs-1.3.3/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/ui/qt_objects.py` & `libbs-1.3.3/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs/ui/utils.py` & `libbs-1.3.3/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/libbs.egg-info/PKG-INFO` & `libbs-1.3.3/libbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.3.2
+Version: 1.3.3
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.3.2/libbs.egg-info/SOURCES.txt` & `libbs-1.3.3/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/setup.cfg` & `libbs-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/tests/test_artifacts.py` & `libbs-1.3.3/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/tests/test_cli.py` & `libbs-1.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.3.2/tests/test_decompilers.py` & `libbs-1.3.3/tests/test_decompilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,22 @@
         assert first_changed_func.name == "changed"
         assert first_changed_func.addr == func_addr
         assert len(hits[FunctionHeader]) == 2
 
         # global var names
         # TODO: The gvar test cant function until gvar setting is fixed
         old_global_hits = len(hits[GlobalVariable])
-        g1 = deci.global_vars[0x4008e0]
-        g2 = deci.global_vars[0x601048]
+        g1_addr = deci.art_lifter.lift_addr(0x4008e0)
+        g2_addr = deci.art_lifter.lift_addr(0x601048)
+        g1 = deci.global_vars[g1_addr]
+        g2 = deci.global_vars[g2_addr]
         g1.name = "gvar1"
         g2.name = "gvar2"
-        deci.global_vars[0x4008e0] = g1
-        deci.global_vars[0x601048] = g2
+        deci.global_vars[g1_addr] = g1
+        deci.global_vars[g2_addr] = g2
         # assert len(hits[GlobalVariable]) == old_global_hits + 2
 
         # TODO: Fix CI for below
         main.stack_vars[-24].name = "named_char_array"
         main.stack_vars[-12].name = "named_int"
         deci.functions[func_addr] = main
         #first_changed_sv = hits[StackVariable][0]
```

